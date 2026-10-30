# Modul 02: CSS Selectors

## Ringkasan Ruang Lingkup Materi

Modul ini membahas ragam selector CSS secara menyeluruh: universal selector (*), element selector, class selector, ID selector, grouping selector, combinators (descendant, child >, adjacent sibling +, general sibling ~), keluarga attribute selectors ([attr], exact =, contains *=, prefix ^=, suffix $=, word ~=, hyphen |=), kombinasi selector ganda, hingga complex selectors dan pola daftar selector.

## Tujuan Pembelajaran Modul

- Memahami dan mengimplementasikan selector dasar (universal, element, class, ID).
- Menggunakan combinator relasional (anak, turunan, saudara dekat, saudara umum).
- Menguasai seluruh variasi selector atribut untuk menargetkan elemen berdasarkan atribut dan nilainya.
- Menyusun kombinasi selector bertingkat dan mengelola pengelompokan selector secara efisien.
- Menganalisis performa dan keterbacaan selector kompleks pada struktur dokumen HTML nyata.

## Daftar Submodul

- [16. Universal selector](16_universal_selector.css) — [Halaman Preview](16_universal_selector.html)
- [17. Element selector](17_element_selector.css) — [Halaman Preview](17_element_selector.html)
- [18. Class selector](18_class_selector.css) — [Halaman Preview](18_class_selector.html)
- [19. ID selector](19_id_selector.css) — [Halaman Preview](19_id_selector.html)
- [20. Grouping selector](20_grouping_selector.css) — [Halaman Preview](20_grouping_selector.html)
- [21. Descendant selector](21_descendant_selector.css) — [Halaman Preview](21_descendant_selector.html)
- [22. Child combinator](22_child_selector.css) — [Halaman Preview](22_child_selector.html)
- [23. Adjacent sibling combinator](23_adjacent_sibling_selector.css) — [Halaman Preview](23_adjacent_sibling_selector.html)
- [24. General sibling combinator](24_general_sibling_selector.css) — [Halaman Preview](24_general_sibling_selector.html)
- [25. Attribute selector](25_attribute_selector.css) — [Halaman Preview](25_attribute_selector.html)
- [26. Exact attribute matching](26_attribute_exact_match.css) — [Halaman Preview](26_attribute_exact_match.html)
- [27. Attribute substring matching](27_attribute_contains.css) — [Halaman Preview](27_attribute_contains.html)
- [28. Attribute prefix matching](28_attribute_prefix.css) — [Halaman Preview](28_attribute_prefix.html)
- [29. Attribute suffix matching](29_attribute_suffix.css) — [Halaman Preview](29_attribute_suffix.html)
- [30. Attribute word matching](30_attribute_word_match.css) — [Halaman Preview](30_attribute_word_match.html)
- [31. Attribute hyphen matching](31_attribute_hyphen_match.css) — [Halaman Preview](31_attribute_hyphen_match.html)
- [32. Kombinasi selector](32_selector_combinations.css) — [Halaman Preview](32_selector_combinations.html)
- [33. Multiple class selectors](33_multiple_class_selectors.css) — [Halaman Preview](33_multiple_class_selectors.html)
- [34. Complex selectors](34_complex_selectors.css) — [Halaman Preview](34_complex_selectors.html)
- [35. Pola selector list](35_selector_list_patterns.css) — [Halaman Preview](35_selector_list_patterns.html)

---

## Pembahasan dan Penjelasan Submodul

### 16. Universal selector

**Tujuan:** Menargetkan seluruh elemen dalam dokumen menggunakan tanda bintang (*).

**Konsep Utama:**
Universal selector `*` mencocokkan setiap elemen dari tipe apa pun pada dokumen atau dalam konteks wadah tertentu. Sering dipakai untuk reset global batas margin dan padding.

**Penjelasan Source Code:**
Selector `*` digunakan untuk menyamakan box-sizing dan menghapus margin/padding bawaan, diikuti penataan kontainer kartu.

**Source code utama:** [16_universal_selector.css](16_universal_selector.css)

**File pendukung preview:** [16_universal_selector.html](16_universal_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "16_universal_selector.html"
```

**Hasil yang Diharapkan:**
Halaman bersih tanpa celah margin bawaan browser di sekeliling elemen.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Universal selector](output/16_universal_selector.png)

---

### 17. Element selector

**Tujuan:** Menargetkan elemen berdasarkan nama tag HTML (elemen tipe).

**Konsep Utama:**
Element selector (dikenal juga sebagai type selector) mencocokkan semua elemen yang memiliki nama tag yang sama, seperti `p`, `h1`, `blockquote`, atau `table`.

**Penjelasan Source Code:**
Menata tag `h2`, `p`, dan `blockquote` secara langsung untuk membangun hierarki tipografi standar dokumen.

**Source code utama:** [17_element_selector.css](17_element_selector.css)

**File pendukung preview:** [17_element_selector.html](17_element_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "17_element_selector.html"
```

**Hasil yang Diharapkan:**
Struktur artikel terformat dengan heading elegan, teks teratur, dan kutipan bergaris batas.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Element selector](output/17_element_selector.png)

---

### 18. Class selector

**Tujuan:** Menargetkan satu atau banyak elemen menggunakan atribut class dengan prefiks titik (.).

**Konsep Utama:**
Class selector diawali dengan tanda titik (`.`) diikuti nama kelas. Satu kelas dapat dipakai berkali-kali pada elemen berbeda di satu dokumen yang sama, menjadikannya pilar utama modularitas CSS.

**Penjelasan Source Code:**
Membuat kelas komponen `.btn`, `.btn-primary`, dan `.btn-secondary` yang dapat dipasangkan fleksibel pada elemen tombol atau tautan.

**Source code utama:** [18_class_selector.css](18_class_selector.css)

**File pendukung preview:** [18_class_selector.html](18_class_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "18_class_selector.html"
```

**Hasil yang Diharapkan:**
Dua tombol aksi dengan basis bentuk yang sama namun memiliki warna tema primer dan sekunder berbeda.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Class selector](output/18_class_selector.png)

---

### 19. ID selector

**Tujuan:** Menargetkan elemen tunggal yang unik dalam dokumen menggunakan atribut id dengan prefiks tagar (#).

**Konsep Utama:**
ID selector diawali tanda `#`. Dalam standar HTML, nilai ID harus unik dalam satu dokumen. Memiliki spesifisitas yang jauh lebih tinggi daripada class selector.

**Penjelasan Source Code:**
Menata elemen `#main-navbar` dengan warna latar gelap dan posisi tetap di bagian atas.

**Source code utama:** [19_id_selector.css](19_id_selector.css)

**File pendukung preview:** [19_id_selector.html](19_id_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "19_id_selector.html"
```

**Hasil yang Diharapkan:**
Bilah navigasi utama dengan tampilan header eksklusif yang ditargetkan secara presisi melalui ID unik.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi ID selector](output/19_id_selector.png)

---

### 20. Grouping selector

**Tujuan:** Mengelompokkan beberapa selector menggunakan tanda koma (,) untuk efisiensi deklarasi gaya bersama.

**Konsep Utama:**
Jika beberapa selector membutuhkan deklarasi properti yang persis sama, selector tersebut dapat digabungkan dengan memisahkannya menggunakan tanda koma (`,`). Ini menerapkan prinsip DRY (Don't Repeat Yourself).

**Penjelasan Source Code:**
Elemen `h1`, `h2`, dan `h3` dikelompokkan untuk berbagi jenis font dan margin, lalu diberi pewarnaan khusus bertingkat.

**Source code utama:** [20_grouping_selector.css](20_grouping_selector.css)

**File pendukung preview:** [20_grouping_selector.html](20_grouping_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "20_grouping_selector.html"
```

**Hasil yang Diharapkan:**
Tiga level judul dengan konsistensi font dan warna keluarga biru dongker yang rapi.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Grouping selector](output/20_grouping_selector.png)

---

### 21. Descendant selector

**Tujuan:** Menargetkan elemen keturunan (turunan sedalam apa pun) menggunakan spasi kosong sebagai pemisah.

**Konsep Utama:**
Descendant selector `A B` mencocokkan seluruh elemen B yang berada di dalam elemen A, tidak peduli seberapa dalam tingkat sarangannya (anak langsung, cucu, cicit).

**Penjelasan Source Code:**
Selector `.article-card p` memilih semua tag p di dalam kartu artikel dan memberikan warna khusus tanpa memengaruhi p di luar kartu.

**Source code utama:** [21_descendant_selector.css](21_descendant_selector.css)

**File pendukung preview:** [21_descendant_selector.html](21_descendant_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "21_descendant_selector.html"
```

**Hasil yang Diharapkan:**
Paragraf di dalam kartu artikel memiliki format khusus abu-abu elegan, sedangkan paragraf luar tetap standar.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Descendant selector](output/21_descendant_selector.png)

---

### 22. Child combinator

**Tujuan:** Menargetkan hanya elemen anak langsung (direct child) menggunakan tanda kurung siku siku tutup (>).

**Konsep Utama:**
Child combinator `A > B` hanya mencocokkan elemen B yang merupakan keturunan langsung (anak tingkat pertama) dari elemen A, mengabaikan cucu atau tingkat lebih dalam.

**Penjelasan Source Code:**
Selector `ul.nav-menu > li` menata item menu utama, sementara submenu bersarang di dalam li tidak terkena aturan yang sama.

**Source code utama:** [22_child_selector.css](22_child_selector.css)

**File pendukung preview:** [22_child_selector.html](22_child_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "22_child_selector.html"
```

**Hasil yang Diharapkan:**
Menu navigasi horizontal di mana hanya item tingkat pertama yang berjejer horizontal, sedangkan submenu anak tetap vertikal.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Child combinator](output/22_child_selector.png)

---

### 23. Adjacent sibling combinator

**Tujuan:** Menargetkan elemen saudara terdekat yang berada tepat setelah elemen referensi menggunakan tanda tambah (+).

**Konsep Utama:**
Adjacent sibling combinator `A + B` mencocokkan elemen B yang langsung berdampingan tepat setelah elemen A dalam hierarki induk yang sama.

**Penjelasan Source Code:**
Selector `h2 + p` secara khusus menata paragraf pembuka (lead paragraph) yang muncul persis setelah judul `h2`.

**Source code utama:** [23_adjacent_sibling_selector.css](23_adjacent_sibling_selector.css)

**File pendukung preview:** [23_adjacent_sibling_selector.html](23_adjacent_sibling_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "23_adjacent_sibling_selector.html"
```

**Hasil yang Diharapkan:**
Paragraf pertama setelah heading memiliki ukuran font lebih besar dan tebal, sedangkan paragraf kedua berukuran normal.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Adjacent sibling combinator](output/23_adjacent_sibling_selector.png)

---

### 24. General sibling combinator

**Tujuan:** Menargetkan semua saudara kandung setelah elemen referensi menggunakan tanda tilde (~).

**Konsep Utama:**
General sibling combinator `A ~ B` mencocokkan semua elemen B yang terletak setelah elemen A dan memiliki induk yang sama, tidak harus berdampingan langsung.

**Penjelasan Source Code:**
Selector `.target-flag ~ p` memilih seluruh paragraf yang berada setelah elemen penanda `.target-flag`.

**Source code utama:** [24_general_sibling_selector.css](24_general_sibling_selector.css)

**File pendukung preview:** [24_general_sibling_selector.html](24_general_sibling_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "24_general_sibling_selector.html"
```

**Hasil yang Diharapkan:**
Seluruh paragraf setelah garis penanda diberi aksen warna dan indentasi khusus.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi General sibling combinator](output/24_general_sibling_selector.png)

---

### 25. Attribute selector

**Tujuan:** Menargetkan elemen berdasarkan keberadaan atribut tertentu [attr].

**Konsep Utama:**
Attribute selector `[attr]` mencocokkan setiap elemen yang memiliki atribut tersebut, tanpa memperhitungkan berapa nilai yang terkandung di dalamnya.

**Penjelasan Source Code:**
Selector `input[required]` dan `a[target]` memberikan indikator visual pada formulir yang wajib diisi dan tautan eksternal.

**Source code utama:** [25_attribute_selector.css](25_attribute_selector.css)

**File pendukung preview:** [25_attribute_selector.html](25_attribute_selector.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "25_attribute_selector.html"
```

**Hasil yang Diharapkan:**
Input form yang memiliki atribut required diberi batas border oranye peringatan.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Attribute selector](output/25_attribute_selector.png)

---

### 26. Exact attribute matching

**Tujuan:** Menargetkan elemen yang nilai atributnya persis sama menggunakan [attr='val'].

**Konsep Utama:**
Exact attribute selector `[attr='val']` hanya mencocokkan elemen bila isi atribut tersebut sama persis secara menyeluruh dengan string yang dicantumkan.

**Penjelasan Source Code:**
Menata input form berdasarkan tipenya secara tepat sasaran (`input[type='text']`, `input[type='password']`, `button[type='submit']`).

**Source code utama:** [26_attribute_exact_match.css](26_attribute_exact_match.css)

**File pendukung preview:** [26_attribute_exact_match.html](26_attribute_exact_match.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "26_attribute_exact_match.html"
```

**Hasil yang Diharapkan:**
Form login yang rapi dengan gaya khusus untuk input teks, password, dan tombol kirim.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Exact attribute matching](output/26_attribute_exact_match.png)

---

### 27. Attribute substring matching

**Tujuan:** Menargetkan elemen yang atributnya memuat cuplikan teks tertentu menggunakan [attr*='val'].

**Konsep Utama:**
Substring match selector `[attr*='val']` mencocokkan elemen jika string 'val' ditemukan di posisi mana saja di dalam nilai atribut tersebut.

**Penjelasan Source Code:**
Selector `a[href*='youtube']` memberikan gaya khusus merah dan ikon teks untuk tautan video streaming.

**Source code utama:** [27_attribute_contains.css](27_attribute_contains.css)

**File pendukung preview:** [27_attribute_contains.html](27_attribute_contains.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "27_attribute_contains.html"
```

**Hasil yang Diharapkan:**
Tautan yang mengarah ke platform YouTube secara otomatis berpenampilan merah dengan label video.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Attribute substring matching](output/27_attribute_contains.png)

---

### 28. Attribute prefix matching

**Tujuan:** Menargetkan elemen yang nilai atributnya diawali teks tertentu menggunakan [attr^='val'].

**Konsep Utama:**
Prefix match selector `[attr^='val']` mencocokkan elemen bila nilai atribut dimulai persis dengan string 'val'. Sangat lazim untuk mendeteksi protokol protokol aman https:// atau tel:.

**Penjelasan Source Code:**
Menargetkan tautan aman `a[href^='https://']` dengan warna hijau dan gembok indikator keamanan.

**Source code utama:** [28_attribute_prefix.css](28_attribute_prefix.css)

**File pendukung preview:** [28_attribute_prefix.html](28_attribute_prefix.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "28_attribute_prefix.html"
```

**Hasil yang Diharapkan:**
Tautan HTTPS memiliki styling hijau yang menandakan koneksi aman terenkripsi.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Attribute prefix matching](output/28_attribute_prefix.png)

---

### 29. Attribute suffix matching

**Tujuan:** Menargetkan elemen yang nilai atributnya diakhiri teks tertentu menggunakan [attr$='val'].

**Konsep Utama:**
Suffix match selector `[attr$='val']` mencocokkan elemen jika nilai atribut berakhir dengan string 'val'. Sangat ampuh untuk memberikan ikon sesuai ekstensi file unduhan (.pdf, .zip, .png).

**Penjelasan Source Code:**
Selector `a[href$='.pdf']` memberikan lencana oranye khusus dokumen, sementara `a[href$='.zip']` bertema ungu arsip.

**Source code utama:** [29_attribute_suffix.css](29_attribute_suffix.css)

**File pendukung preview:** [29_attribute_suffix.html](29_attribute_suffix.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "29_attribute_suffix.html"
```

**Hasil yang Diharapkan:**
Dua link download file terformat otomatis dengan warna indikator tipe file yang sesuai.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Attribute suffix matching](output/29_attribute_suffix.png)

---

### 30. Attribute word matching

**Tujuan:** Menargetkan elemen jika atributnya memuat kata utuh tertentu yang dipisahkan spasi menggunakan [attr~='val'].

**Konsep Utama:**
Word match selector `[attr~='val']` mencocokkan bila 'val' merupakan satu kata utuh dalam daftar kata yang dipisahkan spasi pada atribut target.

**Penjelasan Source Code:**
Selector `[data-tags~='urgent']` menargetkan kartu tugas yang memiliki tag urgent di antara deretan tag lainnya.

**Source code utama:** [30_attribute_word_match.css](30_attribute_word_match.css)

**File pendukung preview:** [30_attribute_word_match.html](30_attribute_word_match.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "30_attribute_word_match.html"
```

**Hasil yang Diharapkan:**
Kartu tugas mendesak memiliki bingkai merah cerah dan badge darurat.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Attribute word matching](output/30_attribute_word_match.png)

---

### 31. Attribute hyphen matching

**Tujuan:** Menargetkan elemen bahasa atau kode yang diawali nilai dan diikuti tanda hubung menggunakan [attr|='val'].

**Konsep Utama:**
Hyphen match selector `[attr|='val']` mencocokkan elemen bila nilai atributnya persis 'val' ATAU diawali dengan 'val-'. Umumnya digunakan untuk kode bahasa (lang='id' atau lang='id-ID').

**Penjelasan Source Code:**
Selector `[lang|='id']` memberikan aksen warna bendera merah putih lembut pada teks berbahasa Indonesia.

**Source code utama:** [31_attribute_hyphen_match.css](31_attribute_hyphen_match.css)

**File pendukung preview:** [31_attribute_hyphen_match.html](31_attribute_hyphen_match.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "31_attribute_hyphen_match.html"
```

**Hasil yang Diharapkan:**
Paragraf berbahasa Indonesia dihias dengan aksen khusus yang dideteksi otomatis dari atribut lang.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Attribute hyphen matching](output/31_attribute_hyphen_match.png)

---

### 32. Kombinasi selector

**Tujuan:** Menggabungkan beberapa tipe selector (tag + class + attribute) menjadi satu ekspresi seleksi.

**Konsep Utama:**
Selector dapat digabungkan tanpa spasi untuk mensyaratkan semua kriteria terpenuhi sekaligus. Contoh: `button.primary[disabled]` menargetkan elemen button bertipe class primary yang sedang disabled.

**Penjelasan Source Code:**
Selector `a.external-link[target='_blank']` menyeleksi link yang memenuhi ketiga syarat tersebut sekaligus.

**Source code utama:** [32_selector_combinations.css](32_selector_combinations.css)

**File pendukung preview:** [32_selector_combinations.html](32_selector_combinations.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "32_selector_combinations.html"
```

**Hasil yang Diharapkan:**
Tombol tautan eksternal yang terformat khusus dengan simbol eksternal.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Kombinasi selector](output/32_selector_combinations.png)

---

### 33. Multiple class selectors

**Tujuan:** Menargetkan elemen yang memiliki dua atau lebih kelas sekaligus (.classA.classB).

**Konsep Utama:**
Ketika dua nama kelas dirangkai tanpa spasi (`.classA.classB`), selector hanya cocok untuk elemen yang memiliki kedua kelas tersebut pada saat bersamaan.

**Penjelasan Source Code:**
Selector `.badge.danger` hanya aktif jika elemen memiliki kedua kelas tersebut, memisahkannya dari badge biasa.

**Source code utama:** [33_multiple_class_selectors.css](33_multiple_class_selectors.css)

**File pendukung preview:** [33_multiple_class_selectors.html](33_multiple_class_selectors.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "33_multiple_class_selectors.html"
```

**Hasil yang Diharapkan:**
Lencana biasa berwarna abu-abu, sedangkan lencana yang juga memiliki kelas danger berwarna merah tegas.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Multiple class selectors](output/33_multiple_class_selectors.png)

---

### 34. Complex selectors

**Tujuan:** Menyusun selector kompleks yang menggabungkan berbagai combinator untuk menembus struktur hierarki DOM yang rumit.

**Konsep Utama:**
Complex selector memadukan kombinasi tipe, kelas, atribut, dan combinators seperti `.card > .header h3 + span` untuk menargetkan elemen di lokasi yang sangat spesifik.

**Penjelasan Source Code:**
Selector menata subjudul kartu yang terletak persis setelah judul h3 di dalam header kartu produk.

**Source code utama:** [34_complex_selectors.css](34_complex_selectors.css)

**File pendukung preview:** [34_complex_selectors.html](34_complex_selectors.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "34_complex_selectors.html"
```

**Hasil yang Diharapkan:**
Elemen waktu rilis kartu tampil dengan warna muted dan ukuran proporsional persis di bawah judul kartu.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Complex selectors](output/34_complex_selectors.png)

---

### 35. Pola selector list

**Tujuan:** Menulis daftar selector yang efisien, mudah dirawat, dan terhindar dari invalidasi seluruh ruleset.

**Konsep Utama:**
Selector list memisahkan beberapa selector dengan koma. Penting diperhatikan bahwa pada CSS tradisional, bila ada satu selector tidak valid dalam daftar koma, seluruh ruleset akan gugur.

**Penjelasan Source Code:**
Mendemonstrasikan penulisan daftar selector bertingkat yang rapi per baris untuk mempermudah code review dan git diff.

**Source code utama:** [35_selector_list_patterns.css](35_selector_list_patterns.css)

**File pendukung preview:** [35_selector_list_patterns.html](35_selector_list_patterns.html)

**Cara Menjalankan:**
Buka file HTML pendukung di peramban web (Google Chrome, Microsoft Edge, atau Mozilla Firefox), atau gunakan Live Server / HTTP Server:

```bash
# Buka langsung file HTML di browser default
start "" "35_selector_list_patterns.html"
```

**Hasil yang Diharapkan:**
Berbagai elemen form (input, textarea, select) memiliki visual fokus dan border yang konsisten.

**Screenshot Hasil Eksekusi:**

![Hasil eksekusi Pola selector list](output/35_selector_list_patterns.png)

---

## Ringkasan Modul

Penguasaan CSS Selectors pada Modul 2 membuka fleksibilitas tinggi dalam menargetkan elemen HTML secara tepat sasaran tanpa mengotori markup dengan class berlebihan. Pemahaman combinator dan attribute selectors merupakan bekal utama dalam memahami kalkulasi specificity pada Modul 3.

### Keterkaitan Materi
Seluruh submodul dalam modul ini dirancang secara berjenjang untuk membangun pemahaman yang kokoh dan aplikatif. Lanjutkan ke modul berikutnya setelah menguasai seluruh konsep di atas.
