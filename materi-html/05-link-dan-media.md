# 🌐 BAB 5 — Link, Gambar, Audio, dan Video

## 5.1 Pengantar
HTML5 memungkinkan halaman web menampilkan **media interaktif dan terhubung antarhalaman** dengan mudah.  
Bab ini membahas **tautan (link)**, **gambar**, dan **multimedia (audio & video)** secara lengkap.

---

## 5.2 Hyperlink (`<a>`)
Hyperlink menghubungkan satu halaman ke halaman lain atau ke file eksternal.

```html
<a href="https://www.google.com" target="_blank" title="Buka Google">Kunjungi Google</a>
```

| Atribut | Fungsi |
|----------|--------|
| `href` | Alamat tujuan link |
| `target` | Cara membuka link (`_self`, `_blank`, `_parent`, `_top`) |
| `title` | Teks tooltip saat diarahkan kursor |
| `download` | Memaksa browser mengunduh file |

Contoh link unduhan:
```html
<a href="dokumen.pdf" download>Unduh File PDF</a>
```

---

## 5.3 Link Internal dan Eksternal
| Jenis | Contoh | Keterangan |
|--------|---------|------------|
| **Internal** | `<a href="about.html">Tentang</a>` | Menuju halaman di situs yang sama |
| **Eksternal** | `<a href="https://youtube.com">YouTube</a>` | Menuju website lain |
| **Anchor (ID)** | `<a href="#bagian1">Lompat ke Bagian 1</a>` | Menuju bagian tertentu dalam halaman |

---

## 5.4 Gambar (`<img>`)
Tag `<img>` bersifat **self-closing** dan digunakan untuk menampilkan gambar.

```html
<img src="gambar.jpg" alt="Deskripsi gambar" width="300" />
```

| Atribut | Fungsi |
|----------|--------|
| `src` | Lokasi file gambar |
| `alt` | Teks alternatif (penting untuk SEO & aksesibilitas) |
| `width`, `height` | Ukuran gambar (disarankan via CSS) |
| `title` | Info tambahan saat hover |
| `loading="lazy"` | Menunda pemuatan gambar (optimasi performa) |

### Gambar Responsif:
```html
<img src="small.jpg" srcset="medium.jpg 768w, large.jpg 1200w" alt="Responsive Image">
```

---

## 5.5 Audio
HTML5 menghadirkan dukungan audio tanpa plugin tambahan seperti Flash.

```html
<audio controls>
  <source src="lagu.mp3" type="audio/mpeg" />
  Browser Anda tidak mendukung audio tag.
</audio>
```

| Atribut | Fungsi |
|----------|--------|
| `controls` | Menampilkan tombol play/pause |
| `autoplay` | Memainkan otomatis (kadang diblokir browser) |
| `loop` | Mengulang otomatis |
| `muted` | Menonaktifkan suara awal |
| `preload` | Mengatur pemuatan file (`auto`, `metadata`, `none`) |

---

## 5.6 Video
Tag `<video>` digunakan untuk menampilkan video dengan kontrol bawaan.

```html
<video controls width="400" poster="thumbnail.jpg">
  <source src="video.mp4" type="video/mp4" />
  Browser Anda tidak mendukung video tag.
</video>
```

| Atribut | Fungsi |
|----------|--------|
| `controls` | Menampilkan kontrol video |
| `autoplay` | Memulai otomatis |
| `poster` | Gambar pratinjau sebelum diputar |
| `muted` | Tanpa suara awal |
| `loop` | Memutar berulang |
| `preload` | Mode pemuatan video |

---

## 5.7 Elemen `<figure>` dan `<figcaption>`
HTML5 menambahkan elemen untuk memberi keterangan gambar/video.

```html
<figure>
  <img src="html5-logo.png" alt="Logo HTML5" width="150" />
  <figcaption>Logo resmi HTML5</figcaption>
</figure>
```

---

## 5.8 Media Embedding (YouTube, Maps, dll)
Gunakan `<iframe>` untuk menyematkan konten eksternal.

```html
<iframe 
  width="560" 
  height="315" 
  src="https://www.youtube.com/embed/dD2EISBDjWM" 
  title="Video YouTube HTML5" 
  frameborder="0" 
  allowfullscreen>
</iframe>
```

---

## 5.9 Optimasi Media di HTML5
✅ Gunakan format modern (WebP untuk gambar, MP4/WebM untuk video).  
✅ Gunakan atribut `loading="lazy"` untuk performa.  
✅ Kompres ukuran file sebelum diunggah.  
✅ Tambahkan `alt` dan `title` untuk SEO & aksesibilitas.  

---

## 5.10 Kesimpulan
HTML5 menjadikan web lebih interaktif dengan dukungan **link, gambar, audio, dan video native** tanpa plugin eksternal.  
Gunakan elemen media secara efisien agar website tetap cepat dan mudah diakses di semua perangkat.

---

<div align="left">

🔗 [← Kembali ke Bab 4: Teks dan Formatting](../materi-html/04-teks-dan-formatting.md)

</div>
<div align="right">

🔗 [Lanjut ke Bab 6 → List dan Tabel HTML5](../materi-html/06-list-dan-tabel.md)

</div>
