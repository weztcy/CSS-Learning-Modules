# Modul 04: CSS Box Model

## Ringkasan Ruang Lingkup Materi

Modul ini membedah pilar tata letak utama CSS: Box Model. Pembahasan mencakup 4 lapis anatomi (content, padding, border, margin), perbedaan fundamental antara content-box dan border-box, pengaturan dimensi terikat (min/max width dan height), fenomena margin collapse, teknik centering margin auto, logical properties modern (margin-inline, padding-block), global box sizing reset, hingga intrinsic sizing keywords (min-content, max-content, fit-content) dan aspect-ratio.

## Tujuan Pembelajaran Modul

- Memahami empat lapisan Box Model: Content, Padding, Border, dan Margin.
- Menganalisis perbedaan kalkulasi ukuran antara box-sizing: content-box dan border-box.
- Mengontrol batas dimensi dengan width, height, min-width, max-width, min-height, max-height.
- Mencegah dan memanfaatkan fenomena margin collapsing pada elemen bertumpuk vertikal.
- Menerapkan CSS Logical Properties (margin-inline, padding-block) untuk mendukung internasionalisasi penulisan.
- Menggunakan intrinsic sizing mutakhir dan properti aspect-ratio untuk mempertahankan proporsi elemen.

## Daftar Submodul

- [51. Box model dasar](51_box_model_basic.css) — [Halaman Preview](51_box_model_basic.html)
- [52. box-sizing: content-box](52_content_box.css) — [Halaman Preview](52_content_box.html)
- [53. box-sizing: border-box](53_border_box.css) — [Halaman Preview](53_border_box.html)
- [54. Properti width](54_width_property.css) — [Halaman Preview](54_width_property.html)
- [55. Properti height](55_height_property.css) — [Halaman Preview](55_height_property.html)
- [56. Properti min-width](56_min_width.css) — [Halaman Preview](56_min_width.html)
- [57. Properti max-width](57_max_width.css) — [Halaman Preview](57_max_width.html)
- [58. Properti min-height](58_min_height.css) — [Halaman Preview](58_min_height.html)
- [59. Properti max-height](59_max_height.css) — [Halaman Preview](59_max_height.html)
- [60. Properti margin](60_margin_property.css) — [Halaman Preview](60_margin_property.html)
- [61. Margin collapsing](61_margin_collapse.css) — [Halaman Preview](61_margin_collapse.html)
- [62. Properti padding](62_padding_property.css) — [Halaman Preview](62_padding_property.html)
- [63. Pemusatan menggunakan margin: auto](63_margin_auto.css) — [Halaman Preview](63_margin_auto.html)
- [64. Logical margin properties](64_logical_margin.css) — [Halaman Preview](64_logical_margin.html)
- [65. Logical padding properties](65_logical_padding.css) — [Halaman Preview](65_logical_padding.html)
- [66. Global box sizing](66_box_sizing_global.css) — [Halaman Preview](66_box_sizing_global.html)
- [67. Intrinsic sizing](67_intrinsic_sizing.css) — [Halaman Preview](67_intrinsic_sizing.html)
- [68. min-content dan max-content](68_min_content_max_content.css) — [Halaman Preview](68_min_content_max_content.html)
- [69. Fungsi fit-content()](69_fit_content.css) — [Halaman Preview](69_fit_content.html)
- [70. Properti aspect-ratio](70_aspect_ratio.css) — [Halaman Preview](70_aspect_ratio.html)

---

## Pembahasan dan Penjelasan Submodul

### 51. Box model dasar

**Tujuan:** Memvisualisasikan empat lapisan box model: Content, Padding, Border, dan Margin.

**Konsep Utama:**
Setiap elemen pada halaman web dirender sebagai kotak empat persegi panjang yang terdiri dari: area konten (tempat teks/gambar berada), padding (ruang napas dalam), border (garis pembatas), dan margin (ruang pemisah luar).

**Penjelasan Source Code:**
Mendemonstrasikan kotak dengan warna latar berbeda pada setiap lapis untuk memperlihatkan batas fisik masing-masing komponen box model.

**Source code utama:** [51_box_model_basic.css](51_box_model_basic.css)

**File pendukung preview:** [51_box_model_basic.html](51_box_model_basic.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "51_box_model_basic.html"
```

**Hasil yang Diharapkan:**
Kotak visual bertingkat yang menonjolkan area konten biru, padding kuning lembut, border solid, dan margin.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Box model dasar](output/51_box_model_basic.png)

---

### 52. box-sizing: content-box

**Tujuan:** Memahami perhitungan default box-sizing: content-box di mana padding dan border menambah lebar total.

**Konsep Utama:**
Pada `content-box` (default W3C), properti `width` hanya berlaku untuk area konten. Total lebar elemen di layar adalah: `width + padding-left + padding-right + border-left + border-right`. Ini kerap menyebabkan elemen meluap (overflow).

**Penjelasan Source Code:**
Mendemonstrasikan kotak dengan width: 300px, padding: 30px, dan border: 10px yang total lebarnya membengkak menjadi 380px.

**Source code utama:** [52_content_box.css](52_content_box.css)

**File pendukung preview:** [52_content_box.html](52_content_box.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "52_content_box.html"
```

**Hasil yang Diharapkan:**
Kotak berlabel content-box yang tampak lebih lebar dari lebar yang dideklarasikan.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi box-sizing: content-box](output/52_content_box.png)

---

### 53. box-sizing: border-box

**Tujuan:** Memahami model perhitungan modern border-box di mana padding dan border termasuk dalam width.

**Konsep Utama:**
Pada `border-box`, nilai `width` mencakup konten + padding + border. Jika Anda menetapkan width 300px, maka total elemen akan tetap tepat 300px tanpa membengkak, mempermudah pembuatan tata letak responsif.

**Penjelasan Source Code:**
Membuat kotak dengan lebar pasti 280px yang menyerap padding dan border ke bagian dalam tanpa menambah ukuran luar.

**Source code utama:** [53_border_box.css](53_border_box.css)

**File pendukung preview:** [53_border_box.html](53_border_box.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "53_border_box.html"
```

**Hasil yang Diharapkan:**
Kotak berlabel border-box yang presisi selebar 280px.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi box-sizing: border-box](output/53_border_box.png)

---

### 54. Properti width

**Tujuan:** Mengatur lebar elemen menggunakan satuan tetap (px) dan relatif (%).

**Konsep Utama:**
Properti `width` menentukan lebar horizontal elemen tingkat blok. Nilai persentase mengacu pada lebar elemen induknya, memungkinkan desain responsif yang luwes.

**Penjelasan Source Code:**
Menampilkan kartu dengan lebar fixed 320px dan bar progress dengan width 65% di dalamnya.

**Source code utama:** [54_width_property.css](54_width_property.css)

**File pendukung preview:** [54_width_property.html](54_width_property.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "54_width_property.html"
```

**Hasil yang Diharapkan:**
Komponen kartu dengan bar indikator yang terisi 65% secara proporsional.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti width](output/54_width_property.png)

---

### 55. Properti height

**Tujuan:** Mengatur ketinggian vertikal elemen dan memahami risiko konten meluap.

**Konsep Utama:**
Properti `height` menentukan tinggi elemen. Secara default bernilai `auto` (menyesuaikan konten). Menetapkan fixed height tanpa perencanaan dapat memicu overflow jika konten lebih panjang dari tinggi yang ditentukan.

**Penjelasan Source Code:**
Menata kotak hero banner dengan tinggi tetap 180px dan vertikal align.

**Source code utama:** [55_height_property.css](55_height_property.css)

**File pendukung preview:** [55_height_property.html](55_height_property.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "55_height_property.html"
```

**Hasil yang Diharapkan:**
Spanduk hero berlatar belakang gradasi dengan tinggi pasti 180px dan konten di tengah.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti height](output/55_height_property.png)

---

### 56. Properti min-width

**Tujuan:** Menetapkan batas lebar minimum agar elemen tidak mengecil melebihi batas terbaca.

**Konsep Utama:**
Properti `min-width` mencegah lebar elemen menjadi lebih sempit dari nilai tertentu, bahkan ketika ruang induk atau viewport menyusut.

**Penjelasan Source Code:**
Tombol aksi diberi `min-width: 140px` agar teks pendek sekalipun tetap memiliki ukuran tombol yang proporsional dan mudah diklik.

**Source code utama:** [56_min_width.css](56_min_width.css)

**File pendukung preview:** [56_min_width.html](56_min_width.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "56_min_width.html"
```

**Hasil yang Diharapkan:**
Tombol dengan lebar minimum yang konsisten meskipun label teksnya singkat ('OK').

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti min-width](output/56_min_width.png)

---

### 57. Properti max-width

**Tujuan:** Membatasi lebar maksimum elemen agar tidak melebar berlebihan pada layar besar.

**Konsep Utama:**
Properti `max-width` mencegah elemen melebar melebihi batas yang ditentukan, namun tetap memperbolehkan elemen menyusut fleksibel pada layar yang lebih kecil. Ini adalah kunci tata letak responsif modern.

**Penjelasan Source Code:**
Wadah konten diberi `width: 100%` dan `max-width: 600px` dengan `margin: 0 auto`.

**Source code utama:** [57_max_width.css](57_max_width.css)

**File pendukung preview:** [57_max_width.html](57_max_width.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "57_max_width.html"
```

**Hasil yang Diharapkan:**
Wadah artikel yang elegan di layar desktop lebar dan otomatis menyusut rapi pada layar kecil.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti max-width](output/57_max_width.png)

---

### 58. Properti min-height

**Tujuan:** Menetapkan tinggi minimum elemen namun tetap mengizinkan ekspansi ketika konten bertambah.

**Konsep Utama:**
`min-height` menetapkan tinggi minimal sebuah kotak. Jika konten di dalamnya sedikit, kotak tetap memiliki tinggi minimal tersebut; jika konten bertambah panjang, kotak akan membesar otomatis tanpa overflow.

**Penjelasan Source Code:**
Membuat kartu informasi dengan `min-height: 160px` untuk menjaga keseragaman grid.

**Source code utama:** [58_min_height.css](58_min_height.css)

**File pendukung preview:** [58_min_height.html](58_min_height.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "58_min_height.html"
```

**Hasil yang Diharapkan:**
Kotak yang memiliki ruang vertikal lapang meskipun isi teksnya singkat.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti min-height](output/58_min_height.png)

---

### 59. Properti max-height

**Tujuan:** Membatasi tinggi maksimum elemen yang dipadukan dengan overflow-y: auto untuk kotak scrollable.

**Konsep Utama:**
Properti `max-height` membatasi pertumbuhan vertikal elemen. Sering dipadukan dengan `overflow-y: auto` untuk membuat kotak daftar pesan, log terminal, atau syarat & ketentuan yang dapat digulir.

**Penjelasan Source Code:**
Wadah pesan log dibatasi dengan `max-height: 140px` dan `overflow-y: auto`.

**Source code utama:** [59_max_height.css](59_max_height.css)

**File pendukung preview:** [59_max_height.html](59_max_height.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "59_max_height.html"
```

**Hasil yang Diharapkan:**
Kotak log berketinggian terbatas dengan scrollbar vertikal rapi.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti max-height](output/59_max_height.png)

---

### 60. Properti margin

**Tujuan:** Mengatur margin 4 sisi (top, right, bottom, left) secara individual dan shorthand.

**Konsep Utama:**
Margin mengatur jarak ruang luar di sekeliling elemen. Shorthand margin: 1 nilai (semua sisi), 2 nilai (vertikal horizontal), 3 nilai (top horizontal bottom), 4 nilai (top right bottom left - searah jarum jam).

**Penjelasan Source Code:**
Mendemonstrasikan penataan margin shorthand 2 nilai `margin: 15px 25px` dan shorthand 4 nilai `margin: 10px 20px 30px 40px`.

**Source code utama:** [60_margin_property.css](60_margin_property.css)

**File pendukung preview:** [60_margin_property.html](60_margin_property.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "60_margin_property.html"
```

**Hasil yang Diharapkan:**
Dua kotak yang memperlihatkan spasi jarak luar dengan orientasi simetris dan asimetris.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti margin](output/60_margin_property.png)

---

### 61. Margin collapsing

**Tujuan:** Memahami fenomena runtuhnya margin vertikal ketika dua margin saling bertemu.

**Konsep Utama:**
Margin collapsing adalah perilaku alami CSS di mana margin atas dan margin bawah dari dua elemen blok yang bertetangga melebur menjadi satu margin tunggal sebesar nilai margin yang paling besar (bukan dijumlahkan).

**Penjelasan Source Code:**
Dua kotak bertetangga dengan margin-bottom 30px dan margin-top 20px menghasilkan jarak nyata 30px, bukan 50px.

**Source code utama:** [61_margin_collapse.css](61_margin_collapse.css)

**File pendukung preview:** [61_margin_collapse.html](61_margin_collapse.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "61_margin_collapse.html"
```

**Hasil yang Diharapkan:**
Visualisasi jarak vertikal antara dua kotak yang memperlihatkan peleburan margin menjadi 30px.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Margin collapsing](output/61_margin_collapse.png)

---

### 62. Properti padding

**Tujuan:** Mengatur ruang dalam (padding) pada elemen untuk memberikan ruang bernapas pada konten.

**Konsep Utama:**
Padding adalah ruang interior di antara konten teks/elemen anak dengan garis batas (border). Berbeda dengan margin, padding tidak pernah mengalami collapsing dan selalu memiliki latar belakang yang sama dengan elemen.

**Penjelasan Source Code:**
Mengatur padding kartu secara asimetris untuk menciptakan tata letak formulir masukan yang proporsional.

**Source code utama:** [62_padding_property.css](62_padding_property.css)

**File pendukung preview:** [62_padding_property.html](62_padding_property.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "62_padding_property.html"
```

**Hasil yang Diharapkan:**
Kotak kartu dengan ruang dalam yang nyaman dan teks yang tidak menabrak batas tepi kotak.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti padding](output/62_padding_property.png)

---

### 63. Pemusatan menggunakan margin: auto

**Tujuan:** Memposisikan elemen blok tepat di tengah secara horizontal menggunakan margin: auto.

**Konsep Utama:**
Ketika sebuah elemen blok memiliki lebar terdefinisi (`width` atau `max-width`), memberikan `margin-left: auto` dan `margin-right: auto` akan membagi sisa ruang kosong secara seimbang di kedua sisi, menempatkan elemen tepat di tengah wadah.

**Penjelasan Source Code:**
Elemen `.centered-modal` dengan lebar 420px dan `margin: 40px auto` diposisikan secara otomatis di tengah jendela browser.

**Source code utama:** [63_margin_auto.css](63_margin_auto.css)

**File pendukung preview:** [63_margin_auto.html](63_margin_auto.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "63_margin_auto.html"
```

**Hasil yang Diharapkan:**
Kotak modal yang berada presisi di tengah layar secara horizontal.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Pemusatan menggunakan margin: auto](output/63_margin_auto.png)

---

### 64. Logical margin properties

**Tujuan:** Menerapkan margin berbasis arah aliran penulisan (margin-inline dan margin-block).

**Konsep Utama:**
CSS Logical Properties menggantikan arah fisik (top, bottom, left, right) dengan istilah berbasis alur teks: `margin-block` (sumbu vertikal pada bahasa LTR) dan `margin-inline` (sumbu horizontal). Mendukung multibahasa LTR dan RTL secara mulus.

**Penjelasan Source Code:**
Mengatur `margin-block: 20px` dan `margin-inline: auto` sebagai alternatif modern dari margin 2 nilai.

**Source code utama:** [64_logical_margin.css](64_logical_margin.css)

**File pendukung preview:** [64_logical_margin.html](64_logical_margin.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "64_logical_margin.html"
```

**Hasil yang Diharapkan:**
Kotak yang terpusat dan berjarak vertikal teratur menggunakan logical margin properties.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Logical margin properties](output/64_logical_margin.png)

---

### 65. Logical padding properties

**Tujuan:** Mengatur ruang dalam menggunakan padding-inline dan padding-block.

**Konsep Utama:**
Serupa dengan margin, `padding-block` mengatur ruang dalam pada sumbu atas-bawah aliran konten, sedangkan `padding-inline` mengatur ruang dalam pada sumbu kiri-kanan.

**Penjelasan Source Code:**
Menerapkan `padding-block: 12px` dan `padding-inline: 24px` pada tombol navigasi lencana.

**Source code utama:** [65_logical_padding.css](65_logical_padding.css)

**File pendukung preview:** [65_logical_padding.html](65_logical_padding.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "65_logical_padding.html"
```

**Hasil yang Diharapkan:**
Lencana tombol modern dengan proporsi padding logis yang seimbang.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Logical padding properties](output/65_logical_padding.png)

---

### 66. Global box sizing

**Tujuan:** Menerapkan pola best practice industri untuk mereset seluruh elemen dokumen ke border-box.

**Konsep Utama:**
Pola industri standar yang dipelopori oleh Paul Irish menetapkan `box-sizing: border-box` pada `html`, kemudian membuat seluruh elemen dan pseudo-element mewarisinya (`box-sizing: inherit`). Ini memudahkan integrasi komponen pihak ketiga.

**Penjelasan Source Code:**
Menetapkan aturan `html { box-sizing: border-box; }` dan `*, *::before, *::after { box-sizing: inherit; }`.

**Source code utama:** [66_box_sizing_global.css](66_box_sizing_global.css)

**File pendukung preview:** [66_box_sizing_global.html](66_box_sizing_global.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "66_box_sizing_global.html"
```

**Hasil yang Diharapkan:**
Struktur dua kolom yang berdampingan secara sempurna tanpa pecah ke baris baru.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Global box sizing](output/66_box_sizing_global.png)

---

### 67. Intrinsic sizing

**Tujuan:** Memahami konsep intrinsic sizing (ukuran berbasis konten alami) vs extrinsic sizing (ukuran yang dipaksakan).

**Konsep Utama:**
Extrinsic sizing menetapkan ukuran pasti dari luar (misal width: 400px), sedangkan Intrinsic sizing membiarkan peramban menghitung dimensi berdasarkan isi konten internalnya sendiri.

**Penjelasan Source Code:**
Membandingkan wadah extrinsic yang membatasi teks secara paksa dengan wadah intrinsic yang membalut teks secara pas.

**Source code utama:** [67_intrinsic_sizing.css](67_intrinsic_sizing.css)

**File pendukung preview:** [67_intrinsic_sizing.html](67_intrinsic_sizing.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "67_intrinsic_sizing.html"
```

**Hasil yang Diharapkan:**
Dua kotak perbandingan yang memperlihatkan perbedaan dimensi pas konten vs dimensi kaku.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Intrinsic sizing](output/67_intrinsic_sizing.png)

---

### 68. min-content dan max-content

**Tujuan:** Membedakan kata kunci ukuran min-content dan max-content.

**Konsep Utama:**
`min-content` menyusutkan kotak sekecil mungkin tanpa menyebabkan kata terpotong (lebarnya sama dengan kata terpanjang di dalamnya). `max-content` melebarkan kotak sebesar mungkin tanpa memecah baris (tanpa soft-wrap).

**Penjelasan Source Code:**
Mendemonstrasikan teks yang sama dalam dua kotak dengan `width: min-content` dan `width: max-content`.

**Source code utama:** [68_min_content_max_content.css](68_min_content_max_content.css)

**File pendukung preview:** [68_min_content_max_content.html](68_min_content_max_content.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "68_min_content_max_content.html"
```

**Hasil yang Diharapkan:**
Kotak pertama menyusut setara satu kata terpanjang, sedangkan kotak kedua memanjang satu baris utuh.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi min-content dan max-content](output/68_min_content_max_content.png)

---

### 69. Fungsi fit-content()

**Tujuan:** Menggunakan fit-content() untuk menggabungkan elastisitas max-content dengan batasan ruang.

**Konsep Utama:**
Fungsi `fit-content(limit)` menggunakan ukuran alami konten (seperti `max-content`), namun jika ukuran konten melebihi batas argumen yang diberikan, lebarnya akan ditahan pada batas tersebut.

**Penjelasan Source Code:**
Menata kotak paragraf dengan `width: fit-content(380px)`.

**Source code utama:** [69_fit_content.css](69_fit_content.css)

**File pendukung preview:** [69_fit_content.html](69_fit_content.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "69_fit_content.html"
```

**Hasil yang Diharapkan:**
Kotak yang membalut teks dengan rapi namun tidak pernah melampaui lebar 380px.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi fit-content()](output/69_fit_content.png)

---

### 70. Properti aspect-ratio

**Tujuan:** Menjaga proporsi rasio aspek elemen (misal 16/9 atau 1/1) secara otomatis ketika lebar berubah.

**Konsep Utama:**
Properti `aspect-ratio` menetapkan rasio lebar terhadap tinggi yang diinginkan untuk kotak elemen. Saat lebar berubah (misal responsif), tinggi elemen akan dihitung otomatis oleh browser tanpa trik padding-top lawas.

**Penjelasan Source Code:**
Membuat kotak pemutar video berasio `aspect-ratio: 16 / 9` dan thumbnail kartu berasio `aspect-ratio: 1 / 1`.

**Source code utama:** [70_aspect_ratio.css](70_aspect_ratio.css)

**File pendukung preview:** [70_aspect_ratio.html](70_aspect_ratio.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "70_aspect_ratio.html"
```

**Hasil yang Diharapkan:**
Dua wadah responsif yang mempertahankan rasio 16:9 dan persegi 1:1 secara sempurna.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti aspect-ratio](output/70_aspect_ratio.png)

---

## Ringkasan Modul

Box model adalah fondasi perhitungan geometri setiap elemen di peramban web. Penguasaan box model, terutama border-box dan intrinsic sizing, menjadi prasyarat mutlak sebelum mempelajari teknik tata letak modern seperti Flexbox dan CSS Grid pada modul-modul mendatang.

### Keterkaitan Materi
Seluruh submodul dalam modul ini dirancang secara berjenjang untuk membangun pemahaman yang kokoh dan aplikatif. Lanjutkan ke modul berikutnya setelah menguasai seluruh konsep di atas.
