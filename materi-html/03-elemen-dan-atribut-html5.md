# 🧩 BAB 3 — Elemen dan Atribut HTML5

## 3.1 Pengantar
HTML dibangun dari **elemen** dan **atribut**.  
- Elemen adalah blok penyusun halaman web.  
- Atribut memberikan informasi tambahan untuk elemen tersebut.

> 🧠 “Setiap bagian di HTML memiliki tujuan spesifik — pahami elemennya, maka kamu memahami struktur web.”

---

## 3.2 Elemen HTML
Elemen HTML terdiri dari:
```html
<tagname>konten</tagname>
```

Contoh:
```html
<p>Ini paragraf</p>
<h1>Judul Besar</h1>
```

### Jenis Elemen
| Jenis | Contoh | Deskripsi |
|--------|---------|-----------|
| **Block-level** | `<div>`, `<p>`, `<section>` | Menempati seluruh lebar halaman |
| **Inline** | `<span>`, `<a>`, `<strong>` | Hanya selebar konten |

---

## 3.3 Elemen Umum HTML5
| Elemen | Fungsi | Contoh |
|--------|---------|--------|
| `<h1>`–`<h6>` | Judul dari besar ke kecil | `<h2>Subjudul</h2>` |
| `<p>` | Paragraf | `<p>Teks paragraf</p>` |
| `<a>` | Hyperlink | `<a href="#">Klik di sini</a>` |
| `<img>` | Gambar | `<img src="foto.jpg" alt="Deskripsi" />` |
| `<ul>` / `<ol>` | Daftar | `<ul><li>Item</li></ul>` |
| `<table>` | Tabel | `<table><tr><td>Data</td></tr></table>` |

---

## 3.4 Atribut HTML
Atribut digunakan di dalam tag pembuka untuk memberikan informasi tambahan.

### Contoh:
```html
<a href="https://example.com" target="_blank" title="Buka tautan baru">
  Kunjungi Situs
</a>
```

| Atribut | Fungsi |
|----------|--------|
| `href` | Alamat tujuan tautan |
| `target` | Cara membuka tautan (`_self`, `_blank`) |
| `title` | Tooltip saat diarahkan kursor |
| `alt` | Deskripsi teks alternatif untuk gambar |

---

## 3.5 Atribut Global (Universal)
Semua elemen HTML5 bisa memakai atribut global berikut:

| Atribut | Deskripsi |
|----------|------------|
| `id` | Identitas unik elemen |
| `class` | Mengelompokkan elemen |
| `style` | Menambahkan CSS inline |
| `title` | Keterangan tambahan |
| `lang` | Bahasa konten |
| `hidden` | Menyembunyikan elemen |
| `draggable` | Menentukan apakah elemen bisa diseret |
| `contenteditable` | Mengizinkan elemen diedit langsung di browser |

### Contoh:
```html
<p id="paragraf1" class="info" style="color:blue;" title="Paragraf Informasi">
  Ini adalah paragraf dengan atribut global.
</p>
```

---

## 3.6 Atribut Boolean
Atribut **boolean** tidak memerlukan nilai (cukup ditulis saja).

| Atribut | Fungsi | Contoh |
|----------|--------|--------|
| `disabled` | Menonaktifkan elemen input | `<input type="text" disabled>` |
| `checked` | Menandai checkbox aktif | `<input type="checkbox" checked>` |
| `readonly` | Tidak bisa diubah | `<input type="text" readonly>` |
| `required` | Wajib diisi | `<input type="email" required>` |
| `autoplay` | Memainkan media otomatis | `<video autoplay>` |

---

## 3.7 Atribut Khusus HTML5
Beberapa atribut baru muncul di HTML5 untuk mendukung fitur modern:
| Atribut | Elemen | Fungsi |
|----------|---------|--------|
| `placeholder` | `<input>` | Menampilkan teks petunjuk |
| `autofocus` | `<input>` | Fokus otomatis saat halaman dibuka |
| `controls` | `<audio>`, `<video>` | Menampilkan kontrol media |
| `srcset` | `<img>` | Mendukung gambar responsif |
| `download` | `<a>` | Memaksa unduhan file |

Contoh:
```html
<a href="ebook.pdf" download>Unduh Ebook</a>
<img src="foto.jpg" srcset="foto@2x.jpg 2x" alt="Foto resolusi tinggi" />
```

---

## 3.8 Contoh Lengkap Elemen + Atribut
```html
<article id="post1" class="artikel" lang="id">
  <h2>Belajar HTML5</h2>
  <p>HTML5 memperkenalkan banyak elemen dan atribut baru.</p>
  <img src="gambar.jpg" alt="Gambar HTML5" width="300" draggable="true" />
  <a href="https://validator.w3.org" target="_blank" title="Validasi HTML5">Validasi di W3C</a>
</article>
```

---

## 3.9 Kesalahan Umum pada Atribut
🚫 **Menulis atribut tanpa tanda kutip:**
```html
<a href=https://google.com>Google</a>
```
✅ **Gunakan tanda kutip ganda atau tunggal:**
```html
<a href="https://google.com">Google</a>
```

---

## 3.10 Kesimpulan
Elemen dan atribut adalah **fondasi inti HTML5.**  
Mengetahui perbedaan block/inline dan penggunaan atribut global membuat struktur web lebih efisien, mudah dibaca, dan mudah diatur dengan CSS/JavaScript.

---

<div align="left">

🔗 [← Kembali ke Bab 2: Struktur Dokumen HTML5](../materi-html/02-struktur-dokumen-html5.md)

</div>
<div align="right">

🔗 [Lanjut ke Bab 4 → Teks dan Formatting Modern](../materi-html/04-teks-dan-formatting.md)

</div>
