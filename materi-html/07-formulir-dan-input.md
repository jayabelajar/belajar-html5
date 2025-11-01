# 📝 BAB 7 — Formulir dan Input HTML5

## 7.1 Pengantar
Formulir (form) adalah cara utama **berinteraksi dengan pengguna** di web.  
HTML5 memperkenalkan banyak **fitur baru** untuk validasi otomatis dan input yang lebih intuitif.

---

## 7.2 Struktur Dasar Formulir
```html
<form action="/proses" method="POST">
  <label for="nama">Nama:</label>
  <input type="text" id="nama" name="nama" required />
  
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" />
  
  <input type="submit" value="Kirim" />
</form>
```

| Atribut | Fungsi |
|----------|--------|
| `action` | URL tujuan pengiriman data |
| `method` | Cara kirim (`GET` / `POST`) |
| `name` | Nama variabel dikirim |
| `id` | Identifikasi elemen untuk label |
| `required` | Input wajib diisi |

---

## 7.3 Elemen Form Umum
| Elemen | Fungsi | Contoh |
|---------|---------|--------|
| `<input>` | Bidang input tunggal | `<input type="text">` |
| `<textarea>` | Input teks panjang | `<textarea></textarea>` |
| `<select>` | Dropdown pilihan | `<select><option>1</option></select>` |
| `<button>` | Tombol aksi | `<button>Kirim</button>` |
| `<fieldset>` | Mengelompokkan input | `<fieldset>...</fieldset>` |
| `<legend>` | Judul kelompok fieldset | `<legend>Data Pribadi</legend>` |

---

## 7.4 Jenis Input HTML5 Modern
HTML5 menambah banyak tipe baru untuk kemudahan pengguna.

| Type | Fungsi | Contoh |
|-------|---------|--------|
| `text` | Teks biasa | `<input type="text">` |
| `email` | Validasi format email | `<input type="email">` |
| `password` | Menyembunyikan input | `<input type="password">` |
| `number` | Input angka | `<input type="number" min="0" max="100">` |
| `date` | Pilih tanggal | `<input type="date">` |
| `time` | Pilih waktu | `<input type="time">` |
| `color` | Pemilih warna | `<input type="color">` |
| `range` | Slider angka | `<input type="range" min="0" max="10">` |
| `file` | Unggah file | `<input type="file">` |
| `url` | Validasi URL | `<input type="url">` |
| `tel` | Input nomor telepon | `<input type="tel">` |
| `search` | Kolom pencarian | `<input type="search">` |
| `checkbox` | Pilihan ganda | `<input type="checkbox" checked>` |
| `radio` | Pilihan tunggal | `<input type="radio" name="gender">` |
| `submit` | Tombol kirim | `<input type="submit" value="Kirim">` |
| `reset` | Reset form | `<input type="reset">` |

---

## 7.5 Atribut Tambahan Input
| Atribut | Fungsi | Contoh |
|----------|--------|--------|
| `placeholder` | Teks petunjuk awal | `<input placeholder="Masukkan nama">` |
| `readonly` | Tidak bisa diubah | `<input readonly>` |
| `disabled` | Tidak aktif | `<input disabled>` |
| `autofocus` | Fokus otomatis | `<input autofocus>` |
| `pattern` | Validasi regex | `<input pattern="[A-Za-z]{3,}">` |
| `maxlength` | Batas karakter | `<input maxlength="20">` |

---

## 7.6 Label & Aksesibilitas
Gunakan tag `<label>` agar formulir lebih ramah aksesibilitas.

```html
<label for="username">Username:</label>
<input id="username" name="username" type="text" />
```

> Saat label diklik, input yang terkait otomatis fokus.

---

## 7.7 Validasi Otomatis HTML5
Browser bisa memvalidasi input secara otomatis tanpa JavaScript.

```html
<form>
  <input type="email" placeholder="Masukkan email" required>
  <input type="number" min="1" max="10" required>
  <input type="submit" value="Kirim">
</form>
```

Pesan validasi otomatis muncul bila format salah atau kosong.

---

## 7.8 Elemen `<datalist>` (Autocomplete)
HTML5 mendukung daftar saran otomatis saat mengetik.

```html
<label for="browser">Browser Favorit:</label>
<input list="browsers" id="browser" name="browser">
<datalist id="browsers">
  <option value="Chrome">
  <option value="Firefox">
  <option value="Edge">
  <option value="Safari">
</datalist>
```

---

## 7.9 Contoh Formulir Lengkap
```html
<form action="/daftar" method="POST">
  <fieldset>
    <legend>Formulir Pendaftaran</legend>

    <label>Nama:</label>
    <input type="text" name="nama" required>

    <label>Email:</label>
    <input type="email" name="email" required>

    <label>Tanggal Lahir:</label>
    <input type="date" name="lahir">

    <label>Jenis Kelamin:</label>
    <input type="radio" name="gender" value="Pria"> Pria
    <input type="radio" name="gender" value="Wanita"> Wanita

    <label>Hobi:</label>
    <input type="checkbox" name="hobi" value="Membaca"> Membaca
    <input type="checkbox" name="hobi" value="Olahraga"> Olahraga

    <label>Warna Favorit:</label>
    <input type="color" name="warna">

    <input type="submit" value="Daftar">
  </fieldset>
</form>
```

---

## 7.10 Kesimpulan
Formulir HTML5 kini lebih kaya dan mudah digunakan.  
Gunakan tipe input yang tepat dan validasi otomatis agar pengalaman pengguna lebih nyaman serta aman.

---

<div align="left">

🔗 [← Kembali ke Bab 6: List dan Tabel HTML5](../materi-html/06-list-dan-tabel.md)

</div>
<div align="right">

🔗 [Lanjut ke Bab 8 → Elemen Semantik HTML5](../materi-html/08-elemen-semantik-html5.md)

</div>
