# 🌐 BAB 1 — Pengenalan HTML5

## 1.1 Apa Itu HTML5?
**HTML5 (HyperText Markup Language versi 5)** adalah **bahasa standar untuk membuat dan menyusun halaman web**.  
HTML5 merupakan versi terbaru dari HTML yang membawa banyak peningkatan seperti:
- Tag semantik baru (`<header>`, `<article>`, `<footer>`, dll)
- Dukungan multimedia bawaan (`<audio>`, `<video>`)
- Elemen grafis seperti `<canvas>`
- Form input baru (misalnya `email`, `date`, `number`)
- API tambahan untuk aplikasi web modern

> 💡 HTML5 dirancang untuk membuat web **lebih interaktif, terstruktur, dan ramah perangkat** — tanpa memerlukan plugin tambahan seperti Flash.

---

## 1.2 Sejarah Singkat HTML
| Versi | Tahun | Pengembang | Fitur Penting |
|--------|--------|-------------|----------------|
| HTML 1.0 | 1993 | Tim Berners-Lee | Dasar hyperlink & teks |
| HTML 2.0 | 1995 | IETF | Standarisasi elemen umum |
| HTML 3.2 | 1997 | W3C | Dukungan tabel & skrip |
| HTML 4.01 | 1999 | W3C | Peningkatan struktur, form |
| XHTML 1.0 | 2000 | W3C | Sintaks XML ketat |
| **HTML5** | **2014 (W3C)** | WHATWG & W3C | Multimedia, API, semantik |

> 🎯 Sejak HTML5, pengembang web tidak lagi hanya membuat halaman statis — tapi bisa membangun **aplikasi web dinamis** yang bisa dijalankan di desktop maupun mobile.

---

## 1.3 Fungsi dan Peran HTML5
HTML5 berperan sebagai **kerangka dasar** halaman web yang bekerja sama dengan:
- **CSS (Cascading Style Sheets)** → untuk tampilan dan layout  
- **JavaScript (ES6/DOM)** → untuk logika dan interaktivitas  

Fungsi utamanya:
- Menyusun struktur konten web  
- Menghubungkan antarhalaman melalui hyperlink  
- Menyematkan media, formulir, dan elemen interaktif  
- Memudahkan integrasi dengan API dan aplikasi web modern

---

## 1.4 Struktur Dasar Dokumen HTML5
Setiap file HTML5 dimulai dengan deklarasi `<!DOCTYPE html>` yang memberitahu browser bahwa dokumen ini menggunakan standar HTML5.

```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Judul Halaman Saya</title>
</head>
<body>
  <h1>Selamat Datang di Dunia HTML5</h1>
  <p>Ini adalah halaman web pertama saya menggunakan HTML5.</p>
</body>
</html>
```

**Penjelasan singkat:**
| Bagian | Keterangan |
|---------|-------------|
| `<!DOCTYPE html>` | Menandakan dokumen menggunakan HTML5 |
| `<html>` | Elemen akar (root) dari seluruh dokumen |
| `<head>` | Menyimpan metadata, judul, link CSS, dll |
| `<body>` | Konten utama yang terlihat di browser |
| `<meta>` | Informasi tambahan untuk browser & SEO |
| `<title>` | Judul halaman yang tampil di tab browser |

---

## 1.5 Elemen HTML5
HTML5 memiliki ratusan elemen (tag), namun umumnya dikelompokkan menjadi:

| Kategori | Contoh Tag | Fungsi |
|-----------|-------------|--------|
| **Struktur** | `<header>`, `<nav>`, `<main>`, `<footer>` | Mengatur tata letak halaman |
| **Teks** | `<h1>–<h6>`, `<p>`, `<strong>`, `<em>` | Menampilkan teks & heading |
| **Media** | `<img>`, `<audio>`, `<video>` | Menyematkan gambar & media |
| **Formulir** | `<form>`, `<input>`, `<textarea>`, `<button>` | Input pengguna |
| **Tabel & Daftar** | `<table>`, `<ul>`, `<ol>`, `<li>` | Menyajikan data & list |
| **Semantik** | `<article>`, `<section>`, `<aside>`, `<figure>` | Struktur logis konten |
| **Interaktif/API** | `<canvas>`, `<details>`, `<dialog>` | Elemen dinamis dan interaktif |

---

## 1.6 Perbedaan HTML vs HTML5
| Aspek | HTML | HTML5 |
|--------|-------|-------|
| Versi | Lama (4.01) | Modern (final: 2014) |
| Multimedia | Butuh plugin (Flash) | Native `<audio>` & `<video>` |
| Struktur | `<div>` untuk semua | Elemen semantik baru |
| API | Tidak tersedia | Geolocation, Storage, Drag & Drop |
| Responsif | Belum ada | Atribut `viewport`, mobile-friendly |

---

## 1.7 Fitur Baru HTML5 yang Penting
1. **Tag Semantik Baru:**  
   `<header>`, `<footer>`, `<article>`, `<section>`, `<nav>`  
   → membantu SEO dan aksesibilitas.

2. **Multimedia Bawaan:**  
   Tag `<video>` dan `<audio>` memungkinkan streaming tanpa Flash.
   ```html
   <video controls width="300">
     <source src="video.mp4" type="video/mp4">
     Browser Anda tidak mendukung video tag.
   </video>
   ```

3. **Grafis & Visual:**  
   Tag `<canvas>` memungkinkan pembuatan grafik, animasi, dan game berbasis JavaScript.
   ```html
   <canvas id="kanvas" width="200" height="100"></canvas>
   ```

4. **Form Input Baru:**  
   Tipe input tambahan seperti `email`, `date`, `color`, `range`.
   ```html
   <input type="email" placeholder="Masukkan email" required>
   ```

5. **Web Storage API:**  
   Menyimpan data di browser tanpa cookie (melalui `localStorage` & `sessionStorage`).

6. **Geolocation API:**  
   Menentukan lokasi pengguna untuk layanan berbasis lokasi (maps, tracking, dll).

---

## 1.8 Contoh Sederhana Halaman HTML5 Lengkap
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Contoh Halaman HTML5</title>
</head>
<body>
  <header>
    <h1>Website Saya</h1>
    <nav>
      <a href="#">Beranda</a> |
      <a href="#">Tentang</a> |
      <a href="#">Kontak</a>
    </nav>
  </header>

  <main>
    <article>
      <h2>Artikel Utama</h2>
      <p>HTML5 membuat pengembangan web lebih mudah dan terstruktur.</p>
    </article>

    <aside>
      <h3>Sidebar</h3>
      <p>Ini area tambahan seperti menu atau iklan.</p>
    </aside>
  </main>

  <footer>
    <p>&copy; 2025 Mulyo Anjang Jaya Kusuma</p>
  </footer>
</body>
</html>
```

---

## 1.9 Validasi & Praktik Baik
✅ Gunakan `<!DOCTYPE html>` di baris pertama.  
✅ Pastikan tag ditutup dengan benar.  
✅ Gunakan atribut `lang` pada `<html>`.  
✅ Gunakan **tag semantik** daripada `<div>` berlebihan.  
✅ Validasi kode di [https://validator.w3.org](https://validator.w3.org).  

---

## 1.10 Kesimpulan
HTML5 adalah **evolusi besar** dari HTML yang membawa web ke arah **lebih terbuka, interaktif, dan mudah diakses.**  
Setelah memahami dasar HTML5, kamu siap lanjut ke **Bab 2 – Struktur Dokumen HTML5**, untuk membahas bagian `<head>`, `<meta>`, `<link>`, dan `<body>` secara mendalam.

---

<div align="left">

🔗 [← Kembali ke Daftar Materi](../README.md)

</div>
<div align="right">

🔗 [Lanjut ke Bab 2 → Struktur Dokumen HTML5](../materi-html/02-struktur-dokumen-html5.md)

</div>
