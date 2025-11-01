# 🧩 BAB 8 — Elemen Semantik HTML5

## 8.1 Pengantar
HTML5 memperkenalkan **elemen semantik** untuk memberi makna pada struktur halaman web.  
Berbeda dari `<div>` generik, elemen semantik memberi tahu browser, mesin pencari, dan pembaca layar **fungsi sebenarnya dari sebuah bagian konten.**

> 💡 “Semantik membantu manusia dan mesin memahami struktur web tanpa harus menebak.”

---

## 8.2 Apa Itu Elemen Semantik?
Elemen **semantik** = elemen yang memiliki arti kontekstual terhadap isi di dalamnya.  
Contoh:
```html
<header>...</header>
<article>...</article>
<footer>...</footer>
```

Sedangkan elemen **non-semantik** seperti `<div>` dan `<span>` tidak menjelaskan makna apapun.

---

## 8.3 Daftar Elemen Semantik HTML5
| Elemen | Fungsi | Contoh Penggunaan |
|--------|---------|------------------|
| `<header>` | Bagian atas halaman atau artikel | Judul, logo, menu |
| `<nav>` | Navigasi utama situs | Link menu |
| `<main>` | Konten utama halaman | Artikel utama |
| `<section>` | Bagian tematik dalam halaman | Bab, blok konten |
| `<article>` | Konten mandiri | Artikel berita, posting blog |
| `<aside>` | Informasi tambahan | Sidebar, catatan |
| `<footer>` | Bagian bawah halaman | Hak cipta, tautan sosmed |
| `<figure>` | Media + deskripsi | Gambar, grafik, video |
| `<figcaption>` | Keterangan pada figure | Teks penjelas gambar |
| `<time>` | Menunjukkan waktu/tanggal | `<time datetime="2025-11-02">2 Nov 2025</time>` |
| `<mark>` | Penyorotan teks penting | `<mark>Penting</mark>` |

---

## 8.4 Contoh Struktur Semantik Lengkap
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Contoh Struktur Semantik</title>
</head>
<body>
  <header>
    <h1>Belajar HTML5 Semantik</h1>
    <nav>
      <a href="#">Beranda</a> | <a href="#">Artikel</a> | <a href="#">Kontak</a>
    </nav>
  </header>

  <main>
    <article>
      <h2>Manfaat Elemen Semantik</h2>
      <p>Semantik membantu SEO dan aksesibilitas.</p>
      <figure>
        <img src="struktur.png" alt="Struktur Semantik">
        <figcaption>Struktur Semantik HTML5</figcaption>
      </figure>
    </article>

    <aside>
      <h3>Catatan Tambahan</h3>
      <p>Gunakan tag sesuai maknanya, bukan untuk styling.</p>
    </aside>
  </main>

  <footer>
    <p>&copy; 2025 Belajar HTML5 — Semua Hak Dilindungi.</p>
  </footer>
</body>
</html>
```

---

## 8.5 Manfaat Elemen Semantik
✅ **SEO Friendly** — mesin pencari lebih mudah memahami struktur halaman  
✅ **Aksesibilitas** — pembaca layar dapat mengenali bagian halaman  
✅ **Keterbacaan kode** — lebih mudah dipahami dan dipelihara  
✅ **Standar modern** — sesuai pedoman W3C  

---

## 8.6 Tips Penggunaan Semantik
| Kebutuhan | Gunakan Elemen |
|-------------|----------------|
| Judul halaman | `<header>` |
| Navigasi utama | `<nav>` |
| Isi utama | `<main>` |
| Artikel berita / post | `<article>` |
| Seksi bagian konten | `<section>` |
| Sidebar / catatan | `<aside>` |
| Hak cipta | `<footer>` |

---

## 8.7 Kesalahan Umum
🚫 Menggunakan `<div>` untuk semua bagian (anti-pattern)  
✅ Ganti `<div class="header">` → `<header>`  
✅ Ganti `<div class="footer">` → `<footer>`  

---

## 8.8 Kesimpulan
Elemen semantik membuat web lebih bermakna, mudah dibaca, dan terindeks dengan baik.  
Gunakan elemen sesuai konteks untuk menciptakan struktur HTML5 yang profesional dan efisien.

---

<div align="left">

🔗 [← Kembali ke Bab 7: Formulir dan Input HTML5](../materi-html/07-formulir-dan-input.md)

</div>
<div align="right">

🔗 [Lanjut ke Bab 9 → Meta Tag, SEO, dan Aksesibilitas](../materi-html/09-meta-tag-dan-seo.md)

</div>
