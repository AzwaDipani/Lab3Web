# Lab3Web

Nama : Muhammad Azwa Dipani

NIM  : 312210417

Kelas : TI.22.A1

## Instruksi Praktikum
> 1. Persiapkan text editor misalnya VSCode.
> 2. Buat folder baru dengan nama Lab3Web
> 3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
> 4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

## Praktikum
**1. Membuat Ordered List & Undordered List**

```
<section id="order-list">
  <h2>Ordered List</h2>
  <ol>
    <li>Pemrograman Web</li>
    <li>Sistem Informasi</li>
    <li>Basis Data 2</li>
  </ol>
</section>
```

![img](pictures/Screenshot%20(141).png)


```
<section id="unorder-list">
  <h2>Unordered List</h2>
  <ul type="square">
    <li>Jaringan Komputer</li>
    <li>Struktur Data</li>
    <li>Algoritma &amp; Pemrograman</li>
  </ul>
</section>
```

![img](pictures/Screenshot%20(142).png)


**2. Membuat Description List**

```
<section id="unorder-list">
  <h2>Description List</h2>
  <dl>
    <dt>Fakultas Teknik</dt>
    <dd>Teknik Industri</dd>
    <dd>Teknik Informatika</dd>
    <dd>Teknik Lingkungan</dd>
    <dt>Fakultas Ekonomi dan Bisnis</dt>
    <dd>Akuntansi</dd>
    <dd>Manajemen</dd>
    <dd>Bisnis Digital</dd>
  </dl>
</section>
```

![img](pictures/Screenshot%20(143).png)


**3. Membuat Table**

```
<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>Teknik</td>
      <td>Teknik Informatika</td>
    </tr>
    <tr>
      <td>2.</td>
      <td>Teknik</td>
      <td>Teknik Industri</td>
    </tr>
    <tr>
      <td>3.</td>
      <td>Teknik</td>
      <td>Teknik Lingkungan</td>
    </tr>
  </tbody>
</table>
```

![img](pictures/Screenshot%20(144).png)


**4. Membuat Margin dan Padding**

```
<table border="1" cellpadding="4" cellspacing="0"></table>
```

![img](pictures/Screenshot%20(145).png)


**5. Menggabungkan Sel Data**

```
<tr>
  <td>1.</td>
  <td rowspan="3">Teknik</td>
  <td>Teknik Informatika</td>
</tr>
```

![img](pictures/Screenshot%20(146).png)


**6. Membuat Form**

```
<form action="proses.php" method="post">
  <fieldset>
    <legend>Data Pelanggan</legend>
    <p>
      <label for="nama">Nama</label>
      <input type="text" id="nama" name="nama" />
    </p>
    <p>
      <label for="alamat">Alamat</label>
      <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
    </p>
    <p>
      <label>Jenis Kelamin</label>
      <input id="jk_l" type="radio" name="kelamin" value="L" /><label for="jk_l"
        >Laki-laki</label
      >
      <input id="jk_p" type="radio" name="kelamin" value="P" /><label
        qafor="jk_p"
        >Perempuan</label
      >
    </p>
    <p><input type="submit" value="Login" /></p>
  </fieldset>
</form>
```

![img](pictures/Screenshot%20(147).png)


**7. Menambahkan Style**

```
<style>
        form p > label {
            display: inline-block;
            width: 100px;
        }
        form input[type="text"], form textarea {
            border: 1px solid #197a43;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 5px 15px;
        }
    </style>
```

![img](pictures/Screenshot%20(148).png)


**8. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org**


![img](pictures/Screenshot%20(149).png)

![img](pictures/Screenshot%20(150).png)


## Pertanyaan dan Tugas
1. Buatlah form yang menampilkan **dropdown** menu dan **listbox** dengan *multiple selection.*

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tugas Form Dropdown and Listbox</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <nav>
        <a href="Lab3Web.html">List HTML</a>
        <a href="lab3_tabel.html">Tabel HTML</a>
        <a href="lab3_form.html">Form HTML</a>
        <a href="lab3_tugas.html">Form Dropdown & Listbox</a>
    </nav>
    <header>
        <h1>Form Dropdown & Listbox</h1>
    </header>
    <form action="#">
        <label for="lang">Language</label>
        <select name="languages" id="lang">
          <option value="select">Select a Language</option>
          <option value="javascript">JavaScript</option>
          <option value="php">PHP</option>
          <option value="java">Java</option>
          <option value="golang">Golang</option>
          <option value="python">Python</option>
          <option value="c#">C#</option>
          <option value="C++">C++</option>
          <option value="erlang">Erlang</option>
        </select>
        <input type="submit" value="Submit">
    </form>
</body>

</html>
```

```
body {
    margin-top: 50px;
    text-align: center;
    height: 100vh; 
    background-color: #f1f1f1;
  }
  
  h1 {
    color: rgb(12, 0, 0);
  }

  input {
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto;
  }

  label {
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto;
  }

  select {
    margin-bottom: 10px;
    margin-top: 10px;
  }
  
  nav {
    background-color: #3fb8e0c5;
    padding: 10px;
    position: fixed;
    top: 0px;
    right: 0px;
    left: 0px;
    text-align: center;
  }
  
  nav a {
    color: #fff;
    text-decoration: none;
    padding: 2px 4px;
    font-size: 13px;
  }
```

![img](pictures/Screenshot%20(151).png)
![img](pictures/Screenshot%20(152).png)


## Selesai, Terima Kasih
