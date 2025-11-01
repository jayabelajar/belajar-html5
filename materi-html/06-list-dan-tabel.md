# 📋 BAB 6 — List dan Tabel HTML5

## 6.1 Pengantar
HTML5 menyediakan elemen untuk **menyusun data berurutan atau terstruktur**, yaitu **list (daftar)** dan **tabel (table)**.  
Keduanya berperan penting untuk menampilkan konten informatif secara terorganisir.

---

## 6.2 List (Daftar)
List digunakan untuk menampilkan kumpulan item yang berhubungan.  
Ada **3 jenis utama**: unordered, ordered, dan definition list.

---

### 6.2.1 Unordered List (`<ul>`)
Menampilkan daftar **tanpa urutan angka** (biasanya berupa bullet).

```html
<ul>
  <li>Apel</li>
  <li>Pisang</li>
  <li>Jeruk</li>
</ul>
```

Hasil:  
• Apel  
• Pisang  
• Jeruk

---

### 6.2.2 Ordered List (`<ol>`)
Menampilkan daftar **berurutan** (angka, huruf, atau romawi).

```html
<ol>
  <li>Bangun tidur</li>
  <li>Mandi</li>
  <li>Sarapan</li>
</ol>
```

Atribut penting:
| Atribut | Fungsi | Contoh |
|----------|---------|--------|
| `type` | Menentukan jenis penomoran (`1`, `A`, `a`, `I`, `i`) | `<ol type="A">` |
| `start` | Nomor awal urutan | `<ol start="5">` |
| `reversed` | Mengurutkan mundur | `<ol reversed>` |

---

### 6.2.3 Nested List
List dapat disusun di dalam list lain.

```html
<ul>
  <li>Frontend
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
    </ul>
  </li>
  <li>Backend</li>
</ul>
```

---

### 6.2.4 Definition List (`<dl>`)
Cocok untuk **glosarium atau daftar istilah**.

```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```

---

## 6.3 Tabel (Table)
Tabel digunakan untuk **menampilkan data dalam baris dan kolom**.

```html
<table border="1">
  <tr>
    <th>Nama</th>
    <th>Usia</th>
    <th>Kota</th>
  </tr>
  <tr>
    <td>Andi</td>
    <td>21</td>
    <td>Surabaya</td>
  </tr>
  <tr>
    <td>Sinta</td>
    <td>22</td>
    <td>Malang</td>
  </tr>
</table>
```

| Tag | Fungsi |
|------|--------|
| `<table>` | Pembungkus seluruh tabel |
| `<tr>` | Baris tabel (table row) |
| `<th>` | Header kolom |
| `<td>` | Isi data (table data) |

---

### 6.3.1 Atribut Tabel
| Atribut | Fungsi |
|----------|--------|
| `border` | Menentukan ketebalan garis (disarankan via CSS) |
| `cellpadding` | Jarak dalam sel |
| `cellspacing` | Jarak antar sel |
| `colspan` | Menggabungkan kolom |
| `rowspan` | Menggabungkan baris |

Contoh gabungan kolom:
```html
<td colspan="2">Gabungan dua kolom</td>
```

---

### 6.3.2 Struktur Lengkap dengan `<thead>`, `<tbody>`, `<tfoot>`
```html
<table>
  <thead>
    <tr>
      <th>Nama</th>
      <th>Nilai</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Budi</td>
      <td>90</td>
    </tr>
    <tr>
      <td>Siti</td>
      <td>85</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="2">Total Siswa: 2</td>
    </tr>
  </tfoot>
</table>
```

---

### 6.3.3 Styling Modern (CSS)
Gunakan CSS untuk membuat tabel lebih rapi:
```html
<style>
  table {
    border-collapse: collapse;
    width: 100%;
  }
  th, td {
    border: 1px solid #aaa;
    padding: 8px;
    text-align: left;
  }
  th {
    background: #eaeaea;
  }
</style>
```

---

## 6.4 Kesimpulan
List dan tabel membantu menyusun informasi agar mudah dibaca dan dipahami.  
Gunakan tabel hanya untuk **data tabular**, bukan layout (karena itu tugas CSS).

---

<div align="left">

🔗 [← Kembali ke Bab 5: Link dan Media](../materi-html/05-link-dan-media.md)

</div>
<div align="right">

🔗 [Lanjut ke Bab 7 → Formulir dan Input HTML5](../materi-html/07-formulir-dan-input.md)

</div>
