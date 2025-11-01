# 🧾 BAB 11 — Rangkuman Tag HTML5 & Fungsinya

> Ringkasan cepat elemen-elemen HTML5 yang paling sering dipakai, beserta fungsi dan contoh minimumnya.

## 11.1 Struktur Dokumen
| Tag | Fungsi | Contoh Minimum |
|-----|--------|----------------|
| `<!DOCTYPE html>` | Deklarasi dokumen HTML5 | `<!DOCTYPE html>` |
| `<html lang="id">` | Elemen akar + bahasa | `<html lang="id">…</html>` |
| `<head>` | Metadata (tidak tampil) | `<head>…</head>` |
| `<meta charset="UTF-8">` | Encoding karakter | `<meta charset="UTF-8">` |
| `<meta name="viewport">` | Responsif mobile | `<meta name="viewport" content="width=device-width, initial-scale=1.0">` |
| `<title>` | Judul tab browser | `<title>Judul</title>` |
| `<link>` | Tautan eksternal (ikon, CSS) | `<link rel="icon" href="favicon.ico">` |
| `<script>` | JavaScript | `<script src="app.js"></script>` |
| `<body>` | Konten yang ditampilkan | `<body>…</body>` |

## 11.2 Teks & Tipografi
| Tag | Fungsi | Contoh |
|-----|--------|--------|
| `<h1>`–`<h6>` | Heading hierarkis | `<h1>Judul</h1>` |
| `<p>` | Paragraf | `<p>Teks…</p>` |
| `<br>` | Ganti baris | `Baris 1<br>Baris 2` |
| `<hr>` | Pemisah bagian | `<hr>` |
| `<strong>` / `<em>` | Penekanan (tebal/miring, semantik) | `<strong>Penting</strong>` |
| `<b>` / `<i>` | Tebal/miring (non-semantik) | `<b>Bold</b>` |
| `<u>` | Garis bawah | `<u>teks</u>` |
| `<mark>` | Sorotan | `<mark>highlight</mark>` |
| `<small>` | Teks kecil | `<small>catatan</small>` |
| `<sup>` / `<sub>` | Super/subskrip | `x<sup>2</sup>, H<sub>2</sub>O` |
| `<blockquote>` / `<q>` | Kutipan blok/inline | `<blockquote>…</blockquote>` |
| `<code>` / `<pre>` | Kode & teks pramuat | `<pre><code>for…</code></pre>` |
| `<abbr>` | Singkatan (tooltip) | `<abbr title="HyperText Markup Language">HTML</abbr>` |

## 11.3 Link, Media & Gambar
| Tag | Fungsi | Contoh |
|-----|--------|--------|
| `<a>` | Hyperlink/unduh | `<a href="file.pdf" download>Unduh</a>` |
| `<img>` | Gambar + `alt` | `<img src="x.jpg" alt="Deskripsi">` |
| `srcset` | Gambar responsif | `<img src="x.jpg" srcset="x2.jpg 2x">` |
| `<figure>` / `<figcaption>` | Media + keterangan | `<figure>…<figcaption>…</figcaption></figure>` |
| `<audio>` | Audio native | `<audio controls><source src="x.mp3"></audio>` |
| `<video>` | Video native | `<video controls poster="t.jpg"><source src="x.mp4"></video>` |
| `<iframe>` | Sematkan konten (YT/Maps) | `<iframe src="…"></iframe>` |

## 11.4 Daftar & Tabel
| Tag | Fungsi | Contoh |
|-----|--------|--------|
| `<ul>` / `<ol>` | Daftar tak/berurutan | `<ul><li>Item</li></ul>` |
| `<li>` | Item daftar | `<li>Item</li>` |
| `<dl>` `<dt>` `<dd>` | Glosarium/definisi | `<dl><dt>HTML</dt><dd>…</dd></dl>` |
| `<table>` | Tabel | `<table>…</table>` |
| `<tr>` `<th>` `<td>` | Baris/header/sel | `<tr><th>A</th><td>B</td></tr>` |
| `<thead>` `<tbody>` `<tfoot>` | Struktur tabel | `<thead>…</thead>` |

## 11.5 Formulir & Input Modern
| Tag / Atribut | Fungsi | Contoh |
|---------------|--------|--------|
| `<form action method>` | Wadah input | `<form action="/send" method="POST">` |
| `<label for>` | Label aksesibel | `<label for="email">Email</label>` |
| `<input type="…">` | Input umum | `text, email, password, number, date, color, range, file, url, tel, search` |
| Atribut input | Validasi/UX | `required, min, max, step, pattern, placeholder, autofocus, readonly, disabled` |
| `<textarea>` | Teks panjang | `<textarea rows="4"></textarea>` |
| `<select><option>` | Dropdown | `<select><option>Opsi</option></select>` |
| `<fieldset><legend>` | Kelompok field | `<fieldset><legend>Data</legend>…</fieldset>` |
| `<datalist>` | Saran otomatis | `<input list="opt"><datalist id="opt">…</datalist>` |
| `<button type="submit">` | Tombol kirim | `<button type="submit">Kirim</button>` |

## 11.6 Elemen Semantik Struktur
| Tag | Fungsi | Contoh |
|-----|--------|--------|
| `<header>` | Kepala halaman/section | `<header>Logo+Nav</header>` |
| `<nav>` | Navigasi utama | `<nav><a>…</a></nav>` |
| `<main>` | Konten utama | `<main>…</main>` |
| `<section>` | Bagian tematik | `<section id="about">…</section>` |
| `<article>` | Konten mandiri | `<article>Blog Post</article>` |
| `<aside>` | Info samping | `<aside>Sidebar</aside>` |
| `<footer>` | Kaki halaman | `<footer>©</footer>` |
| `<time datetime>` | Waktu/ISO | `<time datetime="2025-11-02">2 Nov 2025</time>` |
| `<details><summary>` | Konten collapsible | `<details><summary>Lihat</summary>…</details>` |
| `<dialog open>` | Dialog native | `<dialog open>Halo</dialog>` |

## 11.7 Atribut Global Penting
`id`, `class`, `style`, `title`, `lang`, `hidden`, `tabindex`, `draggable`, `contenteditable`, `aria-*`

**Contoh aksesibilitas:**
```html
<button aria-label="Buka menu">☰</button>
<img src="foto.jpg" alt="Foto profil Mulyo" />
<nav aria-label="Navigasi utama">…</nav>
```

## 11.8 Pola Umum yang Baik
- Satu `<h1>` per halaman, gunakan `<h2>–<h6>` berurutan.
- Gambar wajib memiliki `alt`.
- Gunakan elemen semantik daripada `<div>` generik.
- Validasi di https://validator.w3.org
- Tambahkan `<meta name="viewport">` untuk mobile.
