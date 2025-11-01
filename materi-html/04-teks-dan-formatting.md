# ✍️ BAB 4 — Teks dan Formatting Modern

## 4.1 Pengantar
Teks adalah elemen paling dasar dalam HTML5.  
Pengaturan teks yang baik membantu meningkatkan **keterbacaan, struktur konten, dan pengalaman pengguna**.

HTML5 menyediakan berbagai tag untuk memberi **makna semantik** terhadap teks — bukan hanya tampilan visual.

> 💡 “Gunakan tag berdasarkan makna, bukan hanya untuk gaya.”

---

## 4.2 Heading (Judul)
HTML memiliki **enam tingkat heading**: `<h1>` hingga `<h6>`  
Gunakan berurutan untuk struktur yang logis.

```html
<h1>Judul Utama</h1>
<h2>Subjudul</h2>
<h3>Sub-subjudul</h3>
```

| Tag | Fungsi | Catatan |
|------|--------|----------|
| `<h1>` | Judul utama halaman | Gunakan hanya 1x per halaman |
| `<h2>`–`<h6>` | Subjudul hierarkis | Dapat digunakan berulang |

---

## 4.3 Paragraf dan Pemisah
```html
<p>Ini adalah sebuah paragraf. HTML secara otomatis memberi jarak antar paragraf.</p>
<p>Setiap paragraf baru dibuat dengan tag &lt;p&gt;.</p>
<hr />
```

| Tag | Fungsi |
|------|--------|
| `<p>` | Membuat paragraf |
| `<br>` | Ganti baris tanpa jarak |
| `<hr>` | Garis pemisah antar bagian |

---

## 4.4 Penekanan dan Gaya Teks
HTML5 menyediakan elemen semantik untuk memperjelas arti teks.

| Tag | Arti Semantik | Contoh |
|------|----------------|--------|
| `<strong>` | Penting / penekanan kuat | `<strong>Wajib diisi</strong>` |
| `<em>` | Penekanan ringan (miring) | `<em>Perhatikan ini</em>` |
| `<b>` | Tebal (tanpa arti semantik) | `<b>Bold</b>` |
| `<i>` | Miring (tanpa arti semantik) | `<i>Italic</i>` |
| `<u>` | Garis bawah | `<u>Teks digarisbawahi</u>` |
| `<mark>` | Sorotan / highlight | `<mark>Penting</mark>` |
| `<small>` | Teks kecil | `<small>Catatan</small>` |
| `<del>` / `<ins>` | Dihapus / ditambahkan | `<del>Harga lama</del> <ins>Harga baru</ins>` |

---

## 4.5 Kutipan dan Referensi
```html
<blockquote cite="https://www.example.com/artikel">
  “HTML5 membawa struktur yang lebih jelas dan bermakna.”
</blockquote>

<p>Kata <q>markup</q> berarti tanda atau struktur teks.</p>
```

| Tag | Fungsi |
|------|--------|
| `<blockquote>` | Kutipan panjang (blok) |
| `<q>` | Kutipan pendek (dalam paragraf) |
| `cite` | Atribut untuk sumber kutipan |

---

## 4.6 Superscript & Subscript
```html
<p>H<sub>2</sub>O = air</p>
<p>E = mc<sup>2</sup></p>
```

| Tag | Fungsi |
|------|--------|
| `<sub>` | Subskrip (di bawah) |
| `<sup>` | Superskrip (di atas) |

---

## 4.7 Preformatted & Code
Gunakan `<pre>` untuk teks dengan format tetap, dan `<code>` untuk menampilkan kode program.

```html
<pre>
for (let i = 0; i < 5; i++) {
  console.log("Halo");
}
</pre>

<p>Contoh fungsi di <code>JavaScript</code>.</p>
```

| Tag | Fungsi |
|------|--------|
| `<pre>` | Menjaga spasi & baris |
| `<code>` | Menandai potongan kode |

---

## 4.8 Elemen Inline vs Block
| Jenis | Contoh Tag | Ciri |
|--------|-------------|------|
| **Block** | `<p>`, `<div>`, `<article>` | Membuat blok baru |
| **Inline** | `<a>`, `<span>`, `<em>` | Mengalir di dalam teks |

Contoh:
```html
<p>Teks <span style="color:red;">berwarna merah</span> di paragraf.</p>
```

---

## 4.9 Kesimpulan
HTML5 menyediakan elemen semantik untuk **mengomunikasikan makna teks**, bukan sekadar tampilan.  
Dengan struktur teks yang baik, konten akan lebih mudah dipahami manusia dan mesin pencari.

---

<div align="left">

🔗 [← Kembali ke Bab 3: Elemen dan Atribut HTML5](../materi-html/03-elemen-dan-atribut-html5.md)

</div>
<div align="right">

🔗 [Lanjut ke Bab 5 → Link, Gambar, Audio, dan Video](../materi-html/05-link-dan-media.md)

</div>
