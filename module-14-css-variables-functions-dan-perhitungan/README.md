# Modul 14: CSS Variables, Functions, dan Perhitungan

## Ringkasan Ruang Lingkup Materi

Modul ini membahas kapabilitas pemrograman deklaratif dalam CSS modern: CSS Custom Properties (variabel CSS), aturan deklarasi dengan prefiks ganda (--nama), lingkup cakupan (scope global :root vs scope lokal komponen), pemanggilan var() beserta nilai fallback cadangannya, fungsi kalkulasi matematis dinamis calc() yang mencampur berbagai unit (100% - 40px), fungsi batas min(), max(), dan rentang clamp(), fungsi manipulasi warna mutakhir color-mix() dan relative color syntax, fungsi otomatis adaptasi tema light-dark(), sistem penomoran otomatis CSS Counters (counter-reset, counter-increment, fungsi counter() dan counters()), serta arsitektur Design Tokens, sistem spacing modular, dan variabel tema aplikasi (Theming).

## Tujuan Pembelajaran Modul

- Mendefinisikan dan mengonsumsi variabel kustom CSS (--var-name) menggunakan fungsi var().
- Mengelola hierarki scope variabel global pada :root dan override scope lokal pada sub-komponen.
- Melakukan kalkulasi dimensi dinamis dengan calc(), min(), max(), dan clamp().
- Memanfaatkan fitur warna modern W3C: color-mix() dan fungsi light-dark().
- Membuat sistem penomoran bab dan daftar hierarkis otomatis dengan CSS Counters.
- Menyusun arsitektur Design Tokens terstruktur untuk tema terang/gelap (Theming System).

## Daftar Submodul

- [246. CSS custom properties](246_css_custom_properties.css) — [Halaman Preview](246_css_custom_properties.html)
- [247. Deklarasi variabel CSS](247_css_variable_declaration.css) — [Halaman Preview](247_css_variable_declaration.html)
- [248. Scope variabel CSS](248_css_variable_scope.css) — [Halaman Preview](248_css_variable_scope.html)
- [249. Variabel pada :root](249_root_selector_variables.css) — [Halaman Preview](249_root_selector_variables.html)
- [250. Fungsi var()](250_var_function.css) — [Halaman Preview](250_var_function.html)
- [251. Fungsi calc()](251_calc_function.css) — [Halaman Preview](251_calc_function.html)
- [252. Fungsi min()](252_min_function.css) — [Halaman Preview](252_min_function.html)
- [253. Fungsi max()](253_max_function.css) — [Halaman Preview](253_max_function.html)
- [254. Fungsi clamp()](254_clamp_function.css) — [Halaman Preview](254_clamp_function.html)
- [255. Fungsi color-mix()](255_color_mix_function.css) — [Halaman Preview](255_color_mix_function.html)
- [256. Relative color syntax](256_relative_color_syntax.css) — [Halaman Preview](256_relative_color_syntax.html)
- [257. Fungsi light-dark()](257_light_dark_function.css) — [Halaman Preview](257_light_dark_function.html)
- [258. CSS counters](258_css_counters.css) — [Halaman Preview](258_css_counters.html)
- [259. counter-reset dan counter-increment](259_counter_reset_increment.css) — [Halaman Preview](259_counter_reset_increment.html)
- [260. Fungsi counter() dan counters()](260_counter_function.css) — [Halaman Preview](260_counter_function.html)
- [261. Fallback variabel CSS](261_custom_property_fallback.css) — [Halaman Preview](261_custom_property_fallback.html)
- [262. Design tokens dengan CSS variables](262_design_tokens.css) — [Halaman Preview](262_design_tokens.html)
- [263. Sistem spacing dinamis](263_dynamic_spacing_system.css) — [Halaman Preview](263_dynamic_spacing_system.html)
- [264. Sistem warna dinamis](264_dynamic_color_system.css) — [Halaman Preview](264_dynamic_color_system.html)
- [265. Variabel tema aplikasi](265_theme_variables.css) — [Halaman Preview](265_theme_variables.html)

---

## Pembahasan dan Penjelasan Submodul

### 246. CSS custom properties

**Tujuan:** Memahami konsep dan sintaks dasar CSS Custom Properties (Variabel CSS).

**Konsep Utama:**
CSS Custom Properties diawali dengan dua tanda minus (`--nama-variabel`). Berbeda dengan variabel preprocessor (Sass), CSS variables bersifat dinamis di browser dan dapat dibaca serta dimanipulasi secara real-time.

**Penjelasan Source Code:**
Mendefinisikan variabel warna primer dan menggunakannya pada judul serta tombol kartu.

**Source code utama:** [246_css_custom_properties.css](246_css_custom_properties.css)

**File pendukung preview:** [246_css_custom_properties.html](246_css_custom_properties.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "246_css_custom_properties.html"
```

**Hasil yang Diharapkan:**
Kotak komponen kartu yang menggunakan variabel warna terpusat.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi CSS custom properties](output/246_css_custom_properties.png)

---

### 247. Deklarasi variabel CSS

**Tujuan:** Mendeklarasikan variabel CSS dengan berbagai tipe nilai: warna, ukuran, string, dan waktu.

**Konsep Utama:**
Variabel CSS dapat menampung tipe nilai apa pun yang valid dalam CSS: warna HEX/RGB, ukuran piksel/rem, durasi waktu transisi, hingga string font.

**Penjelasan Source Code:**
Mendeklarasikan koleksi variabel untuk radius sudut, padding, dan warna kartu.

**Source code utama:** [247_css_variable_declaration.css](247_css_variable_declaration.css)

**File pendukung preview:** [247_css_variable_declaration.html](247_css_variable_declaration.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "247_css_variable_declaration.html"
```

**Hasil yang Diharapkan:**
Komponen kartu styled yang seluruh dimensinya diatur melalui variabel kustom.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Deklarasi variabel CSS](output/247_css_variable_declaration.png)

---

### 248. Scope variabel CSS

**Tujuan:** Memahami konsep cakupan (scope) lokal vs pewarisan variabel CSS di DOM tree.

**Konsep Utama:**
Variabel CSS mengikuti hierarki DOM: jika didefinisikan pada komponen tertentu, variabel tersebut hanya dapat diakses oleh elemen tersebut dan keturunannya (Local Scope).

**Penjelasan Source Code:**
Menampilkan dua kartu dengan kelas berbeda yang menimpa nilai `--theme-color` secara lokal.

**Source code utama:** [248_css_variable_scope.css](248_css_variable_scope.css)

**File pendukung preview:** [248_css_variable_scope.html](248_css_variable_scope.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "248_css_variable_scope.html"
```

**Hasil yang Diharapkan:**
Dua kartu identik namun memiliki warna tema lokal berbeda (merah vs ungu).

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Scope variabel CSS](output/248_css_variable_scope.png)

---

### 249. Variabel pada :root

**Tujuan:** Mendefinisikan variabel CSS global pada pseudo-class :root.

**Konsep Utama:**
Pseudo-class `:root` merujuk pada elemen teratas dokumen HTML. Variabel yang dideklarasikan pada `:root` memiliki cakupan global (Global Scope) dan dapat diakses di mana saja di seluruh stylesheet.

**Penjelasan Source Code:**
Mendefinisikan variabel global di `:root` untuk warna merek dan font dokumen.

**Source code utama:** [249_root_selector_variables.css](249_root_selector_variables.css)

**File pendukung preview:** [249_root_selector_variables.html](249_root_selector_variables.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "249_root_selector_variables.html"
```

**Hasil yang Diharapkan:**
Komponen yang mengonsumsi variabel global root secara seragam.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Variabel pada :root](output/249_root_selector_variables.png)

---

### 250. Fungsi var()

**Tujuan:** Mengambil dan menerapkan nilai variabel menggunakan fungsi var().

**Konsep Utama:**
Fungsi `var(--nama-variabel)` menyisipkan nilai dari custom property ke dalam properti CSS apa pun.

**Penjelasan Source Code:**
Mengonsumsi variabel `--main-radius` dan `--main-bg` ke dalam tombol aksi modern.

**Source code utama:** [250_var_function.css](250_var_function.css)

**File pendukung preview:** [250_var_function.html](250_var_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "250_var_function.html"
```

**Hasil yang Diharapkan:**
Tombol aksi yang ditata secara elegan dengan pemanggilan fungsi var().

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi var()](output/250_var_function.png)

---

### 251. Fungsi calc()

**Tujuan:** Melakukan kalkulasi matematis dinamis (+, -, *, /) yang mencampur beragam unit CSS.

**Konsep Utama:**
Fungsi `calc()` memungkinkan perhitungan matematis yang mencampur berbagai unit tak sejenis, misalnya `width: calc(100% - 40px)`. Operator tambah (+) dan kurang (-) WAJIB diapit spasi.

**Penjelasan Source Code:**
Menghitung lebar kotak secara presisi: 100% lebar layar dikurangi 40px margin.

**Source code utama:** [251_calc_function.css](251_calc_function.css)

**File pendukung preview:** [251_calc_function.html](251_calc_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "251_calc_function.html"
```

**Hasil yang Diharapkan:**
Kotak yang presisi selebar kontainer dikurangi jarak 40px.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi calc()](output/251_calc_function.png)

---

### 252. Fungsi min()

**Tujuan:** Memilih nilai terkecil dari daftar ekspresi nilai menggunakan min().

**Konsep Utama:**
Fungsi `min(val1, val2, ...)` mengevaluasi argumen dan menerapkan nilai yang paling kecil. Misalnya `width: min(100%, 450px)` otomatis berfungsi seperti `max-width: 450px`.

**Penjelasan Source Code:**
Mengatur lebar kotak kartu dengan `width: min(90%, 460px)`.

**Source code utama:** [252_min_function.css](252_min_function.css)

**File pendukung preview:** [252_min_function.html](252_min_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "252_min_function.html"
```

**Hasil yang Diharapkan:**
Kotak responsif yang tidak pernah lebih lebar dari 460px.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi min()](output/252_min_function.png)

---

### 253. Fungsi max()

**Tujuan:** Menetapkan batas ukuran lantai minimum menggunakan fungsi max().

**Konsep Utama:**
Fungsi `max(val1, val2)` memilih nilai yang paling besar, bertindak sebagai pengaman batas bawah (lantai ukuran). Misalnya `height: max(100px, 15vh)`.

**Penjelasan Source Code:**
Membuat kotak dengan tinggi `height: max(120px, 20vw)`.

**Source code utama:** [253_max_function.css](253_max_function.css)

**File pendukung preview:** [253_max_function.html](253_max_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "253_max_function.html"
```

**Hasil yang Diharapkan:**
Kotak yang tingginya tidak pernah menyusut di bawah 120px.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi max()](output/253_max_function.png)

---

### 254. Fungsi clamp()

**Tujuan:** Mengunci nilai di dalam rentang minimum, nilai ideal dinamis, dan maksimum.

**Konsep Utama:**
Fungsi `clamp(min, preferred, max)` adalah perpaduan sempurna dari `min()` dan `max()`. Sangat populer untuk padding dan ukuran font fluida.

**Penjelasan Source Code:**
Menerapkan `padding: clamp(12px, 4vw, 32px)` yang fluida dan elastis.

**Source code utama:** [254_clamp_function.css](254_clamp_function.css)

**File pendukung preview:** [254_clamp_function.html](254_clamp_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "254_clamp_function.html"
```

**Hasil yang Diharapkan:**
Kotak kartu dengan ruang dalam (padding) yang beradaptasi secara fluida seirama ukuran layar.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi clamp()](output/254_clamp_function.png)

---

### 255. Fungsi color-mix()

**Tujuan:** Mencampurkan dua warna dalam ruang warna tertentu (in srgb) murni di CSS.

**Konsep Utama:**
Fungsi `color-mix(in srgb, warna1 persen, warna2)` mencampurkan dua warna secara dinamis langsung di peramban, memudahkan pembuatan variasi tint dan shade dari satu warna brand.

**Penjelasan Source Code:**
Mencampurkan 80% biru dengan 20% putih untuk membuat warna biru muda serasi.

**Source code utama:** [255_color_mix_function.css](255_color_mix_function.css)

**File pendukung preview:** [255_color_mix_function.html](255_color_mix_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "255_color_mix_function.html"
```

**Hasil yang Diharapkan:**
Kotak warna hasil pencampuran dinamis antara warna biru dan putih murni.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi color-mix()](output/255_color_mix_function.png)

---

### 256. Relative color syntax

**Tujuan:** Memodifikasi kanal warna yang sudah ada secara relatif (misal mengubah alpha atau lightness).

**Konsep Utama:**
Relative Color Syntax (CSS Color 5) memungkinkan pengambilan kanal warna dasar untuk dimodifikasi: `rgb(from #2563eb r g b / 0.5)` untuk menambahkan transparansi pada warna heksadesimal yang ada.

**Penjelasan Source Code:**
Mendemonstrasikan derivasi warna transparan relatif dari warna dasar yang ada.

**Source code utama:** [256_relative_color_syntax.css](256_relative_color_syntax.css)

**File pendukung preview:** [256_relative_color_syntax.html](256_relative_color_syntax.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "256_relative_color_syntax.html"
```

**Hasil yang Diharapkan:**
Kotak warna dengan transparansi turunan yang elegan.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Relative color syntax](output/256_relative_color_syntax.png)

---

### 257. Fungsi light-dark()

**Tujuan:** Menyediakan warna mode terang dan gelap dalam satu baris deklarasi menggunakan light-dark().

**Konsep Utama:**
Fungsi `light-dark(lightColor, darkColor)` otomatis memilih nilai pertama saat `color-scheme: light` dan nilai kedua saat `color-scheme: dark`, menyederhanakan kode dark mode secara radikal.

**Penjelasan Source Code:**
Menentukan warna latar dan teks yang otomatis adaptif menggunakan `light-dark()`.

**Source code utama:** [257_light_dark_function.css](257_light_dark_function.css)

**File pendukung preview:** [257_light_dark_function.html](257_light_dark_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "257_light_dark_function.html"
```

**Hasil yang Diharapkan:**
Komponen yang secara instan mendukung light dan dark theme tanpa blok media query duplikat.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi light-dark()](output/257_light_dark_function.png)

---

### 258. CSS counters

**Tujuan:** Memahami konsep pencacah otomatis (CSS Counters) untuk penomoran daftar dan subbab.

**Konsep Utama:**
CSS Counters adalah 'variabel angka' bawaan CSS yang nilainya dapat diinisialisasi (`counter-reset`) dan ditambah bertahap (`counter-increment`) untuk memberi nomor otomatis pada elemen.

**Penjelasan Source Code:**
Mengatur penomoran otomatis pada langkah-langkah panduan pengerjaan modul.

**Source code utama:** [258_css_counters.css](258_css_counters.css)

**File pendukung preview:** [258_css_counters.html](258_css_counters.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "258_css_counters.html"
```

**Hasil yang Diharapkan:**
Daftar bernomor otomatis yang dihitung murni menggunakan CSS counter.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi CSS counters](output/258_css_counters.png)

---

### 259. counter-reset dan counter-increment

**Tujuan:** Mengatur nilai awal dan besaran penambahan (step increment) pencacah.

**Konsep Utama:**
`counter-reset: nama [nilai_awal]` mengatur titik awal angka (default: 0). `counter-increment: nama [step]` menambah angka sebesar nilai step (bisa bertambah +1, +2, atau bahkan minus untuk hitung mundur).

**Penjelasan Source Code:**
Membuat hitungan bertingkat kelipatan 10 (step 10).

**Source code utama:** [259_counter_reset_increment.css](259_counter_reset_increment.css)

**File pendukung preview:** [259_counter_reset_increment.html](259_counter_reset_increment.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "259_counter_reset_increment.html"
```

**Hasil yang Diharapkan:**
Daftar bernomor dengan kenaikan bertahap 10, 20, 30.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi counter-reset dan counter-increment](output/259_counter_reset_increment.png)

---

### 260. Fungsi counter() dan counters()

**Tujuan:** Memformat gaya nomor (romawi/abjad) dan menyusun penomoran bersarang (1.1, 1.2) dengan counters().

**Konsep Utama:**
Fungsi `counter(nama, style)` dapat diformat menjadi romawi (`upper-roman`) atau abjad (`lower-alpha`). Fungsi `counters(nama, '.')` menyusun nomor bersarang hierarkis bertingkat secara otomatis.

**Penjelasan Source Code:**
Menampilkan daftar bersarang dengan penomoran bab 1.1, 1.2 menggunakan `counters()`.

**Source code utama:** [260_counter_function.css](260_counter_function.css)

**File pendukung preview:** [260_counter_function.html](260_counter_function.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "260_counter_function.html"
```

**Hasil yang Diharapkan:**
Daftar bersarang dengan nomor hierarki otomatis yang rapi.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fungsi counter() dan counters()](output/260_counter_function.png)

---

### 261. Fallback variabel CSS

**Tujuan:** Menyediakan nilai cadangan (fallback) pada var() jika variabel belum didefinisikan.

**Konsep Utama:**
Fungsi `var(--nama, fallbackValue)` menerima parameter kedua sebagai nilai cadangan. Jika `--nama` belum dideklarasikan atau tidak valid, browser akan otomatis memakai nilai fallback tersebut.

**Penjelasan Source Code:**
Mengonsumsi variabel yang belum ada dengan fallback aman warna oranye `#ea580c`.

**Source code utama:** [261_custom_property_fallback.css](261_custom_property_fallback.css)

**File pendukung preview:** [261_custom_property_fallback.html](261_custom_property_fallback.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "261_custom_property_fallback.html"
```

**Hasil yang Diharapkan:**
Elemen yang tetap tampil rapi dengan warna fallback cadangan.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fallback variabel CSS](output/261_custom_property_fallback.png)

---

### 262. Design tokens dengan CSS variables

**Tujuan:** Menyusun kamus Design Tokens (warna, radius, elevasi) untuk standarisasi proyek.

**Konsep Utama:**
Design Tokens adalah nilai-nilai desain atomik (seperti token warna, spasi, shadow) yang disimpan dalam variabel global untuk menjamin konsistensi di seluruh tim rekayasa perangkat lunak.

**Penjelasan Source Code:**
Membangun kartu dengan mengonsumsi token warna primer, token radius, dan token shadow.

**Source code utama:** [262_design_tokens.css](262_design_tokens.css)

**File pendukung preview:** [262_design_tokens.html](262_design_tokens.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "262_design_tokens.html"
```

**Hasil yang Diharapkan:**
Komponen kartu yang terstruktur rapi berdasarkan design tokens terpusat.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Design tokens dengan CSS variables](output/262_design_tokens.png)

---

### 263. Sistem spacing dinamis

**Tujuan:** Membangun skala kelipatan jarak spasi modular berbasis variabel CSS.

**Konsep Utama:**
Sistem spacing dinamis menetapkan unit dasar (misal `--space-base: 4px`) dan mengalikannya menjadi skala terprediksi (8px, 12px, 16px, 24px, 32px), menghapus angka acak pada margin dan padding.

**Penjelasan Source Code:**
Mengatur margin dan padding menggunakan skala kelipatan spasi modular.

**Source code utama:** [263_dynamic_spacing_system.css](263_dynamic_spacing_system.css)

**File pendukung preview:** [263_dynamic_spacing_system.html](263_dynamic_spacing_system.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "263_dynamic_spacing_system.html"
```

**Hasil yang Diharapkan:**
Wadah dengan ritme ruang vertikal dan horizontal yang sangat teratur.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Sistem spacing dinamis](output/263_dynamic_spacing_system.png)

---

### 264. Sistem warna dinamis

**Tujuan:** Membangun sistem palet warna bertingkat (50, 100, 500, 900) dengan variabel CSS.

**Konsep Utama:**
Sistem warna dinamis mendefinisikan skala warna bertingkat dari shade paling terang (50) hingga paling gelap (900) untuk setiap warna peran (primer, sekunder, sukses, bahaya).

**Penjelasan Source Code:**
Menampilkan kartu notifikasi yang memadukan shade 50 (latar), 500 (border), dan 900 (teks).

**Source code utama:** [264_dynamic_color_system.css](264_dynamic_color_system.css)

**File pendukung preview:** [264_dynamic_color_system.html](264_dynamic_color_system.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "264_dynamic_color_system.html"
```

**Hasil yang Diharapkan:**
Kotak notifikasi sukses dengan keharmonisan spektrum warna hijau dari satu keluarga token.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Sistem warna dinamis](output/264_dynamic_color_system.png)

---

### 265. Variabel tema aplikasi

**Tujuan:** Menerapkan arsitektur theming lengkap untuk penggantian tema aplikasi secara instan.

**Konsep Utama:**
Dengan mendefinisikan variabel semantik (`--bg-body`, `--text-main`, `--card-surface`), seluruh tema aplikasi (terang, gelap, atau tema korporat) dapat diganti hanya dengan menambahkan kelas tema pada tag `<body>` atau `<html>`.

**Penjelasan Source Code:**
Menampilkan tema gelap yang diaktifkan melalui atribut `data-theme='dark'` pada wadah.

**Source code utama:** [265_theme_variables.css](265_theme_variables.css)

**File pendukung preview:** [265_theme_variables.html](265_theme_variables.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "265_theme_variables.html"
```

**Hasil yang Diharapkan:**
Panel aplikasi berpenampilan tema gelap pekat dengan aksen biru safir.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Variabel tema aplikasi](output/265_theme_variables.png)

---

## Ringkasan Modul

CSS Custom Properties mengubah cara kita menulis stylesheet menjadi jauh lebih terstruktur, modular, dan dinamis. Dengan menyelesaikan Modul 14, pembelajar siap membangun sistem desain yang dapat diubah temanya hanya dengan mengganti beberapa baris variabel pada elemen root.

### Keterkaitan Materi
Seluruh submodul dalam modul ini dirancang secara berjenjang untuk membangun pemahaman yang kokoh dan aplikatif. Lanjutkan ke modul berikutnya setelah menguasai seluruh konsep di atas.
