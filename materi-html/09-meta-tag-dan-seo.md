# ⚙️ BAB 9 — Meta Tag, SEO, dan Aksesibilitas

## 9.1 Pengantar
HTML5 tidak hanya tentang tampilan, tapi juga tentang **bagaimana mesin pencari dan pengguna memahami halaman web.**  
Dengan penggunaan **meta tag, atribut semantik, dan aksesibilitas (a11y)** yang baik, website menjadi lebih mudah ditemukan dan digunakan.

---

## 9.2 Apa Itu Meta Tag?
Meta tag adalah elemen dalam `<head>` yang menyimpan **informasi (metadata)** tentang halaman.  
Tidak ditampilkan di layar, tapi dibaca oleh **browser, mesin pencari, dan sosial media crawler.**

---

## 9.3 Meta Tag Umum HTML5
```html
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<meta name="description" content="Panduan lengkap belajar HTML5 dari dasar hingga mahir." />
<meta name="keywords" content="HTML5, belajar html, web development" />
<meta name="author" content="Mulyo Anjang Jaya Kusuma" />
<title>Belajar HTML5</title>
```

| Tag | Fungsi |
|------|--------|
| `charset` | Menentukan karakter encoding (UTF-8 disarankan) |
| `viewport` | Mengatur tampilan responsif di mobile |
| `description` | Deskripsi halaman (penting untuk SEO) |
| `keywords` | Kata kunci pencarian (kurang relevan modern) |
| `author` | Nama pembuat halaman |
| `robots` | Instruksi untuk bot mesin pencari |

---

## 9.4 Meta Tag Media Sosial (Open Graph & Twitter)
Agar halaman tampil menarik saat dibagikan di sosial media.

```html
<!-- Open Graph (Facebook, LinkedIn, dll) -->
<meta property="og:title" content="Belajar HTML5 Modern" />
<meta property="og:description" content="Pelajari HTML5 dari dasar dengan contoh praktis dan struktur semantik." />
<meta property="og:image" content="https://example.com/html5.png" />
<meta property="og:url" content="https://example.com" />
<meta property="og:type" content="website" />

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image" />
<meta name="twitter:title" content="Belajar HTML5 Modern" />
<meta name="twitter:description" content="Pelajari HTML5 dari dasar dengan contoh praktis dan struktur semantik." />
<meta name="twitter:image" content="https://example.com/html5.png" />
```

---

## 9.5 SEO (Search Engine Optimization)
HTML5 mendukung praktik SEO melalui:
1. **Tag Semantik:** gunakan `<header>`, `<main>`, `<footer>`, `<article>`, `<section>`  
2. **Struktur Heading:** `<h1>` untuk judul utama, `<h2>`–`<h6>` untuk subjudul  
3. **Alt Text:** selalu tambahkan `alt` pada gambar  
4. **Deskripsi & Title yang jelas**  
5. **Gunakan URL bersih dan relevan**

---

## 9.6 Aksesibilitas (Accessibility / a11y)
Aksesibilitas berarti **semua orang, termasuk disabilitas, dapat menggunakan web.**

### Tips Aksesibilitas HTML5:
| Teknik | Tujuan |
|---------|---------|
| Gunakan tag semantik | Membantu pembaca layar mengenali struktur |
| Tambahkan `alt` di `<img>` | Menjelaskan gambar |
| Gunakan label `<label for>` | Menghubungkan label dengan input |
| Gunakan atribut `aria-` | Memberi informasi tambahan bagi screen reader |
| Gunakan kontras warna yang baik | Membaca teks lebih mudah |

Contoh penggunaan ARIA:
```html
<button aria-label="Tutup Menu">✖</button>
```

---

## 9.7 Contoh Head SEO Friendly
```html
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Panduan belajar HTML5 lengkap untuk pemula dan profesional.">
  <meta name="author" content="Mulyo Anjang Jaya Kusuma">
  <title>Belajar HTML5 Lengkap</title>

  <meta property="og:title" content="Belajar HTML5 Lengkap">
  <meta property="og:description" content="Panduan interaktif dan mudah dipahami.">
  <meta property="og:image" content="https://example.com/html5-banner.jpg">
  <meta property="og:type" content="website">
</head>
```

---

## 9.8 Kesalahan Umum
🚫 Tidak menulis meta viewport → tampilan mobile rusak  
🚫 Tidak menulis alt pada gambar → tidak ramah screen reader  
🚫 Menggunakan banyak `<h1>` dalam satu halaman  
🚫 Mengabaikan struktur semantik dan heading hierarchy  

---

## 9.9 Kesimpulan
Meta tag, semantik, dan aksesibilitas adalah **fondasi web modern yang SEO-friendly dan inklusif**.  
HTML5 bukan hanya untuk tampilan, tapi juga untuk **makna dan pengalaman pengguna.**

---

<div align="left">

🔗 [← Kembali ke Bab 8: Elemen Semantik HTML5](../materi-html/08-elemen-semantik-html5.md)

</div>
<div align="right">

🔗 [Lanjut ke Bab 10 → Praktik Terbaik HTML5](../materi-html/10-praktik-terbaik-html5.md)

</div>
