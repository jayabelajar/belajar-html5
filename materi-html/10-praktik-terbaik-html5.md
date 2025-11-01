# ✅ BAB 10 — Praktik Terbaik Penulisan HTML5

## 10.1 Pengantar
Setelah memahami seluruh elemen dan struktur HTML5, langkah terakhir adalah menerapkan **best practices (praktik terbaik)** agar kode yang dibuat:
- Mudah dibaca dan dipelihara
- Sesuai standar W3C
- SEO dan aksesibilitas optimal
- Siap diintegrasikan dengan CSS & JavaScript modern

---

## 10.2 Prinsip Umum Penulisan HTML5
| Aspek | Praktik Terbaik |
|--------|----------------|
| Struktur | Gunakan elemen semantik sesuai fungsinya |
| Penulisan | Gunakan indentasi konsisten (2–4 spasi) |
| Nama file | Gunakan huruf kecil dan tanda hubung (`about-us.html`) |
| Komentar | Tambahkan komentar seperlunya (`<!-- Menu Utama -->`) |
| Konsistensi | Gunakan huruf kecil untuk tag dan atribut |
| Validasi | Selalu cek di [validator.w3.org](https://validator.w3.org) |

---

## 10.3 Hindari Kesalahan Umum
🚫 Tidak menutup tag:  
```html
<p>Paragraf tidak tertutup
```

✅ Harus:
```html
<p>Paragraf benar.</p>
```

🚫 Menggunakan `<br>` berlebihan untuk jarak  
✅ Gunakan CSS `margin` atau `padding`

🚫 Menggunakan tabel untuk layout  
✅ Gunakan Flexbox atau Grid CSS

---

## 10.4 Struktur Folder yang Baik untuk Proyek HTML5
```
my-website/
├─ index.html
├─ about.html
├─ contact.html
├─ assets/
│  ├─ css/
│  │  └─ style.css
│  ├─ js/
│  │  └─ script.js
│  └─ images/
│     └─ banner.jpg
└─ README.md
```
> 🧩 Pisahkan file HTML, CSS, JS, dan gambar dalam folder yang jelas untuk memudahkan pengelolaan.

---

## 10.5 Konvensi Penulisan Tag dan Atribut
✅ Gunakan huruf kecil untuk tag dan atribut.  
✅ Gunakan tanda kutip ganda untuk nilai atribut.  
✅ Gunakan indentasi untuk struktur bersarang.

Contoh baik:
```html
<section class="hero">
  <h1>Selamat Datang</h1>
  <p>Belajar HTML5 dengan struktur modern.</p>
</section>
```

---

## 10.6 Optimasi Performa HTML5
| Strategi | Penjelasan |
|-----------|------------|
| Gunakan gambar terkompresi | WebP atau JPEG optimasi |
| Gunakan `loading="lazy"` pada gambar | Menunda pemuatan gambar |
| Letakkan skrip di akhir `<body>` | Menghindari blocking render |
| Gunakan CDN untuk library besar | Akses cepat dan efisien |
| Tambahkan caching header | Meningkatkan kecepatan akses |

---

## 10.7 Responsivitas
Gunakan meta viewport dan desain fleksibel.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

Gunakan unit persentase, `vw`, atau `em` agar tampilan responsif.

---

## 10.8 Aksesibilitas dan SEO
✅ Gunakan `alt` pada setiap gambar  
✅ Gunakan heading berurutan `<h1>–<h6>`  
✅ Gunakan `<main>` untuk konten utama  
✅ Gunakan atribut `lang="id"` di tag `<html>`  
✅ Hindari teks hanya bergantung warna  

---

## 10.9 Template HTML5 Siap Produksi
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Template HTML5 responsif modern">
  <title>Judul Halaman</title>
  <link rel="stylesheet" href="assets/css/style.css">
</head>
<body>
  <header>
    <h1>Logo & Judul Website</h1>
    <nav>
      <a href="#">Beranda</a> | <a href="#">Tentang</a> | <a href="#">Kontak</a>
    </nav>
  </header>

  <main>
    <section>
      <h2>Selamat Datang!</h2>
      <p>Ini adalah contoh template HTML5 siap produksi.</p>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Belajar HTML5 — Dibuat oleh Mulyo Anjang Jaya Kusuma</p>
  </footer>
</body>
</html>
```

---

## 10.10 Kesimpulan
HTML5 bukan hanya bahasa markup, tapi juga **kerangka berpikir logis** dalam membangun web yang modern, efisien, dan mudah diakses.  
Gunakan elemen secara bermakna, validasi kode secara rutin, dan terapkan praktik terbaik agar hasilmu layak produksi profesional.

---

<div align="left">

🔗 [← Kembali ke Bab 9: Meta Tag dan SEO](../materi-html/09-meta-tag-dan-seo.md)

</div>
<div align="right">

🔗 [Lanjut ke Lampiran → Contoh & Glosarium HTML5](../materi-html/lampiran-contoh-html.md)

</div>
