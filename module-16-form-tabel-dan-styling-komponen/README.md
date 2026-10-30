# Modul 16: Form, Tabel, dan Styling Komponen

## Ringkasan Ruang Lingkup Materi

Modul ini membahas teknik styling dan kustomisasi antarmuka pengguna (UI) penting dalam web development: styling input formulir, status fokus (:focus, :focus-visible) yang aksesibel, umpan balik validasi visual (:valid, :invalid, :user-invalid), kustomisasi kontrol seleksi native (checkbox dan radio button), perancangan sistem komponen tombol (button variants & states), tipografi dan tata letak tabel data standar, pemberian warna bergantian (zebra striping) dan efek sorot baris, teknik penyajian tabel responsif pada layar sempit, perancangan bilah gulir kustom (custom scrollbar standar W3C & WebKit), hingga styling komponen interaktif akordeon native berbasis elemen HTML5 <details> dan <summary>.

## Tujuan Pembelajaran Modul

- Mengembangkan formulir modern dengan tata visual yang bersih, proporsional, dan nyaman digunakan.
- Menerapkan cincin fokus (:focus-visible) yang memenuhi standar aksesibilitas kontras tinggi WCAG.
- Menampilkan umpan balik visual instan atas validitas data input menggunakan pseudo-class validasi CSS.
- Mendesain komponen kustom checkbox dan radio button yang tetap mendukung aksesibilitas navigasi keyboard.
- Membangun sistem komponen tombol lengkap dengan varian gaya (primary, secondary, danger) dan berbagai ukuran.
- Menata struktur tabel data dengan border-collapse, padding terukur, zebra striping, dan perilaku responsif.
- Menyesuaikan gaya scrollbar serta elemen interaktif akordeon native details/summary secara elegan.

## Daftar Submodul

- [281. Styling input formulir](281_form_input_styling.css) — [Halaman Preview](281_form_input_styling.html)
- [282. Focus states pada formulir](282_form_focus_states.css) — [Halaman Preview](282_form_focus_states.html)
- [283. Validasi visual dengan `:valid` dan `:invalid`](283_form_validation_states.css) — [Halaman Preview](283_form_validation_states.html)
- [284. Styling checkbox dan radio](284_checkbox_radio_styling.css) — [Halaman Preview](284_checkbox_radio_styling.html)
- [285. Komponen tombol](285_button_component.css) — [Halaman Preview](285_button_component.html)
- [286. Styling tabel](286_table_styling.css) — [Halaman Preview](286_table_styling.html)
- [287. Zebra striping pada tabel](287_table_zebra_stripes.css) — [Halaman Preview](287_table_zebra_stripes.html)
- [288. Tabel responsif](288_table_responsive.css) — [Halaman Preview](288_table_responsive.html)
- [289. Styling scrollbar](289_custom_scrollbar.css) — [Halaman Preview](289_custom_scrollbar.html)
- [290. Styling komponen details dan summary](290_details_summary_styling.css) — [Halaman Preview](290_details_summary_styling.html)

---

## Pembahasan dan Penjelasan Submodul

### 281. Styling input formulir

**Tujuan:** Mendesain elemen input teks, email, dan textarea agar rapi, konsisten antar-peramban, dan mudah diisi.

**Konsep Utama:**
Elemen form native memiliki tampilan bawaan peramban yang kaku. Menghilangkan border default, menambahkan padding seimbang, border-radius halus, tipografi konsisten, dan kustomisasi ::placeholder menghasilkan pengalaman input yang ramah pengguna.

**Penjelasan Source Code:**
Mengatur kelompok form field dengan label berjarak teratur, input box bersudut melengkung, transisi halus, dan styling placeholder teks.

**Source code utama:** [281_form_input_styling.css](281_form_input_styling.css)

**File pendukung preview:** [281_form_input_styling.html](281_form_input_styling.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "281_form_input_styling.html"
```

**Hasil yang Diharapkan:**
Formulir masukan modern dengan label rapi, placeholder abu-abu elegan, dan bingkai input bersahabat.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Styling input formulir](output/281_form_input_styling.png)

---

### 282. Focus states pada formulir

**Tujuan:** Mengelola status visual fokus elemen form dengan membedakan :focus dan :focus-visible secara aksesibel.

**Konsep Utama:**
Indikator fokus visual sangat krusial bagi navigasi keyboard (aksesibilitas). Menggunakan kombinasi border berwarna kontras dan cincin fokus lembut (box-shadow) memastikan pengguna tahu letak kursor aktif tanpa merusak estetika.

**Penjelasan Source Code:**
Mengimplementasikan cincin fokus biru cerah dengan transisi halus pada event fokus input.

**Source code utama:** [282_form_focus_states.css](282_form_focus_states.css)

**File pendukung preview:** [282_form_focus_states.html](282_form_focus_states.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "282_form_focus_states.html"
```

**Hasil yang Diharapkan:**
Elemen formulir yang memunculkan glow/cincin fokus biru cerah saat diklik atau diarahkan dengan tombol Tab.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Focus states pada formulir](output/282_form_focus_states.png)

---

### 283. Validasi visual dengan `:valid` dan `:invalid`

**Tujuan:** Menerapkan gaya visual otomatis berdasarkan status validasi formulir bawaan HTML5.

**Konsep Utama:**
CSS menyediakan pseudo-class `:valid`, `:invalid`, serta `:user-invalid` modern untuk memberi indikasi warna batas hijau atau merah seketika data yang diketikkan memenuhi atau melanggar aturan format input (seperti type email atau atribut required).

**Penjelasan Source Code:**
Mendemonstrasikan perubahan warna batas dan ikon bantuan saat input berstatus valid vs invalid.

**Source code utama:** [283_form_validation_states.css](283_form_validation_states.css)

**File pendukung preview:** [283_form_validation_states.html](283_form_validation_states.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "283_form_validation_states.html"
```

**Hasil yang Diharapkan:**
Kotak input yang berubah warna menjadi hijau saat format benar dan merah saat format keliru.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Validasi visual dengan `:valid` dan `:invalid`](output/283_form_validation_states.png)

---

### 284. Styling checkbox dan radio

**Tujuan:** Memodifikasi tampilan kotak centang (checkbox) dan tombol pilihan tunggal (radio) secara kustom dan konsisten.

**Konsep Utama:**
Elemen checkbox dan radio dapat dikustomisasi secara elegan menggunakan properti 'accent-color' untuk kustomisasi cepat, atau teknik menyembunyikan input asli dan membentuk kotak pengganti dengan pseudo-element (:before/:after) yang bereaksi terhadap pseudo-class :checked.

**Penjelasan Source Code:**
Membangun checkbox kustom bertanda centang visual dan radio button kustom dengan bulatan indikator animasi.

**Source code utama:** [284_checkbox_radio_styling.css](284_checkbox_radio_styling.css)

**File pendukung preview:** [284_checkbox_radio_styling.html](284_checkbox_radio_styling.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "284_checkbox_radio_styling.html"
```

**Hasil yang Diharapkan:**
Daftar pilihan checkbox dan radio kustom dengan warna aksen indigo modern dan tanda centang bersih.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Styling checkbox dan radio](output/284_checkbox_radio_styling.png)

---

### 285. Komponen tombol

**Tujuan:** Membangun sistem komponen tombol komprehensif dengan varian gaya (primer, sekunder, bahaya) dan status interaksi.

**Konsep Utama:**
Komponen tombol dirancang modular menggunakan kelas dasar `.btn` untuk tata letak umum (padding, display, border-radius, font-weight), yang dipadukan dengan kelas varian (`.btn-primary`, `.btn-secondary`, `.btn-danger`) serta status hover, active, dan disabled.

**Penjelasan Source Code:**
Mengatur sistem tombol modular dengan berbagai varian warna, ukuran, dan status kursor terdisabled.

**Source code utama:** [285_button_component.css](285_button_component.css)

**File pendukung preview:** [285_button_component.html](285_button_component.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "285_button_component.html"
```

**Hasil yang Diharapkan:**
Deretan tombol antarmuka modern yang seragam, responsif terhadap klik, dan kaya varian gaya.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Komponen tombol](output/285_button_component.png)

---

### 286. Styling tabel

**Tujuan:** Menata struktur dan tipografi tabel data agar profesional, jelas, dan mudah dipindai mata.

**Konsep Utama:**
Tabel HTML sering tampak sempit secara default. Penggunaan `border-collapse: collapse`, padding sel memadai, perataan teks teratur (teks rata kiri, angka rata kanan), border pemisah subtil, dan latar header yang jelas menciptakan tata tabel standar profesional.

**Penjelasan Source Code:**
Mengatur properti border-collapse, lebar 100%, background header gelap/subtil, dan jarak sel data terukur.

**Source code utama:** [286_table_styling.css](286_table_styling.css)

**File pendukung preview:** [286_table_styling.html](286_table_styling.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "286_table_styling.html"
```

**Hasil yang Diharapkan:**
Tabel data produk terstruktur rapi dengan batas garis elegan dan pemisahan baris yang jelas.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Styling tabel](output/286_table_styling.png)

---

### 287. Zebra striping pada tabel

**Tujuan:** Meningkatkan kemudahan membaca baris data panjang melalui teknik belang-belang (zebra striping) dan sorot baris.

**Konsep Utama:**
Teknik 'Zebra striping' menerapkan warna latar bergantian pada baris genap menggunakan selector `tbody tr:nth-child(even)` serta efek sorot baris dengan `tbody tr:hover` guna memandu mata pengguna saat menelusuri data horizontal yang panjang.

**Penjelasan Source Code:**
Mengatur warna latar belang pada baris genap dan perubahan warna latar saat kursor melayang di atas baris.

**Source code utama:** [287_table_zebra_stripes.css](287_table_zebra_stripes.css)

**File pendukung preview:** [287_table_zebra_stripes.html](287_table_zebra_stripes.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "287_table_zebra_stripes.html"
```

**Hasil yang Diharapkan:**
Tabel dengan baris abu-abu lembut bergantian dan efek highlight biru saat baris disorot mouse.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Zebra striping pada tabel](output/287_table_zebra_stripes.png)

---

### 288. Tabel responsif

**Tujuan:** Menangani tampilan tabel data agar tetap nyaman diakses pada perangkat berlayar sempit atau mobile.

**Konsep Utama:**
Tabel data memiliki lebar minimum intrinsik yang berpotensi merusak tata letak mobile. Dua pendekatan utama adalah kontainer pembungkus dengan `overflow-x: auto` (horizontal scroll) dan transformasi baris menjadi kartu data bertumpuk menggunakan pseudo-element `data-label`.

**Penjelasan Source Code:**
Mengombinasikan wrapper overflow untuk tampilan desktop/tablet serta media query transformasi kartu bertumpuk pada layar di bawah 560px.

**Source code utama:** [288_table_responsive.css](288_table_responsive.css)

**File pendukung preview:** [288_table_responsive.html](288_table_responsive.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "288_table_responsive.html"
```

**Hasil yang Diharapkan:**
Tabel yang menampilkan scrollbar geser pada batas kontainer atau berganti bentuk menjadi blok kartu saat layar mengecil.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Tabel responsif](output/288_table_responsive.png)

---

### 289. Styling scrollbar

**Tujuan:** Menyesuaikan gaya visual bilah gulir (scrollbar) agar selaras dengan skema warna desain aplikasi.

**Konsep Utama:**
CSS modern menyediakan properti standar W3C `scrollbar-width` dan `scrollbar-color`. Untuk kompatibilitas peramban berbasis WebKit terdahulu (Chrome, Safari, Edge lama), pseudo-element `::-webkit-scrollbar`, `::-webkit-scrollbar-thumb`, dan `::-webkit-scrollbar-track` digunakan bersamaan.

**Penjelasan Source Code:**
Mengatur properti standar dan pseudo-element WebKit untuk membentuk scrollbar ramping bertema warna ungu lembut.

**Source code utama:** [289_custom_scrollbar.css](289_custom_scrollbar.css)

**File pendukung preview:** [289_custom_scrollbar.html](289_custom_scrollbar.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "289_custom_scrollbar.html"
```

**Hasil yang Diharapkan:**
Kotak teks bergulir dengan bilah geser (scrollbar) ramping berwarna ungu dan jalur latar yang halus.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Styling scrollbar](output/289_custom_scrollbar.png)

---

### 290. Styling komponen details dan summary

**Tujuan:** Mengkustomisasi elemen akordeon interaktif native HTML5 <details> dan <summary> tanpa bantuan JavaScript.

**Konsep Utama:**
Elemen `<details>` dan `<summary>` menyediakan fungsionalitas buka-tutup (collapsible) bawaan. Dengan CSS, kita dapat menghilangkan segitiga marker bawaan (`summary::marker` atau `::-webkit-details-marker`), menambahkan ikon panah chevron kustom dengan rotasi transisi halus saat status `open` aktif.

**Penjelasan Source Code:**
Menghilangkan marker default, menata kartu akordeon dengan padding, dan memutar panah chevron kustom saat elemen details dibuka.

**Source code utama:** [290_details_summary_styling.css](290_details_summary_styling.css)

**File pendukung preview:** [290_details_summary_styling.html](290_details_summary_styling.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "290_details_summary_styling.html"
```

**Hasil yang Diharapkan:**
Kotak akordeon interaktif elegan yang membuka konten pertanyaan-jawaban dengan animasi rotasi panah.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Styling komponen details dan summary](output/290_details_summary_styling.png)

---

## Ringkasan Modul

Komponen formulir dan tabel data merupakan tulang punggung aplikasi web interaktif. Dengan penguasaan teknik styling komponen pada Modul 16, pembelajar mampu menghasilkan antarmuka yang estetis, konsisten, responsif di berbagai ukuran perangkat, serta tetap patuh terhadap standar aksesibilitas keyboard dan pembaca layar.

### Keterkaitan Materi
Seluruh submodul dalam modul ini dirancang secara berjenjang untuk membangun pemahaman yang kokoh dan aplikatif. Lanjutkan ke modul berikutnya setelah menguasai seluruh konsep di atas.
