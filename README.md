# 🧾 Praktikum 5 – JavaScript

**Nama:** Alfarizki Aprilia Putri
**NIM:** 312410455  
**Mata Kuliah:** Pemrograman Web  
**Dosen Pengampu:** Agung Nugroho, S.Kom., M.Kom  
**Universitas:** Universitas Pelita Bangsa  

---

## 🎯 Tujuan Praktikum
1. Mahasiswa memahami sintaks dasar JavaScript.  
2. Mahasiswa mampu menggunakan JavaScript untuk manipulasi elemen HTML.  
3. Mahasiswa mampu membuat kode JavaScript sederhana.  
4. Mahasiswa mampu membuat validasi form menggunakan JavaScript.  

---

## ⚙️ Langkah-Langkah Praktikum

### 🧩 1. Persiapan Folder & File
Buat folder baru bernama **`lab5_javascript`**  
Lalu buat file **`lab5_javascript.html`**

---

### 🍼 2. Menampilkan Tulisan “Hello World”
Kode berikut digunakan untuk menampilkan teks “Hello World” di halaman dan console:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Mengenal JavaScript</title>
</head>
<body>
  <h1>Pengenalan JavaScript</h1>
  <h3>Contoh document.write dan console.log</h3>

  <script>
    document.write("Hello World");
    console.log("Hello World");
  </script>
</body>
</html>

```

![foto]()

### 💬 3. Menampilkan Alert, Prompt, dan Function

Kode ini menampilkan pesan pop-up dan meminta input nama pengguna, kemudian menampilkan sapaan.

```html
<script>
  alert("Halo bayi coder!");

  let nama = prompt("Siapa nama kamu?");
  alert("Hai " + nama + "! Selamat belajar JavaScript~");

  function sapa(nama) {
    document.write("<br>Halo juga, " + nama + "!");
  }

  sapa(nama);
</script>

```
![foto]()

![foto]()

![foto]()

## ➗ 4. Operasi Aritmatika

Membuat perhitungan sederhana menggunakan JavaScript.

```html

<script>
  let a = 10;
  let b = 5;
  let hasil = a + b;
  document.write("<br>Hasil penjumlahan: " + hasil);
</script>

```
![foto]()

### 🔍 5. Seleksi Kondisi (if...else)

Kode ini digunakan untuk menentukan apakah pengguna sudah dewasa atau belum.

```html

<script>
  let umur = prompt("Masukkan umur kamu:");
  if (umur >= 18) {
    document.write("<br>Kamu udah dewasa!");
  } else {
    document.write("<br>Kamu masih bocil 😆");
  }
</script>

```
![foto]()

### 🔄 6. Switch Case

Menampilkan pesan berdasarkan hari yang dimasukkan.

```html
<script>
  let hari = prompt("Masukkan hari (senin/minggu):");
  switch (hari) {
    case "senin":
      document.write("<br>Semangat kerja!");
      break;
    case "minggu":
      document.write("<br>Waktunya santai~");
      break;
    default:
      document.write("<br>Hari tidak dikenal 😅");
  }
</script>

```

![foto]()

### 📝 7. Validasi Form (Tugas Akhir)

Membuat form pendaftaran sederhana dengan validasi agar tidak boleh kosong.

``` html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Validasi Form</title>
</head>
<body>
  <h2>Form Pendaftaran Bayi Coder 🍼</h2>

  <form onsubmit="return validasiForm()">
    Nama: <input type="text" id="nama"><br><br>
    Email: <input type="email" id="email"><br><br>
    Umur: <input type="number" id="umur"><br><br>
    <button type="submit">Kirim</button>
  </form>

  <script>
    function validasiForm() {
      let nama = document.getElementById("nama").value;
      let email = document.getElementById("email").value;
      let umur = document.getElementById("umur").value;

      if (nama == "" || email == "" || umur == "") {
        alert("Isi semua datanya yaa 😚");
        return false;
      } else {
        alert("Yay, data kamu udah lengkap 🎉");
        return true;
      }
    }
  </script>
</body>
</html>


```

![foto]()

![foto]()





