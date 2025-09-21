# 📌 Penjelasan Bootstrap

## 1. Apa itu Bootstrap?

**Bootstrap** adalah framework **CSS open-source** yang digunakan untuk membuat website responsif dan cepat.

* Dikembangkan oleh **Twitter** (2011).
* Sekarang jadi salah satu library front-end paling populer.
* Fungsinya untuk mempermudah styling **HTML** tanpa harus menulis banyak **CSS manual**.

---

## 2. Kenapa Bootstrap Dipakai?

* 📱 **Responsif otomatis** → desain menyesuaikan layar HP, tablet, dan laptop.
* ⚡ **Cepat** → banyak komponen siap pakai (navbar, card, button, form, dll).
* 🎨 **Konsisten** → tampilan UI rapi tanpa styling manual terlalu banyak.
* 🔧 **Mudah digabung** → bisa dipakai bareng framework lain (contoh: Tailwind, React, Vue).

---

## 3. Cara Menggunakan Bootstrap

Di kode kamu, Bootstrap dipanggil lewat **CDN**:

```html
<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" 
      rel="stylesheet">

<!-- Bootstrap Icons -->
<link rel="stylesheet" 
      href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css">
```

* **CSS Bootstrap** → memberikan gaya bawaan untuk elemen HTML.
* **Bootstrap Icons** → pustaka ikon siap pakai (contoh: gear, bookmark, love, chat).

---

## 4. Fitur Bootstrap yang Terlihat di Kode

1. **Tombol & Layout**

   ```html
   <button class="bg-neutral-800 rounded-md px-3 py-1 text-sm font-semibold btn-animate">
     Edit profile
   </button>
   ```

   👉 Walau ditambah Tailwind, tetap bisa pakai utilitas Bootstrap kalau mau.

2. **Ikon dari Bootstrap Icons**

   ```html
   <i class="bi bi-gear text-2xl"></i>   <!-- Ikon Gear (Pengaturan) -->
   <i class="bi bi-bookmark text-lg"></i> <!-- Ikon Bookmark -->
   <i class="bi bi-heart-fill"></i>       <!-- Ikon Love -->
   ```

   👉 `bi bi-nama-icon` adalah class standar untuk menampilkan ikon Bootstrap.

---

## 5. Contoh Komponen Lain dari Bootstrap

Selain ikon, Bootstrap juga punya:

* **Grid system** (`.row`, `.col`) untuk layout.
* **Form control** (input, checkbox, radio, dropdown).
* **Navbar** (navigasi siap pakai).
* **Modal & Alert** untuk pop-up pesan.
* **Carousel** untuk slideshow gambar.

---

## 6. Ringkasan

Bootstrap di kode kamu dipakai untuk:

* **Icons** (gear, bookmark, heart, chat, person).
* **CSS tambahan** untuk mendukung layout (walau mayoritas dipakai Tailwind).

Jadi fungsinya lebih ke **memanfaatkan ikon bawaan Bootstrap** biar nggak perlu cari ikon manual.
