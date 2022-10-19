# Asynchronous Pada JavaScript

terdapat 3 fitur yang selalu dipakai ketika menggunakan JavaScript. kita perlu menjalankan eksekusi kode secara “asinkronus” ke dalam “event loop” dari proses utama JavaScript itu sendiri yaitu :

- Promise
- CallBack
- Await

Deklarasikan Fungsi Promise

    Function GetUser(id) {
        return new Promise ((resolve, reject) => {
            if (id !== "" && id !== underfined) {
                resolve (id) ;
            } else {
                reject ("ID Harus Di Isi");
            }
        });
    }

Cara Penggunaan Promise

    GetUser ()
    .then ((response) => {
        console.log(response);
    })
    .catch ((error) =>{
        console.log(error);
    });

## Fetch Data

> Fetch Data merupakan fungsi atau alat kominikasi HTTP yang bertujuan untuk mengembalikan dan mengirim data pada suatu server.

HTTP Request

1. Get => Mengambil data
2. Post => Mengirim Data
3. Put => Mengirim/Memperbaharui/update
4. Patch => update <= request tidak aman (Mengirim data secara parsial)
5. Delete => Menghapus Data

Fetch Get 1

    fetch ("https://pokeapi.co/api/v2/pokemon/pikachu/", {
        method: "GET"
    })

    .then ((response) => {
        return response.json();
    })
    .then((data) => {
        console.log(data)
    })
    .catch ((error) => {
        console.log(error);
    });

Fetch Get 2

    fetch ("https://pokeapi.co/api/v2/pokemon/pikachu/", {
            method: "GET"
    })
    .then (async (response) => {
        let convertData = await response.json();
        console.log(convertData)
    })
    .catch ((error) => {
            console.log(error);
    });

## Responsive Web Desain

> Responsive Web Design (RWD) ini bertujuan untuk membuat desain websitekita dapat diakses dalam device apapun. Device yang umumnya digunakan adalah lapto/pc, smartphone, dan tablet.

### Tambahkan tampilan di HTML. Pada html terdapat meta viewport yang diperlukan pada responsiv seluler

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>

    </body>
    </html>

### Media Query

> Jenis Media Query untuk responsive web design umumnya hanya menggunakan 2 jenis media query yaitu **main-width** dan **mas-width**.

    Contoh:

    @media screnn and (min-width: your pixel){

    }
    @media screnn and (max-width: your pixel){

    }

> media query digunakan untuk membuat beberapa styles tergantung pada jenis device. terdapat 2 cara dalam menggunakan media query

Cara ke - 1:
membuat file css berbeda untuk masing-masing device

Cara ke - 2:
menggabungkan 1 file css untuk setting styling berbagai device.

### Breckpoint

> perubahan yang terjadi pada tampilan saat berganti device atau ukuran width disebut breckpoint.

### complex Breackpoint Media Query

> jika menginginkan tampilan yang ingin diterapkan pada range ukuran device tertentu. kita bisa membuat menjadi range media query

    contoh :

    body{
    background-color: white ;
    }

    @media screen and (min-width: 500px) and (min-width: 700px)
    body {
    background-color: aquamarine ;
    }

## Boostrep 5

> Bootstrap adalah framework HTML, CSS, dan JavaScript yang berfungsi untuk mendesain website responsive dengan cepat dan mudah.

> Kemudahan yang ditawarkan oleh Bootstrap adalah Anda tak perlu coding komponen website dari nol. Framework ini tersusun dari kumpulan file CSS dan JavaScript berbentuk class yang tinggal pakai.

> Class yang disediakan Bootstrap juga cukup lengkap. Mulai dari class untuk layout halaman, class menu navigasi, class animasi, dan masih banyak lainnya.

#### Cara memanggil css dan js pada boostrep 5

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">

    <!-- Option 1: Bootstrap Bundle with Popper -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>

#### Warna warna yang ada di boostrep 5

"primary": Biru,
"secondary": abu-abu,
"success": Hijau,
"info": Biru langit,
"warning": Kuning,
"danger": Merah,
"light": Putih,
"dark": Hitam.

#### Breakpoint Ukuran yang tersedia

| Breakpoint  | Class infix | Dimensions |
| ----------- | ----------- | ---------- |
| X-Small     | none        | <576px     |
| Small       | sm          | ≥576px     |
| Medium      | md          | ≥768px     |
| Large       | lg          | ≥992px     |
| Extra large | xl          | ≥1200px    |
| Extra large | xxl         | ≥1400px    |
