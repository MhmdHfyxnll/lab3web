## 📄 1. Membuat List
### File: `lab3_list.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan - List</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>

    <!-- Ordered List -->
    <section id="order-list">
        <h2>Ordered List</h2>
        <ol type="A">
            <li>Pemrograman Web</li>
            <li>Sistem Informasi</li>
            <li>Basis Data 2</li>
        </ol>
    </section>

    <!-- Unordered List -->
    <section id="unorder-list">
        <h2>Unordered List</h2>
        <ul type="square">
            <li>Jaringan Komputer</li>
            <li>Struktur Data</li>
            <li>Algoritma &amp; Pemrograman</li>
        </ul>
    </section>

    <!-- Description List -->
    <section id="desc-list">
        <h2>Description List</h2>
        <dl>
            <dt>Fakultas Teknik</dt>
            <dd>Teknik Informatika</dd>
            <dd>Teknik Industri</dd>
            <dd>Teknik Lingkungan</dd>
            <dt>Fakultas Ekonomi dan Bisnis</dt>
            <dd>Akuntansi</dd>
            <dd>Manajemen</dd>
            <dd>Bisnis Digital</dd>
        </dl>
    </section>

    <!-- Nested List -->
    <section id="nested-list">
        <h2>Nested List</h2>
        <ul>
            <li>Makanan
                <ol>
                    <li>Nasi Padang</li>
                    <li>Ayam Bakar</li>
                </ol>
            </li>
            <li>Minuman
                <ol>
                    <li>Jus Mangga</li>
                    <li>Es Teh</li>
                </ol>
            </li>
        </ul>
    </section>
</body>
</html>

2. Membuat Table
File: lab3_tabel.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan - Table</title>
</head>
<body>
    <header>
        <h1>Membuat Table</h1>
    </header>

    <section id="tabel-sederhana">
        <h2>Tabel Sederhana</h2>
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
    </section>

    <section id="tabel-gabung">
        <h2>Tabel dengan Penggabungan Sel</h2>
        <table border="1" cellpadding="6" cellspacing="0">
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
                    <td rowspan="3">Teknik</td>
                    <td>Teknik Informatika</td>
                </tr>
                <tr>
                    <td>2.</td>
                    <td>Teknik Industri</td>
                </tr>
                <tr>
                    <td>3.</td>
                    <td>Teknik Lingkungan</td>
                </tr>
            </tbody>
        </table>
    </section>
</body>
</html>
3. Membuat Form
File: lab3_form.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan - Form</title>
    <style>
        form p > label {
            display: inline-block;
            width: 120px;
        }
        form input[type="text"],
        form textarea,
        form select {
            border: 1px solid #197a43;
            padding: 5px;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #fff;
            font-weight: bold;
            padding: 5px 15px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>

    <form action="proses.php" method="post">
        <fieldset>
            <legend>Data Pelanggan</legend>
            <p>
                <label for="nama">Nama</label>
                <input type="text" id="nama" name="nama">
            </p>
            <p>
                <label for="alamat">Alamat</label>
                <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
            </p>
            <p>
                <label>Jenis Kelamin</label>
                <input id="jk_l" type="radio" name="kelamin" value="L">
                <label for="jk_l">Laki-laki</label>
                <input id="jk_p" type="radio" name="kelamin" value="P">
                <label for="jk_p">Perempuan</label>
            </p>
            <p>
                <label for="kota">Kota</label>
                <select id="kota" name="kota">
                    <option>Bekasi</option>
                    <option>Jakarta</option>
                    <option>Bandung</option>
                    <option>Surabaya</option>
                </select>
            </p>
            <p>
                <label for="hobi">Hobi</label>
                <select id="hobi" name="hobi[]" multiple size="4">
                    <option>Membaca</option>
                    <option>Olahraga</option>
                    <option>Musik</option>
                    <option>Traveling</option>
                </select>
            </p>
            <p><input type="submit" value="Kirim"></p>
        </fieldset>
    </form>
</body>
</html>
```
