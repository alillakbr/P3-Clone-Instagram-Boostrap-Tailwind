## 🔹 Struktur Utama

```html
<!DOCTYPE html>
<html lang="en">
<head> ... </head>
<body> ... </body>
</html>
```

* **DOCTYPE html** → tandanya pakai HTML5.
* **lang="en"** → set bahasa halaman ke English.
* **head** → bagian meta, judul, link CSS.
* **body** → isi utama halaman.

---

## 🔹 Bagian Head

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Instagram Desktop Clone</title>
<script src="https://cdn.tailwindcss.com"></script>
```

* `charset="UTF-8"` → biar semua karakter (emoji, huruf unik) terbaca.
* `viewport` → bikin halaman responsif di HP/laptop.
* `title` → judul tab browser.
* `tailwindcss.com` → import **Tailwind CSS** lewat CDN (gak perlu install manual).

---

## 🔹 Body Utama

```html
<body class="bg-black text-white">
<div class="max-w-4xl mx-auto py-6 px-4">
```

* `bg-black text-white` → latar belakang hitam, teks putih (mirip IG dark mode).
* `max-w-4xl mx-auto` → lebar maksimal kontainer 4xl & rata tengah.
* `py-6 px-4` → padding atas-bawah 6, kiri-kanan 4.

---

## 🔹 Profile Section

* **Foto profil** → `<img src="pp.jpg" class="w-36 h-36 rounded-full mr-8">` (bulat, ukuran 36).
* **Username + tombol** → pakai `flex space-x-4`. Ada **Edit profile, View archive, dan ikon gear**.
* **Statistik** → jumlah postingan, followers, following.
* **Bio** → teks singkat + link handle.

---

## 🔹 Highlights (Sorotan Story)

```html
<div class="flex space-x-6 mb-12">
```

* Menampilkan 3 sorotan (foto bulat + teks di bawahnya).
* Ada 1 tambahan bulat kosong dengan ikon **+ New** buat tambah highlight.

---

## 🔹 Tabs Navigasi

```html
<div class="flex justify-center border-t border-neutral-700 border-b mb-6">
```

* Ada 3 tab:

  * **Posts** (grid ikon).
  * **Saved** (ikon bookmark).
  * **Mentions** (ikon person).
* Tombol berubah warna pas **hover**.

---

## 🔹 Posts Grid

```html
<div class="grid grid-cols-3 gap-1">
```

* Grid 3 kolom.
* Tiap postingan: gambar + overlay muncul saat di-hover (`opacity-0 group-hover:opacity-100`).
* Overlay isi jumlah **likes ❤️** dan **comments 💬**.

---

## 🔹 Footer

```html
<footer class="text-neutral-500 text-center text-sm py-8 space-x-4">
```

* Mirip footer IG asli → ada link "Meta, About, Blog, Jobs, Help, Privacy, Terms..."
* Teks kecil abu-abu.
* Ada copyright: `© 2025 Instagram from Meta`.

---

Bootstrap Icons

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css">
```

* Ini **import Bootstrap Icons** (ikon gear, hati, komentar, plus, grid, dll).
* Dipanggil dengan `<i class="bi bi-..."></i>`.

Jadi singkatnya:

* **Tailwind CSS** → buat styling (warna, margin, flexbox, grid).
* **Bootstrap Icons** → buat ikon-ikon kecil (gear, bookmark, heart, chat).
* Struktur halaman → profil → highlights → tabs → grid posts → footer.
