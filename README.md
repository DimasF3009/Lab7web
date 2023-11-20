# Lab7web

## Cetak hello world
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>
    <?php
        echo "Hello World". "<br>";
    ?>
</body>
</html>
```
### Output
![hello world](https://github.com/DimasF3009/Lab7web/assets/115356128/57f4fc19-2e1a-4457-9b2f-80fb1be1c025)

## VAR PHP
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>
    <?php
        echo "Hello World". "<br>";
    ?>
    <?php
        $nim = "312210267";
        $nama = 'Dimas Firmansyah';
        echo "NIM : " .$nim ."<br>";
        echo "Nama : $nama";
    ?>
</body>
</html>
```
### Output
![variable](https://github.com/DimasF3009/Lab7web/assets/115356128/9b264827-af23-4037-ac93-cf01e9695180)

# Predefine Variable $_GET
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <?php
        $nama = $_GET['nama'];
        echo "Selamat Datang, $nama!";
    ?>
</body>
</html>
```
### Output
![variable get](https://github.com/DimasF3009/Lab7web/assets/115356128/e1ff1ebe-301e-4899-8fbd-c25f127f2324)

# FORM
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h2>Form Input</h2>
    <form method="post">
        <label>Nama: </label>
        <input type="text" name="nama">
        <input type="submit" value="Kirim">
    </form>
    <?php
        echo 'Selamat Datang ' . $_POST['nama'];
    ?>
</body>
</html>
```
### Output
![form input](https://github.com/DimasF3009/Lab7web/assets/115356128/b6332e72-bcb6-4d5c-954b-5f22f14468f8)

# operator 
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <?php
        $gaji = 3000000;
        $pajak = 0.1;
        $thp = $gaji - ($gaji*$pajak);
        echo "Gaji sebelum pajak = Rp. $gaji <br>";
        echo "Gaji yang dibawa pulang = Rp. $thp";
    ?>
</body>
</html>
```
### Output
![operator](https://github.com/DimasF3009/Lab7web/assets/115356128/527197c2-cd09-43aa-a3ca-9d9a4bba764c)

# if else
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <?php
        $nama_hari = date("l");
        if ($nama_hari == "Sunday") {
            echo "Minggu";
        } elseif ($nama_hari == "Monday") {
            echo "Senin";
        } else {
            echo "Selasa";
        }
    ?>
</body>
</html>
```
### Output
![if else](https://github.com/DimasF3009/Lab7web/assets/115356128/087b4ef0-1e48-439d-a3fb-9a46f7c201ad)

# Switch
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
<?php
    $nama_hari = date("l");
    switch ($nama_hari) {
    case "Sunday":
        echo "Minggu";
        break;
    case "Monday":
        echo "Senin";
        break;
    case "Tuesday":
        echo "Selasa";
        break;
    default:
        echo "Sabtu";
    }
?>
</body>
</html>
```
### Output
![switch](https://github.com/DimasF3009/Lab7web/assets/115356128/d1f77072-ea44-489b-896b-b7cc322e6b33)

# Looping FOR
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
<?php
    echo "Perulangan 1 sampai 10 <br />";
    for ($i=1; $i<=10; $i++) {
        echo "Perulangan ke: " . $i . '<br />';
    }
    echo "Perulangan Menurun dari 10 ke 1 <br />";
    for ($i=10; $i>=1; $i--) {
        echo "Perulangan ke: " . $i . '<br />';
    }
?>
</body>
</html>
```
### Output
![for](https://github.com/DimasF3009/Lab7web/assets/115356128/fb7c7887-b8b7-43c4-887c-10340f1dd771)

# Looping while
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
<?php
    echo "Perulangan 1 sampai 10 <br />";
    $i=1;
    while ($i<=10) {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
    }
?>
</body>
</html>
```
### Output
![while](https://github.com/DimasF3009/Lab7web/assets/115356128/782936e4-e595-470e-becc-1df29fc4ced8)

# Looping dowhile
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
<?php
    echo "Perulangan 1 sampai 10 <br />";
    $i=1;
    do {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
    } while ($i<=10);
?>
</body>
</html>
```
### Output
![dowhile](https://github.com/DimasF3009/Lab7web/assets/115356128/4063f99d-23a4-455f-af0a-e8cdeb3eeeb0)


# Tugas Membuat form sederhana
```
<!DOCTYPE html>
<html>
<head>
    <title>Form Input PHP</title>
</head>
<body>

<?php
// Fungsi untuk menghitung umur berdasarkan tanggal lahir
function hitungUmur($tanggal_lahir) {
    $tanggal_lahir = new DateTime($tanggal_lahir);
    $sekarang = new DateTime('today');
    $umur = $sekarang->diff($tanggal_lahir);
    return $umur->y;
}

// Daftar pekerjaan beserta gaji
$pekerjaan = array(
    'Programmer' => 5000000,
    'Desainer' => 4500000,
    'Marketing' => 4000000,
    'Manajer' => 6000000
);

// Inisialisasi variabel
$nama = '';
$tanggal_lahir = '';
$pekerjaan_selected = '';
$gaji = 0;

// Pengecekan apakah form sudah di-submit
if ($_SERVER['REQUEST_METHOD'] === 'POST') {
    // Mengambil nilai dari form
    $nama = $_POST['nama'];
    $tanggal_lahir = $_POST['tanggal_lahir'];
    $pekerjaan_selected = $_POST['pekerjaan'];

    // Validasi input
    if (empty($nama) || empty($tanggal_lahir) || empty($pekerjaan_selected)) {
        echo "Semua field harus diisi!";
    } else {
        // Menghitung umur berdasarkan tanggal lahir
        $umur = hitungUmur($tanggal_lahir);

        // Mengambil gaji berdasarkan pekerjaan
        $gaji = $pekerjaan[$pekerjaan_selected];

        // Menampilkan output
        echo "Nama: $nama <br>";
        echo "Umur: $umur tahun <br>";
        echo "Pekerjaan: $pekerjaan_selected <br>";
        echo "Gaji: Rp " . number_format($gaji, 0, ',', '.') . "<br>";
    }
}
?>

<!-- Form input -->
<form method="post" action="">
    Nama: <input type="text" name="nama" value="<?php echo $nama; ?>"><br>
    Tanggal Lahir: <input type="date" name="tanggal_lahir" value="<?php echo $tanggal_lahir; ?>"><br>
    Pekerjaan:
    <select name="pekerjaan">
        <option value="Programmer" <?php echo ($pekerjaan_selected == 'Programmer') ? 'selected' : ''; ?>>Programmer</option>
        <option value="Desainer" <?php echo ($pekerjaan_selected == 'Desainer') ? 'selected' : ''; ?>>Desainer</option>
        <option value="Marketing" <?php echo ($pekerjaan_selected == 'Marketing') ? 'selected' : ''; ?>>Marketing</option>
        <option value="Manajer" <?php echo ($pekerjaan_selected == 'Manajer') ? 'selected' : ''; ?>>Manajer</option>
    </select><br>
    <input type="submit" value="Submit">
</form>

</body>
</html>
```
### Output
![tugas](https://github.com/DimasF3009/Lab7web/assets/115356128/ca980c57-fdb4-49b2-ae3e-8c4a5908d1f7)
