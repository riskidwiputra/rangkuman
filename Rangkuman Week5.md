# **Rangkuman Week 5**


## Web Server dan RESTful API
### Web Server
#### Komponen Web Server
- Hardware
adalah komputer yang menyimpan perangkat lunak server web dan file komponen situs web. (misalnya, dokumen HTML, gambar, CSS stylesheet, dan file JavaScript) Server web terhubung ke Internet dan mendukung pertukaran data fisik dengan perangkat lain yang terhubung ke web.
- Software
server web mencakup beberapa bagian yang mengontrol bagaimana pengguna web mengakses file yang dihosting. Minimal, ini adalah server HTTP. Server HTTP adalah perangkat lunak yang memahami URL (alamat web) dan HTTP (protokol yang digunakan browser Anda untuk melihat halaman web). Server HTTP dapat diakses melalui nama domain situs web yang disimpannya, dan mengirimkan konten situs web yang dihosting ini ke perangkat pengguna akhir.

#### Static Web Server VS Dynamic Web Server
- Static Web Server
   Static Web Server, terdiri dari komputer (perangkat keras) dengan server HTTP (perangkat lunak). Kami menyebutnya "statis" karena server mengirimkan file yang dihosting apa adanya ke browser Anda.
- Dynamic Web Server
  Sebuah server web dinamis terdiri dari server web statis ditambah perangkat lunak tambahan, paling sering server aplikasi dan database. Kami menyebutnya "dinamis" karena server aplikasi memperbarui file yang dihosting sebelum mengirim konten ke browser Anda melalui server HTTP
### Server Side Programming
Web Server menunggu pesan permintaan klien, memprosesnya saat tiba, dan membalas browser web dengan pesan respons HTTP. Respons berisi baris status yang menunjukkan apakah permintaan berhasil atau tidak (misal "HTTP/1.1 200 OK" untuk berhasil). Isi respons yang berhasil atas permintaan akan berisi sumber daya yang diminta (misalnya halaman HTML baru, atau gambar, dll...), yang kemudian dapat ditampilkan oleh web browser.
### Static Sites
Static sites menggunakan rendering sisi server untuk menyajikan file HTML, CSS, dan JavaScript yang telah dibuat sebelumnya ke browser web, berbeda dengan situs dinamis tradisional yang bekerja dengan merender halaman web pada saat permintaan.
### Dynamic Sites
Dynamic sites adalah situs di mana beberapa konten respons dihasilkan secara dinamis, hanya bila diperlukan. Di situs web dinamis, halaman HTML biasanya dibuat dengan memasukkan data dari database ke dalam placeholder di template HTML (ini adalah cara yang jauh lebih efisien untuk menyimpan konten dalam jumlah besar daripada menggunakan situs web statis).
### Perbedaan Static Sites dan Dynamic Sites
- Memiliki tujuan dan perhatian yang berbeda.
- Umumnya tidak menggunakan bahasa pemrograman yang sama (pengecualiannya adalah JavaScript, yang dapat digunakan di sisi server dan klien).
- Berjalan di dalam sistem operasi yang berbeda.
### Yang dapat dilakukan di server-side
- Penyimpanan dan pengiriman informasi yang efisien
- Mengkostumisasi UX
- Akses terkontrol ke konten
- Store session/state information
- Notifikasi dan komunikasi
- Data analysis

## RESTful API
### Pengertian REST
- REST, atau REpresentational State Transfer, adalah gaya arsitektur untuk menyediakan standar antara sistem komputer di web, sehingga memudahkan sistem untuk berkomunikasi satu sama lain.
- Sistem yang sesuai dengan REST, sering disebut sistem RESTful, dicirikan oleh bagaimana mereka tidak memiliki kewarganegaraan dan memisahkan masalah klien dan server
### Komunikasi antara Klien dan Server
- Membuat Requests
  REST mengharuskan klien membuat permintaan ke server untuk mengambil atau mengubah data di server. Permintaan umumnya terdiri dari:
    - kata kerja HTTP, yang mendefinisikan jenis operasi apa yang harus dilakukan
    - Header, yang memungkinkan klien untuk menyampaikan informasi tentang permintaan jalan menuju sumber daya
    - jalan menuju sumber daya
    - badan pesan opsional yang berisi data
- Kata Kerja HTTP
  - Ada 4 kata kerja HTTP dasar yang digunakan dalam permintaan untuk berinteraksi dengan sumber daya dalam sistem REST
    1. GET — mengambil resource tertentu (berdasarkan id) atau kumpulan sumber daya
    2. POST — membuat resource baru
    3. PUT — memperbarui resource tertentu (berdasarkan id)
    4. DELETE — menghapus resource tertentu dengan id
### Parameter Headers dan Accept
- Di header permintaan, klien mengirimkan jenis konten yang dapat diterimanya dari server. Ini disebut bidang Terima, dan ini memastikan bahwa server tidak mengirim data yang tidak dapat dipahami atau diproses oleh klien.
- Tipe lain dan subtipe yang umum digunakan :
  - image — image/png, image/jpeg, image/gif
  - audio — audio/wav, audio/mpeg
  - video — video/mp4, video/ogg
  - application — application/json, application/pdf, application/xml, application/octet-stream

### Response Codes
- Untuk setiap kata kerja HTTP, ada kode status yang diharapkan yang harus dikembalikan server setelah berhasil :
  1. GET — return 200 (OK)
  2. POST — return 201 (CREATED)
  3. PUT — return 200 (OK)
  4. DELETE — return 204 (NO CONTENT) 
 
# Intro Node.Js
Node.js adalah open-source, lintas platform, back-end Javascript yang berjalan pada V8 engine dan mengeksekusi kode JavaScript di luar browser web. Node.js memungkinkan pengembang menggunakan JavaScript untuk menulis command line tools dan untuk skrip sisi server—menjalankan skrip sisi server untuk menghasilkan konten halaman web dinamis sebelum halaman dikirim ke browser web pengguna.
## Node JS Architecture
- **Single Thread**
  - Thread dalam ilmu komputer adalah eksekusi menjalankan beberapa tugas atau program secara bersamaan. Setiap unit yang mampu mengeksekusi kode disebut thread. Javascript menggunakan konsep single thread, yang berarti hanya memiliki satu tumpukan panggilan yang digunakan untuk menjalankan program.
- **Even Loop**
  - Dengan menggunakan konsep arsitektur javascript, walaupun menggunakan single thread tetapi kita dapat melihat javascript seperti menggunakan multi thread
  - Terdapat event queue yang berguna sebagai penampung ketika terdapat perintah baru yang akan dieksekusi.
  - Event loop akan memfasilitasi kondisi ini, event loop akan memeriksa terus menerus, ketika antrian kosong di call stack maka akan menambah antrian baru dari event queue sampai semua perintah selesai di eksekusi.
- **Server side scripting**
  - Sejatinya javascript merupakan bahasa pemrograman yang digunakan di front end side. Sehingga kita hanya bisa mengerjakan javascript dengan menggunakan browser untuk menampilkan hasil eksekusinya. Tetapi dengan menggunakan NodeJS kita dapat menjalankan javascript di server side menggunakan terminal command line menggunakan perintah “node”.
## Javascript For Node JS
- **Arrow Expression**
  Arrow expression merupakan fitur terbaru dari javascript, yaitu mempermudah membuat sintaks function menggunakan “=>”
- **Asynchronous**
  Asynchronous merupakan konsep yang paling penting dari javascript. Pada dasarnya, javascript mengeksekusi code secara single thread dan berurutan baris per baris yang disebut dengan synchronous. Sedangkan asynchronous memungkinkan mengeksekusi code tanpa berurutan dengan cara “skip” code dan melanjutkan eksekusi code selanjutnya. Konsep ini menungkinkan code kita tidak terjadi blocking dan lebih efisien.
- **JSON**
JSON atau Javascript Object Notation merupakan format yang digunakan untuk menyimpan dan mengirim data menggunakan konsep object di javascript. JSON dapat digunakan di hampir semua bahasa pemrograman sehingga sangat cocok untuk dipelajari

## Membuat Web Server Dengan Node JS
- **Node JS Web Server**
  - Node.js memiliki built-in modul yang disebut HTTP, built-in modul ini memungkinkan Node JS mentransfer data melalui Hyper Text Transfer Protocol (HTTP).
  - Modul HTTP dapat membuat server HTTP yang mendengarkan port server dan memberikan respons kembali ke klien.
  - Untuk menggunakan modul HTTP, gunakan require()
  - Gunakan method createServer() untuk membuat server HTTP
  - Callback function yang digunakan pada method http.createServer(), akan dijalankan ketika seseorang mencoba mengakses komputer pada port 8080.
  - Contoh :
    ```
    const http = require('http')
    
    http.createServer(function(req, res) => {
      res.write('Hello World')
      res.end()
    }).listen(8080)
    ```
# Express.js
- Express.js adalah framework web app untuk Node.js yang ditulis dengan bahasa pemrograman JavaScript. Framework open source ini dibuat oleh TJ Holowaychuk pada tahun 2010 lalu.
- Express.js adalah framework back end. Artinya, ia bertanggung jawab untuk mengatur fungsionalitas website, seperti pengelolaan routing dan session, permintaan HTTP, penanganan error, serta pertukaran data di server.
## Installation and Preparation Express.js
- Karena expressJS adalah sebuah modules atau package yang dikembangkan menggunakan bahasa javascript, maka kita bisa menggunakan NPM untuk menginstall express JS
 ```js
 npm install express --save
 ```
- Terdapat beberapa module yang perlu diinstal untuk mempermudah develop server side application, seperti nodemon (agar dapat restart application otomatis selama proses development)
```js
npm install --save-dev nodemon
```
## Method ExpressJS
Kita dapat menggunakan method dalam REST API seperti `GET`,`POST`, `PUT`, `PATCH` dan `DELETE`

## Response ExpressJS
- Kita dapat mengirim response berupa output json yang biasa dipakai untuk back end application. Dengan menggunakan output json maka kita dapat mengirim data yang mudah diakses.
- Objek `res` mewakili respons HTTP yang dikirim oleh aplikasi Express saat mendapat permintaan HTTP.
- Dalam dokumentasi ini dan menurut konvensi, objek selalu dirujuk sebagai `res`(dan permintaan HTTPnya adalah `req`) tetapi nama sebenarnya ditentukan oleh parameter ke fungsi panggilan balik tempat Anda bekerja.
- Sebagai contoh:
  ```js
  app.get('/user/:id', function (req, res) {
    res.send('user ' + req.params.id)
  })
  ```
  Di dalam route kita dapat mengirim response menggunakan parameter dari route express.js yaitu `res.Send()` untuk mengirim plain text ketika kita mengakses route tersebut.
- Properties
  - `res.app`
  - `res.headersSent`
  - `res.locals`
- Methods
  - `res.append()`
  - `res.attachment()`
  - `res.cookie()`
  - `res.clearCookie()`
  - `res.download()`
  - `res.end()`
  - `res.format()`
  - `res.get()`
  - `res.json()`
  - `res.jsonp()`
  - `res.links()`
  - `res.location()`
  - `res.redirect()`
  - `res.render()`
  - `res.send()`
  - `res.sendFile()`
  - `res.sendStatus()`
  - `res.set()`
  - `res.status()`
  - `res.type()`
  - `res.vary()`
  
## Nested route
Nested route digunakan ketika terdapat banyak route yang memiliki nama yang sama atau ingin membuat route yang lebih mendalam
## Express Middleware
- Apa Itu Middleware ?
  - `Middleware function` adalah sebuah fungsi yang memiliki akses ke `object request (req)`, `object response (res)`, dan sebuah `fungsi next` didalam request-response cycle.
- `Fungsi next` biasanya di berikan nama variable next.
### Bagaimana Cara Middleware Bekerja?
Secara umum, prinsip kerja Middleware adalah mencegat request yang masuk untuk kemudian diproses terlebih dahulu sebelum diberikan kepada Controller yang dituju atau diarahkan ke Controller yang lain. Dengan menggunakan fitur ini, kita dapat membuat komponen yang reusable untuk melakukan pekerjaan-pekerjaan tersebut.
### Apa Saja Yang Bisa Dilakukan Oleh Function Middleware?
- Menjalankan kode apapun.
- Memodifikasi Object Request dan Object Response.
- Menghentikan request-response cycle.
- Melanjutkan ke middleware function selanjutnya atau ke handler function dalam suatu request response cycle.
### Jenis Express Middleware
- Berdasarkan Cara Penggunaan
  - Application Level Middleware
  - Router Level Middleware
  - Error Handling Middleware
- Berdasarkan Cara Penggunaan : Application Level Middleware
  - Application Level Middleware adalah sebuh function middleware yang melekat ke instance object Application Express.
  - Penggunaannya dengan cara memanggil method app.use().
  - Application Level Middleware akan di jalankan setiap kali Express Application menerima sebuah HTTP Request.
- Berdasarkan Cara Penggunaan : Router Level Middleware
  - Router Level Middleware adalah sebuh function middleware yang cara kerjanya sama persis dengan application level middleware, yang menjadikan perbedaan adalah middleware function ini melekat ke instance object Router Express.
  - Penggunaannya dengan cara memanggil method express.Router().
  - Router Level Middleware hanya akan di jalankan setiap kali sebuah Express Router yang menggunakan middleware ini menerima sebuah HTTP Request, sedangan pada Router yang lain tidak akan dijalankan.
- Berdasarkan Source Middleware Function
  - Express Build-in Middleware
    - express.static()
    - express.json()
    - express.urlEncoded()
    - Third Party (custom) Middleware
# Design Database with MySQL
## Entity / Entitas
adalah kumpulan objek yang dapat diidetifikasikan secara unik atau berbeda. Biasanya simbol dari entitas adalah persegi panjang
## Atribut
 berfungsi untuk mendeskripsikan karakteristik dari entitas tersebut. Simbol dari atribut adalah elips
## Relasi
adalah hubungan antara entitas
## Apa Itu Primary Key Dan Foreign Key Di SQL Database?
- Primary key adalah tanda pengenal unik yang membedakan satu record dari yang lain. Oleh karena itu, setiap record dalam SQL database management system harus memiliki primary key.
- ada beberapa aturan yang harus kalian ikuti ketika menentukan primary key untuk tabel:
  - Primary key harus berisi nilai unik
  - Kolom primary key tidak boleh berisi nilai NULL
  - Sebuah tabel hanya memiliki satu primary key
- Foreign key adalah pengenal unik atau kombinasi pengenal unik yang menghubungkan dua tabel atau lebih dalam database.
  <br>Saat memutuskan tabel mana dalam database relasional yang harus memiliki foreign key, harus terlebih dahulu mengidentifikasi tabel mana yang merupakan subjek dan objek dalam hubungannya.
## Perbedaan Primary Key Dan Foreign Key
- Tidak ada dua baris yang dapat memiliki value identik untuk primary key sedangkan Foreign key dapat berisi value duplikat.
- Tidak ada batasan dalam memasukkan value ke dalam kolom tabel primary key ssedangkan Saat memasukkan value apa pun dalam tabelforeign key, pastikan bahwa value tersebut ada di kolom primary key.
- dapat memiliki satu primary key dalam sebuah tabel sedangkan foreign key dapat memiliki beberapa dalam satu tabel.
## Unnormalized Form
 Unnormalized Form adalah suatu kondisi dimana sebuah tabel yang memiliki rangkap atau data yang terduplikasi. Unnormalized Form ini sebenarnya adalah kumpulan data data mentah yang dimasukkan semua dalam satu tabel yang sama (tidak dipecah ke tabel lain). Data tersebut di input dengan apa adanya dan tidak dipilah sesuai dengan jenisnya.
## NORMALISASI
proses pengelompokan atribut data yang membentuk entitas sederhana, nonredundan, fleksibel, dan mudah beradaptasi, Sehingga dapat dipastikan bahwa database yang dibuat berkualitas baik.