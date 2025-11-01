# 🧱 BAB 2 — Struktur Dokumen HTML5

## 2.1 Pengantar
Struktur dokumen HTML5 menentukan bagaimana browser membaca, menafsirkan, dan menampilkan halaman web.  
HTML5 memiliki format **hierarkis**, dimulai dari deklarasi dokumen hingga isi halaman utama.

> 🎯 Tujuan bab ini: memahami anatomi file HTML5 dan fungsi setiap bagiannya.

---

## 2.2 Anatomi Dasar Dokumen HTML5
Setiap file HTML5 memiliki kerangka umum seperti ini:

```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Judul Halaman</title>
</head>
<body>
  <h1>Konten Utama</h1>
</body>
</html>
```

### Penjelasan:
| Bagian | Fungsi |
|---------|--------|
| `<!DOCTYPE html>` | Mendeklarasikan bahwa ini adalah dokumen HTML5 |
| `<html>` | Elemen akar dari seluruh halaman |
| `<head>` | Menyimpan metadata (tidak tampil di layar) |
| `<body>` | Menyimpan konten utama yang terlihat pengguna |

---

## 2.3 Bagian `<head>` — Informasi Halaman
Elemen `<head>` berisi **metadata**, seperti:
- judul halaman (`<title>`)
- pengaturan tampilan (`<meta>`)
- link ke CSS atau ikon
- deskripsi SEO

### Contoh:
```html
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Belajar dasar HTML5 secara lengkap" />
  <title>Belajar HTML5</title>
  <link rel="stylesheet" href="style.css" />
  <link rel="icon" href="favicon.ico" type="image/x-icon" />
</head>
```

### Penjelasan meta penting:
| Tag | Fungsi |
|------|--------|
| `<meta charset="UTF-8">` | Menentukan encoding karakter agar mendukung semua bahasa |
| `<meta name="viewport">` | Membuat halaman responsif di perangkat mobile |
| `<meta name="description">` | Deskripsi singkat untuk SEO |
| `<link rel="icon">` | Menentukan ikon tab browser (favicon) |

---

## 2.4 Bagian `<body>` — Konten Utama
Semua yang terlihat di halaman berada dalam `<body>`, termasuk:
- teks
- gambar
- tautan
- video
- form
- struktur layout (header, nav, footer, dll)

### Contoh:
```html
<body>
  <header>
    <h1>Website Belajar HTML5</h1>
  </header>
  <main>
    <section>
      <p>HTML5 memperkenalkan struktur dokumen yang lebih jelas dan semantik.</p>
    </section>
  </main>
  <footer>
    <p>© 2025 Mulyo Anjang Jaya Kusuma</p>
  </footer>
</body>
```

---

## 2.5 Elemen Semantik dalam Struktur Dokumen
HTML5 memperkenalkan tag semantik agar struktur halaman lebih jelas:
| Elemen | Fungsi |
|--------|--------|
| `<header>` | Bagian kepala (judul/navigasi) |
| `<nav>` | Navigasi utama |
| `<main>` | Konten utama halaman |
| `<section>` | Bagian dari isi utama |
| `<article>` | Konten independen (berita/artikel) |
| `<aside>` | Konten sampingan |
| `<footer>` | Bagian bawah halaman |

---

## 2.6 Template Lengkap Dokumen HTML5
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Contoh struktur HTML5 lengkap" />
  <title>Struktur HTML5 Lengkap</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Judul Website</h1>
  </header>
  <nav>
    <a href="#">Beranda</a> | <a href="#">Artikel</a> | <a href="#">Kontak</a>
  </nav>
  <main>
    <article>
      <h2>Artikel Utama</h2>
      <p>Ini adalah isi artikel yang menjelaskan tentang struktur HTML5.</p>
    </article>
    <aside>
      <h3>Sidebar</h3>
      <p>Menu tambahan di samping.</p>
    </aside>
  </main>
  <footer>
    <p>© 2025 Belajar HTML5</p>
  </footer>
</body>
</html>
```

---

## 2.7 Kesimpulan
Struktur HTML5 kini lebih **teratur dan bermakna** dengan dukungan elemen semantik.  
Penggunaan struktur yang benar memudahkan SEO, pembaca layar, dan kolaborasi antar developer.

---

<div align="left">

🔗 [← Kembali ke Bab 1: Pengenalan HTML5](../materi-html/01-pengenalan-html5.md)

</div>
<div align="right">

🔗 [Lanjut ke Bab 3 → Elemen dan Atribut HTML5](../materi-html/03-elemen-dan-atribut-html5.md)

</div>
