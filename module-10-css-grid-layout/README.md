# Modul 10: CSS Grid Layout

## Ringkasan Ruang Lingkup Materi

Modul ini mengeksplorasi sistem tata letak 2-dimensi paling mutakhir dalam CSS: CSS Grid Layout. Materi mencakup konsep garis kisi (grid lines) dan lintasan (tracks), deklarasi display: grid, perancangan kolom grid-template-columns dan baris grid-template-rows, penamaan area visual grid-template-areas, perentangan sel dengan grid-column dan grid-row (span), properti grid-area, pengaturan spasi gap, alur otomatis grid-auto-flow (row, column, dense), lintasan implisit grid-auto-columns/rows, auto-fit vs auto-fill, fungsi minmax(), fungsi repeat(), satuan fraksional (fr), perataan sel (justify-items, align-items), hingga pembangunan layout kartu galeri dan dashboard analitik interaktif.

## Tujuan Pembelajaran Modul

- Memahami arsitektur tata letak dua dimensi (baris dan kolom simultan) pada CSS Grid.
- Mendefinisikan kolom dan baris eksplisit menggunakan satuan piksel, persen, dan fractional unit (fr).
- Menyusun tata letak halaman deklaratif berbasis nama area menggunakan grid-template-areas.
- Mengontrol perentangan sel melintasi banyak kolom dan baris dengan grid-column dan grid-row span.
- Membangun grid yang sepenuhnya responsif tanpa media queries menggunakan auto-fit dan minmax().
- Merancang layout dashboard kompleks dengan header, sidebar, konten kartu, dan panel metrik.

## Daftar Submodul

- [166. Pengenalan CSS Grid](166_grid_basic.css) — [Halaman Preview](166_grid_basic.html)
- [167. display: grid](167_display_grid.css) — [Halaman Preview](167_display_grid.html)
- [168. grid-template-columns](168_grid_template_columns.css) — [Halaman Preview](168_grid_template_columns.html)
- [169. grid-template-rows](169_grid_template_rows.css) — [Halaman Preview](169_grid_template_rows.html)
- [170. grid-template-areas](170_grid_template_areas.css) — [Halaman Preview](170_grid_template_areas.html)
- [171. grid-column](171_grid_column.css) — [Halaman Preview](171_grid_column.html)
- [172. grid-row](172_grid_row.css) — [Halaman Preview](172_grid_row.html)
- [173. Properti grid-area](173_grid_area.css) — [Halaman Preview](173_grid_area.html)
- [174. gap pada Grid](174_grid_gap.css) — [Halaman Preview](174_grid_gap.html)
- [175. grid-auto-flow](175_grid_auto_flow.css) — [Halaman Preview](175_grid_auto_flow.html)
- [176. grid-auto-columns dan grid-auto-rows](176_grid_auto_columns_rows.css) — [Halaman Preview](176_grid_auto_columns_rows.html)
- [177. auto-fit](177_grid_auto_fit.css) — [Halaman Preview](177_grid_auto_fit.html)
- [178. auto-fill](178_grid_auto_fill.css) — [Halaman Preview](178_grid_auto_fill.html)
- [179. Fungsi minmax()](179_minmax_function.css) — [Halaman Preview](179_minmax_function.html)
- [180. Fungsi repeat()](180_repeat_function.css) — [Halaman Preview](180_repeat_function.html)
- [181. Unit fr](181_fractional_units.css) — [Halaman Preview](181_fractional_units.html)
- [182. justify-items](182_justify_items_grid.css) — [Halaman Preview](182_justify_items_grid.html)
- [183. align-items pada Grid](183_align_items_grid.css) — [Halaman Preview](183_align_items_grid.html)
- [184. Card layout dengan Grid](184_grid_card_layout.css) — [Halaman Preview](184_grid_card_layout.html)
- [185. Dashboard dengan Grid](185_grid_dashboard_layout.css) — [Halaman Preview](185_grid_dashboard_layout.html)

---

## Pembahasan dan Penjelasan Submodul

### 166. Pengenalan CSS Grid

**Tujuan:** Memahami konsep sistem kisi dua dimensi (baris dan kolom bersamaan).

**Konsep Utama:**
CSS Grid Layout adalah sistem tata letak 2-dimensi pertama yang dirancang khusus untuk web. Grid membagi kontainer menjadi baris dan kolom yang berpotongan membentuk sel-sel kisi.

**Penjelasan Source Code:**
Mengatur kontainer dasar dengan 3 kolom dan 2 baris sel yang tertata rapi.

**Source code utama:** [166_grid_basic.css](166_grid_basic.css)

**File pendukung preview:** [166_grid_basic.html](166_grid_basic.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "166_grid_basic.html"
```

**Hasil yang Diharapkan:**
Kisi kotak 2x3 yang tersusun simetris dan rapi.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Pengenalan CSS Grid](output/166_grid_basic.png)

---

### 167. display: grid

**Tujuan:** Mengaktifkan konteks pemformatan grid pada kontainer induk.

**Konsep Utama:**
Deklarasi `display: grid` menetapkan elemen sebagai grid container tingkat blok. Semua elemen anak langsungnya otomatis menjadi grid items yang dapat diposisikan pada koordinat kisi.

**Penjelasan Source Code:**
Menampilkan dua kolom simetris menggunakan `display: grid`.

**Source code utama:** [167_display_grid.css](167_display_grid.css)

**File pendukung preview:** [167_display_grid.html](167_display_grid.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "167_display_grid.html"
```

**Hasil yang Diharapkan:**
Dua panel sisi yang berjajar simetris dalam konteks grid.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi display: grid](output/167_display_grid.png)

---

### 168. grid-template-columns

**Tujuan:** Mendefinisikan jumlah dan ukuran kolom eksplisit pada grid.

**Konsep Utama:**
Properti `grid-template-columns` menentukan lebar setiap kolom kisi. Menerima deretan nilai ukuran yang dipisahkan spasi (misal: `150px 1fr 2fr`).

**Penjelasan Source Code:**
Membuat layout 3 kolom: sidebar kiri tetap 140px, konten tengah fleksibel 2fr, dan panel kanan 1fr.

**Source code utama:** [168_grid_template_columns.css](168_grid_template_columns.css)

**File pendukung preview:** [168_grid_template_columns.html](168_grid_template_columns.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "168_grid_template_columns.html"
```

**Hasil yang Diharapkan:**
Tiga kolom dengan proporsi asimetris yang tertata rapi.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi grid-template-columns](output/168_grid_template_columns.png)

---

### 169. grid-template-rows

**Tujuan:** Mendefinisikan tinggi baris eksplisit pada tata letak grid.

**Konsep Utama:**
Properti `grid-template-rows` menetapkan ketinggian masing-masing baris kisi dalam grid eksplisit.

**Penjelasan Source Code:**
Mengatur baris header setinggi 50px dan baris isi setinggi 100px.

**Source code utama:** [169_grid_template_rows.css](169_grid_template_rows.css)

**File pendukung preview:** [169_grid_template_rows.html](169_grid_template_rows.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "169_grid_template_rows.html"
```

**Hasil yang Diharapkan:**
Kisi dengan baris pertama kompak dan baris kedua lapang.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi grid-template-rows](output/169_grid_template_rows.png)

---

### 170. grid-template-areas

**Tujuan:** Menyusun tata letak halaman secara visual menggunakan nama area deklaratif.

**Konsep Utama:**
Properti `grid-template-areas` memungkinkan penyusunan tata letak menggunakan representasi grafis berupa string nama area (seperti `'header header' 'sidebar main' 'footer footer'`).

**Penjelasan Source Code:**
Membangun layout website klasik dengan header, sidebar, konten utama, dan footer menggunakan nama area.

**Source code utama:** [170_grid_template_areas.css](170_grid_template_areas.css)

**File pendukung preview:** [170_grid_template_areas.html](170_grid_template_areas.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "170_grid_template_areas.html"
```

**Hasil yang Diharapkan:**
Struktur layout halaman web lengkap yang diposisikan deklaratif melalui grid areas.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi grid-template-areas](output/170_grid_template_areas.png)

---

### 171. grid-column

**Tujuan:** Merentangkan elemen melintasi beberapa kolom menggunakan garis kisi atau span.

**Konsep Utama:**
Shorthand `grid-column: [start] / [end]` atau `grid-column: span [jumlah]` memungkinkan satu item melebar melintasi dua atau lebih kolom kisi.

**Penjelasan Source Code:**
Membuat elemen banner fitur yang merentang selebar 2 kolom penuh di atas dua kartu biasa.

**Source code utama:** [171_grid_column.css](171_grid_column.css)

**File pendukung preview:** [171_grid_column.html](171_grid_column.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "171_grid_column.html"
```

**Hasil yang Diharapkan:**
Banner atas yang melebar memenuhi 2 kolom, diikuti dua kolom sejajar di bawahnya.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi grid-column](output/171_grid_column.png)

---

### 172. grid-row

**Tujuan:** Merentangkan elemen melintasi beberapa baris menggunakan garis kisi vertikal atau span.

**Konsep Utama:**
Shorthand `grid-row: [start] / [end]` atau `grid-row: span [jumlah]` memungkinkan satu item merentang tinggi melintasi dua atau lebih baris secara vertikal.

**Penjelasan Source Code:**
Membuat panel fitur utama yang merentang setinggi 2 baris berdampingan dengan 2 kartu kecil.

**Source code utama:** [172_grid_row.css](172_grid_row.css)

**File pendukung preview:** [172_grid_row.html](172_grid_row.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "172_grid_row.html"
```

**Hasil yang Diharapkan:**
Satu panel tinggi di sisi kiri dan dua panel bertumpuk di sisi kanan.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi grid-row](output/172_grid_row.png)

---

### 173. Properti grid-area

**Tujuan:** Menghubungkan item ke nama area atau menetapkan 4 garis koordinat sekaligus.

**Konsep Utama:**
Properti `grid-area` dapat menetapkan nama area (seperti `grid-area: header`) atau bertindak sebagai shorthand numerik untuk `row-start / column-start / row-end / column-end`.

**Penjelasan Source Code:**
Menempatkan widget metrik pada area tertentu menggunakan nama `grid-area`.

**Source code utama:** [173_grid_area.css](173_grid_area.css)

**File pendukung preview:** [173_grid_area.html](173_grid_area.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "173_grid_area.html"
```

**Hasil yang Diharapkan:**
Widget analitik yang menempati lokasi koordinat grid yang presisi.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Properti grid-area](output/173_grid_area.png)

---

### 174. gap pada Grid

**Tujuan:** Mengatur jarak celah antar-kolom dan antar-baris pada grid menggunakan properti gap.

**Konsep Utama:**
Properti `gap: [row-gap] [column-gap]` mengatur celah teratur di antara baris dan kolom kisi secara elegan tanpa memerlukan margin.

**Penjelasan Source Code:**
Mengatur `gap: 20px 10px` (jarak baris 20px, jarak kolom 10px) pada matriks tombol.

**Source code utama:** [174_grid_gap.css](174_grid_gap.css)

**File pendukung preview:** [174_grid_gap.html](174_grid_gap.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "174_grid_gap.html"
```

**Hasil yang Diharapkan:**
Matriks 4 kotak dengan jarak vertikal lebih lebar daripada jarak horizontal.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi gap pada Grid](output/174_grid_gap.png)

---

### 175. grid-auto-flow

**Tujuan:** Mengatur alur penempatan otomatis item kisi (row, column, dense).

**Konsep Utama:**
Properti `grid-auto-flow` mengontrol bagaimana item baru yang tidak ditentukan posisinya dimasukkan ke dalam kisi: mengisi per baris (`row` - default) atau mengisi per kolom (`column`), serta opsi `dense` untuk mengisi lubang kosong.

**Penjelasan Source Code:**
Mengatur `grid-auto-flow: column` sehingga item mengalir mengisi kolom ke bawah terlebih dahulu.

**Source code utama:** [175_grid_auto_flow.css](175_grid_auto_flow.css)

**File pendukung preview:** [175_grid_auto_flow.html](175_grid_auto_flow.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "175_grid_auto_flow.html"
```

**Hasil yang Diharapkan:**
Kotak-kotak bernomor yang tersusun mengalir ke bawah sebelum berpindah ke kolom samping.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi grid-auto-flow](output/175_grid_auto_flow.png)

---

### 176. grid-auto-columns dan grid-auto-rows

**Tujuan:** Menentukan ukuran lintasan implisit yang terbentuk otomatis saat item melampaui grid eksplisit.

**Konsep Utama:**
Ketika ada lebih banyak item daripada baris/kolom yang didefinisikan di template, peramban menciptakan lintasan implisit (implicit tracks). Ukuran lintasan implisit ini diatur oleh `grid-auto-rows` dan `grid-auto-columns`.

**Penjelasan Source Code:**
Menetapkan `grid-auto-rows: 75px` sehingga setiap baris tambahan otomatis memiliki tinggi seragam 75px.

**Source code utama:** [176_grid_auto_columns_rows.css](176_grid_auto_columns_rows.css)

**File pendukung preview:** [176_grid_auto_columns_rows.html](176_grid_auto_columns_rows.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "176_grid_auto_columns_rows.html"
```

**Hasil yang Diharapkan:**
Kotak-kotak item implisit yang semuanya memiliki ketinggian seragam 75px secara teratur.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi grid-auto-columns dan grid-auto-rows](output/176_grid_auto_columns_rows.png)

---

### 177. auto-fit

**Tujuan:** Membangun layout grid responsif mandiri di mana kolom meregang memenuhi ruang kosong.

**Konsep Utama:**
`auto-fit` pada `repeat(auto-fit, minmax(...))` memasukkan sebanyak mungkin kolom ke dalam kontainer, dan jika item lebih sedikit dari kapasitas kolom, kolom yang ada akan meregang merebut sisa ruang kosong.

**Penjelasan Source Code:**
Menerapkan pola sakti `repeat(auto-fit, minmax(140px, 1fr))` untuk kartu produk otomatis responsif.

**Source code utama:** [177_grid_auto_fit.css](177_grid_auto_fit.css)

**File pendukung preview:** [177_grid_auto_fit.html](177_grid_auto_fit.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "177_grid_auto_fit.html"
```

**Hasil yang Diharapkan:**
Deretan kartu yang fleksibel membagi ruang penuh secara mandiri tanpa media query.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi auto-fit](output/177_grid_auto_fit.png)

---

### 178. auto-fill

**Tujuan:** Mempertahankan slot kolom kosong meskipun tidak ada item untuk mengisinya.

**Konsep Utama:**
Berbeda dengan `auto-fit`, kata kunci `auto-fill` akan tetap membuat slot lintasan kolom kosong di sisi kanan kontainer jika masih ada sisa ruang, tanpa meregangkan item yang ada.

**Penjelasan Source Code:**
Mendemonstrasikan perbedaan auto-fill di mana item tetap pada ukuran minmax tanpa dipaksa melebar.

**Source code utama:** [178_grid_auto_fill.css](178_grid_auto_fill.css)

**File pendukung preview:** [178_grid_auto_fill.html](178_grid_auto_fill.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "178_grid_auto_fill.html"
```

**Hasil yang Diharapkan:**
Dua kartu berukuran tetap dengan ruang slot kolom kosong yang disisakan di sisi kanan.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi auto-fill](output/178_grid_auto_fill.png)

---

### 179. Fungsi minmax()

**Tujuan:** Menetapkan rentang ukuran minimum dan maksimum yang fleksibel pada lintasan grid.

**Konsep Utama:**
Fungsi `minmax(min, max)` membatasi ukuran kolom agar tidak pernah lebih kecil dari batas `min` dan tidak pernah melebihi batas `max`.

**Penjelasan Source Code:**
Mengatur kolom sidebar dengan `minmax(120px, 200px)` yang elastis namun memiliki batas keamanan.

**Source code utama:** [179_minmax_function.css](179_minmax_function.css)

**File pendukung preview:** [179_minmax_function.html](179_minmax_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "179_minmax_function.html"
```

**Hasil yang Diharapkan:**
Sidebar yang fleksibel di dalam rentang aman 120px hingga 200px.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi minmax()](output/179_minmax_function.png)

---

### 180. Fungsi repeat()

**Tujuan:** Menghindari repetisi penulisan ukuran kolom dengan notasi ringkas repeat().

**Konsep Utama:**
Fungsi `repeat(jumlah, ukuran)` menyederhanakan penulisan pola berulang. Contoh: `repeat(4, 1fr)` setara dengan menulis `1fr 1fr 1fr 1fr`.

**Penjelasan Source Code:**
Mendefinisikan 4 kolom identik menggunakan `repeat(4, 1fr)`.

**Source code utama:** [180_repeat_function.css](180_repeat_function.css)

**File pendukung preview:** [180_repeat_function.html](180_repeat_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "180_repeat_function.html"
```

**Hasil yang Diharapkan:**
Empat kolom berjarak seragam dengan lebar yang terbagi persis 25% masing-masing.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi repeat()](output/180_repeat_function.png)

---

### 181. Unit fr

**Tujuan:** Menggunakan satuan fraksional (fr) untuk membagi sisa ruang secara proporsional.

**Konsep Utama:**
Satuan `fr` (fraction) merepresentasikan pecahan dari sisa ruang bebas di dalam grid container setelah semua ukuran tetap (seperti piksel dan celah gap) dialokasikan.

**Penjelasan Source Code:**
Membagi wadah menjadi perbandingan 1fr : 3fr.

**Source code utama:** [181_fractional_units.css](181_fractional_units.css)

**File pendukung preview:** [181_fractional_units.html](181_fractional_units.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "181_fractional_units.html"
```

**Hasil yang Diharapkan:**
Dua kolom di mana kolom kanan memiliki lebar tepat tiga kali lipat kolom kiri.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Unit fr](output/181_fractional_units.png)

---

### 182. justify-items

**Tujuan:** Mengatur perataan horizontal seluruh item di dalam sel masing-masing (start, center, end, stretch).

**Konsep Utama:**
Properti `justify-items` diterapkan pada kontainer grid untuk mengatur perataan seluruh item pada sumbu inline (horizontal) di dalam area selnya masing-masing.

**Penjelasan Source Code:**
Mengatur `justify-items: center` agar tombol-tombol berada di tengah sel tanpa meregang penuh.

**Source code utama:** [182_justify_items_grid.css](182_justify_items_grid.css)

**File pendukung preview:** [182_justify_items_grid.html](182_justify_items_grid.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "182_justify_items_grid.html"
```

**Hasil yang Diharapkan:**
Deretan tombol yang berposisi rapi di tengah sel kolom masing-masing.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi justify-items](output/182_justify_items_grid.png)

---

### 183. align-items pada Grid

**Tujuan:** Mengatur perataan vertikal seluruh item di dalam sel masing-masing pada sumbu blok.

**Konsep Utama:**
Properti `align-items` pada grid mengontrol posisi vertikal item di dalam sel: `stretch` (default: tinggi penuh), `center` (tengah vertikal), `start` (pucuk atas), dan `end` (dasar bawah).

**Penjelasan Source Code:**
Menata sel-sel grid dengan tinggi 100px dan `align-items: center`.

**Source code utama:** [183_align_items_grid.css](183_align_items_grid.css)

**File pendukung preview:** [183_align_items_grid.html](183_align_items_grid.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "183_align_items_grid.html"
```

**Hasil yang Diharapkan:**
Konten di dalam setiap sel kisi mengambang pas di tengah ketinggian sel.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi align-items pada Grid](output/183_align_items_grid.png)

---

### 184. Card layout dengan Grid

**Tujuan:** Membangun tata letak kartu produk responsif mandiri yang adaptif dengan CSS Grid.

**Konsep Utama:**
Kombinasi `grid-template-columns: repeat(auto-fill, minmax(200px, 1fr))` menghasilkan galeri kartu responsif yang secara otomatis mengatur jumlah kolom tanpa memerlukan media queries.

**Penjelasan Source Code:**
Menampilkan 3 kartu kursus dengan thumbnail, judul, dan badge harga yang tersusun dalam grid adaptif.

**Source code utama:** [184_grid_card_layout.css](184_grid_card_layout.css)

**File pendukung preview:** [184_grid_card_layout.html](184_grid_card_layout.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "184_grid_card_layout.html"
```

**Hasil yang Diharapkan:**
Galeri tiga kartu produk berpenampilan profesional dan sejajar rapi.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Card layout dengan Grid](output/184_grid_card_layout.png)

---

### 185. Dashboard dengan Grid

**Tujuan:** Merancang tata letak antarmuka dasbor analitik lengkap menggunakan CSS Grid.

**Konsep Utama:**
CSS Grid adalah fondasi terbaik untuk dashboard analitik: menyatukan widget ringkasan metrik, grafik lebar, dan daftar aktivitas dalam satu struktur terpadu yang konsisten.

**Penjelasan Source Code:**
Membangun dashboard dengan 2 kartu metrik kecil dan 1 panel grafik utama yang membentang 2 kolom di bawahnya.

**Source code utama:** [185_grid_dashboard_layout.css](185_grid_dashboard_layout.css)

**File pendukung preview:** [185_grid_dashboard_layout.html](185_grid_dashboard_layout.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "185_grid_dashboard_layout.html"
```

**Hasil yang Diharapkan:**
Layout dasbor analitik profesional dengan kartu metrik dan panel grafik.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Dashboard dengan Grid](output/185_grid_dashboard_layout.png)

---

## Ringkasan Modul

Jika Flexbox unggul pada penataan komponen 1-dimensi, CSS Grid adalah penguasa mutlak tata letak makro 2-dimensi. Dengan menyelesaikan Modul 10, pembelajar menguasai instrumen layout paling canggih yang ditawarkan oleh web modern.

### Keterkaitan Materi
Seluruh submodul dalam modul ini dirancang secara berjenjang untuk membangun pemahaman yang kokoh dan aplikatif. Lanjutkan ke modul berikutnya setelah menguasai seluruh konsep di atas.
