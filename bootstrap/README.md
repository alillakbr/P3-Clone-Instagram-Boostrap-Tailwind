# Instagram Bootstrap Clone

Proyek ini merupakan replika sederhana halaman profil Instagram menggunakan **Bootstrap 5** dan **Bootstrap Icons**.  
Fokus utamanya adalah menampilkan profil, sorotan, tab navigasi, grid postingan, serta footer dengan layout yang mirip Instagram.

---

## 1. Keputusan Grid dan Breakpoint
- **Bootstrap Grid System** digunakan untuk mengatur tata letak postingan.  
- Setiap post ditempatkan dalam `.col-12 col-sm-4 col-lg-3`:  
  - `col-12` → mobile kecil menampilkan **1 kolom penuh** agar konten terbaca jelas.  
  - `col-sm-4` → pada tablet (≥576px) menjadi **3 kolom** sehingga layout lebih padat.  
  - `col-lg-3` → pada desktop (≥992px) menjadi **4 kolom** untuk memanfaatkan lebar layar.  
- Kelas `.row.g-1` memberi jarak antar post (1 unit gap Bootstrap).  

---

## 2. Pemanfaatan Fitur Bootstrap
- **Grid System** untuk mengatur layout responsif tanpa perlu CSS tambahan yang rumit.  
- **Bootstrap Icons** digunakan pada tombol, overlay post (ikon hati dan komentar), serta tab navigasi.  
- **Utility Classes** seperti `d-flex`, `gap-3`, `text-center`, `rounded-circle` mempercepat styling.  
- **Nav Tabs** digunakan untuk meniru tab navigasi Instagram (Posts, Saved, Tagged).  

---

## 3. CSS Kustom
Beberapa CSS kustom ditambahkan untuk meniru efek Instagram:  
- `.post-container` dengan `aspect-ratio: 1/1` memastikan gambar selalu kotak.  
- `.post-overlay` menampilkan jumlah like dan komentar saat di-hover.  
- Styling tab: `nav-tabs .nav-link.active` diberi garis atas putih agar mirip Instagram.  
- Warna dasar: `body { background-color: #000; color: #fff; }` untuk tema gelap.  

---

## 4. Trade-off Bootstrap Utility vs CSS Kustom
- **Bootstrap Utility**  
  - Kelebihan: cepat, konsisten, dan responsif tanpa tambahan banyak kode.  
  - Kekurangan: keterbatasan dalam efek visual yang lebih kompleks.  

- **CSS Kustom**  
  - Kelebihan: fleksibilitas tinggi, mendukung fitur seperti overlay hover dan rasio aspek.  
  - Kekurangan: butuh kode tambahan, perawatan lebih banyak jika proyek besar.  

---

## 5. Struktur Halaman
1. **Profile Section**  
   Menampilkan foto profil, nama, tombol aksi, statistik, bio, dan link.  

2. **Highlights Section**  
   Menampilkan sorotan cerita dengan foto berbentuk lingkaran dan opsi tambah sorotan baru.  

3. **Tabs Section**  
   Tab navigasi dengan ikon grid, bookmark, dan tagged.  

4. **Posts Grid**  
   Galeri foto berbentuk grid dengan overlay jumlah like dan komentar.  

5. **Footer**  
   Link navigasi tambahan (About, Blog, Jobs, Help, dll) serta copyright.  

---

## 6. Teknologi yang Digunakan
- **Bootstrap 5.3** untuk grid system, komponen, dan utilitas.  
- **Bootstrap Icons 1.11** untuk ikon antarmuka.  
- **HTML5 & CSS3** dengan tambahan custom styling.  
