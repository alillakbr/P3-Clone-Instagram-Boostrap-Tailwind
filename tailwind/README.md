# Penjelasan Layout Instagram Clone

## 1. Keputusan Grid-cols dan Gap di Tiap Breakpoint
- **Default (mobile kecil)**  
  Menggunakan satu kolom agar setiap post terlihat penuh dan jelas.  
  Gap 8px dipilih untuk memberi jarak antar elemen tanpa membuang banyak ruang.  

- **Tablet (640px – 1023px)**  
  Menggunakan tiga kolom karena layar menengah mampu menampilkan lebih banyak konten.  
  Tiga kolom juga meniru tampilan grid Instagram.  

- **Desktop (≥ 1024px)**  
  Menggunakan empat kolom untuk memanfaatkan ruang layar besar agar lebih padat.  
  Lebih efisien karena banyak konten dapat ditampilkan dalam sekali scroll.  

- **Gap konsisten**  
  Tetap digunakan di semua ukuran agar jarak antar gambar rapi dan seragam.  

---

## 2. Pemanfaatan Utility Responsive Tailwind
- Tailwind menyediakan prefix breakpoint seperti `sm:`, `md:`, `lg:` sehingga tidak perlu menulis media query manual.  
- Prinsip penerapan:  
  - Mobile kecil: satu kolom, fokus pada keterbacaan konten.  
  - Tablet: tiga kolom, seimbang untuk layar menengah.  
  - Desktop: empat kolom, optimal untuk layar besar.  
- Contoh penggunaan lain adalah pada **profile-stats**, yang diatur berbeda untuk mobile agar lebih mudah dibaca.  

---

## 3. Trade-off Utility Classes dan Component CSS
- **Utility Classes**  
  - Kelebihan: cepat untuk prototyping, konsisten, hasil langsung terlihat.  
  - Kekurangan: class bisa sangat panjang dan sulit dibaca pada layout kompleks.  

- **Component CSS**  
  - Kelebihan: HTML lebih bersih, mudah dipakai ulang, mendukung styling kompleks.  
  - Kekurangan: membutuhkan file CSS tambahan, workflow lebih lambat, berpotensi menimbulkan konflik style.  

- **Kompromi**  
  Gunakan utility classes untuk layout sederhana atau eksperimen cepat.  
  Refactor menjadi component CSS jika pola sama dipakai berulang atau perlu konsistensi jangka panjang.  
