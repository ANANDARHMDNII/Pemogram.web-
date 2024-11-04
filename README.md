# PROFIL
## UTS Pemrograman Web ![alt text](PHP-Logo-Free-Download-PNG.png)
| Variable           |       isi           |
| -------------------|---------------------|
| **Nama**           | Ananda Rahmadani    |
| **NIM**            | 312310461           |
| **Kelas**          | TI.23.A.5           |
| **Mata Kuliah**    | Pemrograman Web     |

### Membuat Website-Dinamis
### langkah-langkah
### 1. Membuat file website-dinamis


### 2. Menjalankan  MySQL server
![alt text](mysql.png)


# Mengakses Apache Client menggunakan "website-dunamis".
pastikan webserver Apache sudah dijalankan. kemudian untuk mengakses direktory tersebut pada web server dengan mengakses URL:
http://localhost/website-dinamis/?page=home

# 3. Membuat index: membuat webssite-dinamis

# membuat tampilan dalam

<!doctype html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Bootstrap demo</title>
    <!-- Bootstrap -->
    <link href="assets/css/bootstrap.min.css" rel="stylesheet">

    <!-- Datatables -->
    <link href="assets/datatables/dataTables.dataTables.css" rel="stylesheet">
</head>

<body>
    <header>
        <h1 class="text-center p-3">Membuat website dinamis</h1>
        <!-- navbar -->
        <?php include "includes/navbar.php" ?>
        <!-- ./navbar -->

        <!-- konten -->
        <div class="container mt-3">
            <?php include "konten.php"?>
        </div>
        <!-- konten -->

        <footer class="bg-dark text-white text-center py-3 mt-5">
            <div class="container">
                <div class="row">
                    <div class="col-md-4">
                        <h5>Kontak Kami</h5>
                        <p>Email: lutpiahainus@gmail.com</p>
                        <p>Telepon: (+62) 823-3345-6789</p>
                    </div>
                    <div class="col-md-4">
                        <h5>Ikuti Kami</h5>
                        <a href="#" class="text-white me-2"><i class="bi bi-facebook"></i></a>
                        <a href="#" class="text-white me-2"><i class="bi bi-twitter"></i></a>
                        <a href="#" class="text-white"><i class="bi bi-instagram"></i></a>
                    </div>
                    <div class="col-md-4">
                        <h5>Lokasi</h5>
                        <p>Jl. maju, Kota Mundur</p>
                        <p>Indonesia</p>
                    </div>
                </div>
                <div class="text-center mt-3">
                    <small>&copy; 2024 Website Dinamis. All rights reserved.</small>
                </div>
            </div>
        </footer>

        <script src="assets/jquery-3.7.1.js"></script>
        <script src="assets/datatables/dataTables.js"></script>

        <script src="assets/js/bootstrap.bundle.min.js"></script>

        <script>
        new DataTable('#example');
        </script>

</body>

</html>


# Menambahkan data navbar

<nav class="navbar bg-dark navbar-expand-md bg-body-tertiary" data-bs- theme="dark">

    <div class="container-fluid">
        <a class="navbar-brand" href="?page=home">Navbar</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false" aria- label="Toggle navigation">

            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="nav-item">
                    <a class="nav-link active" aria-current="page" href="?page=home">Home</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="?page=about">About</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="?page=contact">Contact</a>
                </li>

                <li class="nav-item dropdown">
                    <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
                        aria-expanded="false">
                        Belajar
                    </a>
                    <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="?page=datatables">Datatables</a></li>

                        <li><a class="dropdown-item" href="?page=form">form</a></li>

                        <li>
                            <hr class="dropdown-divider">
                        </li>
                        <li><a class="dropdown-item" href="#">Something else here</a></li>

                    </ul>
                </li>
            </ul>
            <form class="d-flex" role="search">
                <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">

                <button class="btn btn-outline-success" type="submit">Search</button>

            </form>
        </div>
    </div>
</nav>

# outputnya ketika berhasil:

![alt text](navbar.png)

# 3. Menambahkan Home
dengan memasukan halaman Home

![alt text](image/image.png)

<h1>Halaman Home</h1>
<div class="container">
    <div class="row">
        
        <!-- Card 1 -->
        <div class="col-md-6">
            <div class="card" style="width: 100%;">
                <img src="imege/Cisco.webp" class="card-img-top" alt="...">
                <div class="card-body">
                    <h5 class="card-title">Cisco Networking Academy</h5>
                    <p class="card-text">program tanggung jawab sosial perusahaan (CSR) internasional 
                        yang bertujuan membantu siswa dan pendidik mengembangkan keterampilan untuk pekerjaan di bidang teknologi informasi.</p>
                    <a href="https://www.netacad.com/courses/networking-basics?courseLang=en-US" class="btn btn-primary">Go somewhere</a>
                </div>
            </div>
        </div>

        <!-- Card 2 -->
        <div class="col-md-6">
            <div class="card" style="width: 88%;">
                <img src="imege/GitHub-Emblem.png" class="card-img-top" alt="...">
                <div class="card-body">
                    <h5 class="card-title">Git Hub</h5>
                    <p class="card-text">platform berbasis web yang digunakan untuk mengelola dan menyimpan kode sumber perangkat lunak
                        GitHub menggunakan sistem kontrol versi Git dan layanan hosting internet.</p>
                    <a href="https://github.com/dashboard" class="btn btn-primary">Go somewhere</a>
                </div>
            </div>
        </div>
    </div>
</div>

# 4. Menambahkan about
dengan memasukan image dan carousel dari :
http://localhost/website-dinamis/?page=about

gamabar img

<h1>Halaman about</h1>
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profil - Ananda Rahmadani</title>
    <style>
    /* CSS untuk styling foto dan teks */
    .profile-container {
        text-align: center;
        margin-top: 20px;
    }

    .profile-img {
        width: 150px;
        /* ukuran foto */
        height: 150px;
        border-radius: 50%;
        /* membuat foto menjadi bulat */
        object-fit: cover;
        border: 3px solid #007bff;
        /* warna border */
    }

    .profile-name {
        font-size: 1.5em;
        font-weight: bold;
    }

    .profile-university {
        font-size: 1em;
        color: #555;
    }
    </style>
</head>

<body>
    
    <div class="profile-container">
        <!-- Foto Profil -->
        <img src="imege/Profil.nnda.jpeg" class="profile-img"
            alt="Ananda Rahmadani">

        <!-- Nama dan Universitas -->
        <h2 class="profile-name">Ananda Rahmadani</h2>
        <p class="profile-university">Jl. Pelita , Kota Bangsa</p>
    </div>
    <div id="carouselExampleCaptions" class="carousel slide">
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active"
                aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
                aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
                aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="imege/UPB.jpeg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-none d-md-block">
                    <h5>University</h5>
                    <p>Kalimalang.</p>
                </div>
    </div>
</body>

</html>

# Membuat Data Tables Belajar
berikan Skrip untuk Data Tables Belajar yang mengacu pada:
https://datatables.net/examples/basic_init/zero_configuration.html

# Membuat Form Belajar
menambahkan form dari:
https://getbootstrap.com/docs/5.3/forms/overview/#overview

## KAMSIA
