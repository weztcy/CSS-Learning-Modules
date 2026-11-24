# Modul 11: Responsive Web Design

## Ringkasan Ruang Lingkup Materi

Modul ini membahas paradigma Desain Web Responsif (RWD) dari fondasi hingga teknologi terdepan: sintaks media queries dasar (@media), strategi breakpoint min-width (mobile-first) vs max-width (desktop-first), tipografi responsif dan tipografi fluida dinamis menggunakan fungsi clamp(), tata letak fluida persentase, penanganan gambar responsif (max-width: 100%), navigasi adaptif, integrasi Flexbox dan Grid responsif, deteksi orientasi perangkat (portrait/landscape), query kapabilitas interaksi pengguna (hover dan pointer: fine/coarse), dukungan tema gelap/terang otomatis (prefers-color-scheme), preferensi aksesibilitas pengurangan gerakan (prefers-reduced-motion), gaya cetak dokumen (@media print), revolusi Container Queries (@container) berbasis ukuran elemen induk, hingga penyusunan sistem desain responsif yang terpadu.

## Tujuan Pembelajaran Modul

- Menyusun media queries dengan sintaks range dan operator logika (and, not, only).
- Menerapkan metodologi Mobile-First berbasis min-width sebagai standar industri efisien.
- Menciptakan tipografi fluida yang membesar dan mengecil secara mulus tanpa breakpoint kaku memakai clamp().
- Menyesuaikan antarmuka terhadap kapabilitas perangkat keras (layar sentuh vs mouse presisi melalui hover & pointer).
- Mengimplementasikan Dark Mode otomatis yang sinkron dengan preferensi sistem operasi pengguna.
- Menguasai era baru Container Queries untuk komponen independen yang merespons lebar wadahnya sendiri.

## Daftar Submodul

- [186. Media queries dasar](186_media_queries_basic.css) — [Halaman Preview](186_media_queries_basic.html)
- [187. Breakpoint menggunakan min-width](187_media_min_width.css) — [Halaman Preview](187_media_min_width.html)
- [188. Breakpoint menggunakan max-width](188_media_max_width.css) — [Halaman Preview](188_media_max_width.html)
- [189. Pendekatan mobile-first](189_mobile_first.css) — [Halaman Preview](189_mobile_first.html)
- [190. Pendekatan desktop-first](190_desktop_first.css) — [Halaman Preview](190_desktop_first.html)
- [191. Responsive typography](191_responsive_typography.css) — [Halaman Preview](191_responsive_typography.html)
- [192. Fluid layout](192_fluid_layout.css) — [Halaman Preview](192_fluid_layout.html)
- [193. Tipografi menggunakan clamp()](193_fluid_typography_clamp.css) — [Halaman Preview](193_fluid_typography_clamp.html)
- [194. Responsive images](194_responsive_images.css) — [Halaman Preview](194_responsive_images.html)
- [195. Responsive navigation](195_responsive_navigation.css) — [Halaman Preview](195_responsive_navigation.html)
- [196. Responsive Flexbox](196_responsive_flexbox.css) — [Halaman Preview](196_responsive_flexbox.html)
- [197. Responsive Grid](197_responsive_grid.css) — [Halaman Preview](197_responsive_grid.html)
- [198. Orientation media queries](198_orientation_queries.css) — [Halaman Preview](198_orientation_queries.html)
- [199. Media queries untuk kemampuan hover](199_hover_capability_queries.css) — [Halaman Preview](199_hover_capability_queries.html)
- [200. Media queries untuk pointer](200_pointer_media_queries.css) — [Halaman Preview](200_pointer_media_queries.html)
- [201. Preferensi light dan dark mode](201_prefers_color_scheme.css) — [Halaman Preview](201_prefers_color_scheme.html)
- [202. Preferensi pengurangan gerakan](202_prefers_reduced_motion.css) — [Halaman Preview](202_prefers_reduced_motion.html)
- [203. Media type print dan screen](203_media_print_screen.css) — [Halaman Preview](203_media_print_screen.html)
- [204. Container queries](204_container_queries.css) — [Halaman Preview](204_container_queries.html)
- [205. Responsive design system](205_responsive_design_system.css) — [Halaman Preview](205_responsive_design_system.html)

---

## Pembahasan dan Penjelasan Submodul

### 186. Media queries dasar

**Tujuan:** Memahami struktur sintaks at-rule @media untuk menerapkan gaya bersyarat.

**Konsep Utama:**
At-rule `@media [media-type] and ([feature]) { ... }` memungkinkan stylesheet mengecek kondisi perangkat pengguna (seperti lebar viewport layar) sebelum menerapkan aturan gaya di dalamnya.

**Penjelasan Source Code:**
Mendefinisikan gaya dasar kartu berwarna biru, lalu mengubahnya menjadi hijau pada layar dengan lebar minimal 600px.

**Source code utama:** [186_media_queries_basic.css](186_media_queries_basic.css)

**File pendukung preview:** [186_media_queries_basic.html](186_media_queries_basic.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "186_media_queries_basic.html"
```

**Hasil yang Diharapkan:**
Kotak kartu berpenampilan adaptif dengan informasi kondisi media query yang jelas.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Media queries dasar](output/186_media_queries_basic.png)

---

### 187. Breakpoint menggunakan min-width

**Tujuan:** Menetapkan breakpoint berjenjang ke atas menggunakan fitur min-width.

**Konsep Utama:**
`min-width` memicu gaya ketika lebar layar berada pada atau di atas nilai ambang yang ditentukan. Ini adalah pilar utama pendekatan Mobile-First (mulai dari layar kecil ke layar besar).

**Penjelasan Source Code:**
Menampilkan badge responsif yang warnanya berubah bertahap dari ponsel (merah), tablet (kuning), hingga desktop (hijau).

**Source code utama:** [187_media_min_width.css](187_media_min_width.css)

**File pendukung preview:** [187_media_min_width.html](187_media_min_width.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "187_media_min_width.html"
```

**Hasil yang Diharapkan:**
Lencana status yang menunjukkan breakpoint aktif saat ini.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Breakpoint menggunakan min-width](output/187_media_min_width.png)

---

### 188. Breakpoint menggunakan max-width

**Tujuan:** Menetapkan breakpoint penyusutan dari desktop ke bawah menggunakan max-width.

**Konsep Utama:**
`max-width` memicu gaya ketika lebar layar berada pada atau di bawah nilai tertentu. Pendekatan ini merupakan inti dari strategi Desktop-First (gaya desktop ditulis lebih dulu, lalu dikecilkan untuk layar mobile).

**Penjelasan Source Code:**
Kotak kartu desktop 3 kolom yang menyusut menjadi 1 kolom vertikal saat `max-width: 600px`.

**Source code utama:** [188_media_max_width.css](188_media_max_width.css)

**File pendukung preview:** [188_media_max_width.html](188_media_max_width.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "188_media_max_width.html"
```

**Hasil yang Diharapkan:**
Struktur layout yang menyesuaikan secara elegan saat layar menyempit di bawah 600px.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Breakpoint menggunakan max-width](output/188_media_max_width.png)

---

### 189. Pendekatan mobile-first

**Tujuan:** Menerapkan metodologi arsitektur CSS Mobile-First yang efisien dan minim override.

**Konsep Utama:**
Filosofi Mobile-First mendesain untuk perangkat dengan sumber daya dan layar paling terbatas terlebih dahulu (tanpa media query), kemudian secara progresif menambahkan kompleksitas tata letak ke atas menggunakan `@media (min-width: ...)`.

**Penjelasan Source Code:**
Membangun kartu dengan tata letak satu kolom vertikal di mobile, bertransformasi menjadi dua kolom horizontal di layar yang lebih lebar.

**Source code utama:** [189_mobile_first.css](189_mobile_first.css)

**File pendukung preview:** [189_mobile_first.html](189_mobile_first.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "189_mobile_first.html"
```

**Hasil yang Diharapkan:**
Kartu profil modern yang beralih dari tumpukan vertikal ke baris horizontal secara progresif.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Pendekatan mobile-first](output/189_mobile_first.png)

---

### 190. Pendekatan desktop-first

**Tujuan:** Memahami arsitektur Desktop-First dan cara melakukan override ke layar yang lebih kecil.

**Konsep Utama:**
Pada Desktop-First, gaya awal dirancang untuk layar monitor komputer yang lapang, kemudian aturan ditimpa mundur (graceful degradation) menggunakan `@media (max-width: ...)` untuk mengatasi keterbatasan layar ponsel.

**Penjelasan Source Code:**
Menampilkan navigasi multi-tombol desktop yang dipadatkan saat lebar layar menyempit.

**Source code utama:** [190_desktop_first.css](190_desktop_first.css)

**File pendukung preview:** [190_desktop_first.html](190_desktop_first.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "190_desktop_first.html"
```

**Hasil yang Diharapkan:**
Navigasi desktop yang secara anggun menyusut saat diakses dari layar yang lebih kecil.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Pendekatan desktop-first](output/190_desktop_first.png)

---

### 191. Responsive typography

**Tujuan:** Mengatur ukuran teks agar membesar dan mengecil seirama skala layar menggunakan media queries.

**Konsep Utama:**
Ukuran judul yang terlalu besar pada ponsel (misal 48px) akan merusak tata letak. Melalui media queries, kita menetapkan `font-size: 24px` pada mobile, dan menaikkannya menjadi `font-size: 38px` pada desktop.

**Penjelasan Source Code:**
Mengatur ukuran judul hero secara bertahap pada breakpoint 600px.

**Source code utama:** [191_responsive_typography.css](191_responsive_typography.css)

**File pendukung preview:** [191_responsive_typography.html](191_responsive_typography.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "191_responsive_typography.html"
```

**Hasil yang Diharapkan:**
Judul teks yang proporsional di mobile dan megah di layar lebar desktop.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Responsive typography](output/191_responsive_typography.png)

---

### 192. Fluid layout

**Tujuan:** Membangun tata letak cair berbasis persentase yang meregang lentur tanpa batas langkah kaku.

**Konsep Utama:**
Fluid layout menggunakan satuan persentase (`%`) dan `vw` untuk dimensi elemen, sehingga komponen mengalir cair mengikuti lebar jendela apa pun tanpa bergantung pada breakpoint kaku.

**Penjelasan Source Code:**
Wadah utama diatur `width: 90%` dengan dua kolom `48%` berdampingan.

**Source code utama:** [192_fluid_layout.css](192_fluid_layout.css)

**File pendukung preview:** [192_fluid_layout.html](192_fluid_layout.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "192_fluid_layout.html"
```

**Hasil yang Diharapkan:**
Dua kolom yang meregang elastis seirama perubahan lebar jendela browser.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Fluid layout](output/192_fluid_layout.png)

---

### 193. Tipografi menggunakan clamp()

**Tujuan:** Menciptakan tipografi fluida matematis yang membesar mulus tanpa media query menggunakan clamp().

**Konsep Utama:**
Fungsi `font-size: clamp(min, preferred, max)` mengunci ukuran font: tidak akan pernah lebih kecil dari `min`, bertransisi mulus di nilai `preferred` (berbasis `vw`), dan berhenti membesar di batas `max`.

**Penjelasan Source Code:**
Menerapkan `font-size: clamp(1.25rem, 4vw, 2.5rem)` untuk judul yang selalu sempurna di layar ukuran berapa pun.

**Source code utama:** [193_fluid_typography_clamp.css](193_fluid_typography_clamp.css)

**File pendukung preview:** [193_fluid_typography_clamp.html](193_fluid_typography_clamp.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "193_fluid_typography_clamp.html"
```

**Hasil yang Diharapkan:**
Judul teks berukuran dinamis yang beradaptasi halus seirama pergeseran ukuran jendela.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Tipografi menggunakan clamp()](output/193_fluid_typography_clamp.png)

---

### 194. Responsive images

**Tujuan:** Menjamin aset gambar tidak pernah meluap keluar dari batas kontainernya.

**Konsep Utama:**
Aturan emas gambar responsif di CSS: `max-width: 100%; height: auto; display: block;`. Gambar akan menyusut secara fleksibel bila wadahnya menyempit, namun tidak pernah melar melebihi resolusi aslinya.

**Penjelasan Source Code:**
Memasukkan gambar ke dalam kartu sempit dan membuktikan gambar menyusut proporsional.

**Source code utama:** [194_responsive_images.css](194_responsive_images.css)

**File pendukung preview:** [194_responsive_images.html](194_responsive_images.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "194_responsive_images.html"
```

**Hasil yang Diharapkan:**
Gambar SVG grafis yang terpasang pas di dalam bingkai tanpa merusak lebar kartu.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Responsive images](output/194_responsive_images.png)

---

### 195. Responsive navigation

**Tujuan:** Membangun menu navigasi yang beradaptasi antara mode desktop baris dan mobile tumpuk.

**Konsep Utama:**
Pada mobile, menu navigasi disusun vertikal bertumpuk untuk memudahkan ketukan jari. Pada desktop (`min-width: 600px`), menu bertransformasi menjadi baris horizontal yang kompak.

**Penjelasan Source Code:**
Mengatur flex container navigasi yang beralih dari column di mobile ke row di desktop.

**Source code utama:** [195_responsive_navigation.css](195_responsive_navigation.css)

**File pendukung preview:** [195_responsive_navigation.html](195_responsive_navigation.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "195_responsive_navigation.html"
```

**Hasil yang Diharapkan:**
Menu navigasi adaptif yang ramah sentuhan di ponsel dan ringkas di desktop.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Responsive navigation](output/195_responsive_navigation.png)

---

### 196. Responsive Flexbox

**Tujuan:** Memadukan Flexbox dan Media Queries untuk menciptakan komponen tata letak serbaguna.

**Konsep Utama:**
Pola responsif Flexbox memanfaatkan peralihan `flex-direction: column` ke `row` dan penyesuaian `flex-basis` sesuai lebar viewport.

**Penjelasan Source Code:**
Membuat kartu perbandingan fitur yang otomatis menyesuaikan kolomnya.

**Source code utama:** [196_responsive_flexbox.css](196_responsive_flexbox.css)

**File pendukung preview:** [196_responsive_flexbox.html](196_responsive_flexbox.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "196_responsive_flexbox.html"
```

**Hasil yang Diharapkan:**
Dua kartu fitur yang berdampingan di layar lebar dan bertumpuk di layar sempit.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Responsive Flexbox](output/196_responsive_flexbox.png)

---

### 197. Responsive Grid

**Tujuan:** Mengubah struktur kolom CSS Grid di setiap breakpoint media queries.

**Konsep Utama:**
Di ponsel: 1 kolom `grid-template-columns: 1fr`. Di tablet: 2 kolom `repeat(2, 1fr)`. Di desktop: 3 atau 4 kolom. Memberikan kontrol arsitektural penuh pada setiap ukuran layar.

**Penjelasan Source Code:**
Mengatur galeri produk yang bertransformasi dari 1 kolom ke 2 kolom pada breakpoint 480px.

**Source code utama:** [197_responsive_grid.css](197_responsive_grid.css)

**File pendukung preview:** [197_responsive_grid.html](197_responsive_grid.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "197_responsive_grid.html"
```

**Hasil yang Diharapkan:**
Kisi galeri yang mengembang secara mulus dari 1 kolom ke 2 kolom.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Responsive Grid](output/197_responsive_grid.png)

---

### 198. Orientation media queries

**Tujuan:** Mendeteksi posisi perangkat landscape (mendatar) atau portrait (tegak).

**Konsep Utama:**
Query `@media (orientation: landscape)` dan `(orientation: portrait)` mendeteksi apakah lebar viewport lebih besar daripada tingginya, berguna untuk mengoptimalkan tampilan tablet atau ponsel saat diputar.

**Penjelasan Source Code:**
Menampilkan lencana orientasi yang menandai orientasi layar saat ini.

**Source code utama:** [198_orientation_queries.css](198_orientation_queries.css)

**File pendukung preview:** [198_orientation_queries.html](198_orientation_queries.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "198_orientation_queries.html"
```

**Hasil yang Diharapkan:**
Komponen kartu yang mendeteksi orientasi layar horizontal/vertikal.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Orientation media queries](output/198_orientation_queries.png)

---

### 199. Media queries untuk kemampuan hover

**Tujuan:** Mendeteksi apakah perangkat pengguna mendukung kemampuan hover kursor fisik (mouse) atau tidak (touchscreen).

**Konsep Utama:**
Query `@media (hover: hover)` menargetkan perangkat dengan pointer yang dapat melayang (seperti mouse laptop), sedangkan `@media (hover: none)` menargetkan layar sentuh ponsel di mana efek hover tidak ada.

**Penjelasan Source Code:**
Hanya menerapkan efek transisi hover jika perangkat memang memiliki kursor mouse.

**Source code utama:** [199_hover_capability_queries.css](199_hover_capability_queries.css)

**File pendukung preview:** [199_hover_capability_queries.html](199_hover_capability_queries.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "199_hover_capability_queries.html"
```

**Hasil yang Diharapkan:**
Tombol interaktif yang cerdas mendeteksi kapabilitas hover.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Media queries untuk kemampuan hover](output/199_hover_capability_queries.png)

---

### 200. Media queries untuk pointer

**Tujuan:** Membedakan perangkat dengan pointer presisi (mouse fine) vs pointer sentuhan jari (touch coarse).

**Konsep Utama:**
Query `@media (pointer: coarse)` mendeteksi perangkat dengan akurasi pointer rendah (jari sentuh pada layar ponsel), sehingga tombol harus diperbesar minimal 44x44px. `@media (pointer: fine)` mendeteksi mouse presisi.

**Penjelasan Source Code:**
Membuat tombol yang otomatis membesar dan lebih berjarak di layar sentuh.

**Source code utama:** [200_pointer_media_queries.css](200_pointer_media_queries.css)

**File pendukung preview:** [200_pointer_media_queries.html](200_pointer_media_queries.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "200_pointer_media_queries.html"
```

**Hasil yang Diharapkan:**
Komponen tombol yang otomatis memperbesar target sentuhnya untuk pengguna ponsel.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Media queries untuk pointer](output/200_pointer_media_queries.png)

---

### 201. Preferensi light dan dark mode

**Tujuan:** Menyesuaikan tema warna terang atau gelap otomatis mengikuti preferensi sistem operasi pengguna.

**Konsep Utama:**
Query `@media (prefers-color-scheme: dark)` mendeteksi apakah sistem operasi pengguna diatur dalam mode gelap (Dark Mode). Memungkinkan perubahan palet warna tanpa tombol toggle manual.

**Penjelasan Source Code:**
Mendefinisikan kartu berlatar putih pada mode terang, dan otomatis beralih menjadi hitam elegan pada mode gelap.

**Source code utama:** [201_prefers_color_scheme.css](201_prefers_color_scheme.css)

**File pendukung preview:** [201_prefers_color_scheme.html](201_prefers_color_scheme.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "201_prefers_color_scheme.html"
```

**Hasil yang Diharapkan:**
Kartu adaptif yang otomatis menyinkronkan warnanya dengan preferensi tema sistem operasi.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Preferensi light dan dark mode](output/201_prefers_color_scheme.png)

---

### 202. Preferensi pengurangan gerakan

**Tujuan:** Menghormati aksesibilitas pengguna yang rentan terhadap mabuk gerakan (vestibular disorder).

**Konsep Utama:**
Query `@media (prefers-reduced-motion: reduce)` mendeteksi pengguna yang mengaktifkan pengaturan minim gerakan di sistem operasinya. Wajib mematikan atau menyederhanakan animasi agresif demi kesehatan pengguna.

**Penjelasan Source Code:**
Menonaktifkan animasi berputar saat preferensi reduced motion terdeteksi.

**Source code utama:** [202_prefers_reduced_motion.css](202_prefers_reduced_motion.css)

**File pendukung preview:** [202_prefers_reduced_motion.html](202_prefers_reduced_motion.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "202_prefers_reduced_motion.html"
```

**Hasil yang Diharapkan:**
Elemen yang animasi transformasinya dinonaktifkan secara aman bagi aksesibilitas.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Preferensi pengurangan gerakan](output/202_prefers_reduced_motion.png)

---

### 203. Media type print dan screen

**Tujuan:** Mengatur stylesheet khusus cetak dokumen fisik menggunakan @media print.

**Konsep Utama:**
Query `@media print` menargetkan dokumen saat dicetak ke kertas fisik atau disimpan sebagai PDF. Kita dapat menyembunyikan tombol navigasi, menghilangkan warna latar boros tinta, dan menampilkan URL teks.

**Penjelasan Source Code:**
Menyembunyikan navbar dan tombol cetak saat mode cetak kertas aktif.

**Source code utama:** [203_media_print_screen.css](203_media_print_screen.css)

**File pendukung preview:** [203_media_print_screen.html](203_media_print_screen.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "203_media_print_screen.html"
```

**Hasil yang Diharapkan:**
Tampilan dokumen yang bersih dari elemen interaktif saat dipratinjau untuk dicetak.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Media type print dan screen](output/203_media_print_screen.png)

---

### 204. Container queries

**Tujuan:** Mengatur gaya komponen berdasarkan lebar wadah induknya sendiri menggunakan @container.

**Konsep Utama:**
Container Queries (`@container`) membebaskan komponen dari ketergantungan viewport global. Komponen dapat mengubah tata letaknya sendiri berdasarkan lebar wadah pembungkusnya, menjadikannya komponen modular sejati.

**Penjelasan Source Code:**
Mendefinisikan `container-type: inline-size` pada wadah dan mengubah susunan kartu ketika wadah melebar di atas 400px.

**Source code utama:** [204_container_queries.css](204_container_queries.css)

**File pendukung preview:** [204_container_queries.html](204_container_queries.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "204_container_queries.html"
```

**Hasil yang Diharapkan:**
Komponen kartu modular yang merespons perubahan lebar kontainernya secara independen.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Container queries](output/204_container_queries.png)

---

### 205. Responsive design system

**Tujuan:** Menyatukan breakpoint, skala tipografi, dan grid ke dalam satu sistem desain responsif kohesif.

**Konsep Utama:**
Sistem desain responsif menyatukan token variabel skala spasi, breakpoint konsisten (sm, md, lg), dan pola layout terpadu untuk menjamin seluruh halaman web terasa utuh dan harmonis.

**Penjelasan Source Code:**
Membangun kartu pameran sistem desain lengkap dengan token spacing dan tipografi responsif.

**Source code utama:** [205_responsive_design_system.css](205_responsive_design_system.css)

**File pendukung preview:** [205_responsive_design_system.html](205_responsive_design_system.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "205_responsive_design_system.html"
```

**Hasil yang Diharapkan:**
Struktur kartu UI lengkap dengan header, isi, dan aksi yang mematuhi standar design system.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Responsive design system](output/205_responsive_design_system.png)

---

## Ringkasan Modul

Web diakses melalui ribuan variasi perangkat, mulai dari jam tangan pintar, ponsel lipat, tablet, laptop, hingga monitor 4K. Modul 11 menjamin antarmuka web yang dibangun mampu beradaptasi secara mulus, elegan, dan aksesibel di setiap skenario penggunaan.

### Keterkaitan Materi
Seluruh submodul dalam modul ini dirancang secara berjenjang untuk membangun pemahaman yang kokoh dan aplikatif. Lanjutkan ke modul berikutnya setelah menguasai seluruh konsep di atas.
