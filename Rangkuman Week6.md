# **Rangkuman Week 6**


#### BackEnd Development
- BackEnd adalah bagian belakang layar dari sebuah website atau aplikasi, yang secara teknologi backend merupakan sisi server dari sebuah website atau aplikasi
- Back-End Developers dapat memilih banyak bahasa pemrograman dan framework, tergantung jenis aplikasi apa yang akan dibuat. Contoh dari bahasa pemrogramannya : C Java C++ Python Javascript Rust Golang

#### Databases
- Database adalah kumpulan data yang disimpan secara sistematis di dalam komputer yang dapat diolah dan dimanipulasi atau sebagai gudang penyimpanan data untuk diolah lebih lanjut.Relational Non-Relational

#### API
- API adalah sekumpulan intruksi program dan protokol yang digunakan untuk membangun aplikasi perangkat lunak
- Rest API sebagai penghubung/perantara antara Front End dengan Back End untuk saling bertukar informasi(request dan response)


#### MERN Stack
- MERN adalah salah satu kombinasi teknologi antara Front End dan Back End untuk membuat aplikasi website
- MERN adalah singkatan dari MongoDB, Express, React, dan NodeJS. Teknologi Full-stack yang menggunakan 1 bahasa yaitu Javascript
- Beberapa alasan mengapa menggunakan MERN stack :
Segala kegiatan pengembangan menggunakan bahasa Javascript
Mendukung arsitektur MVC (Model View Controller) untuk membuat proses pengembangan lebih lancar dan terstruktur
Dengan menggunakan Javascript, maka developer hanya perlu menguasai Javascript dan JSON
Open source framework dengan dukungan komunitas yang besar dan baik

### Database

#### Introduction
- Database adalah kumpulan informasi yang disimpan dalam komputer secara sistematik dan saling berelasi
- Database merupakan sekumpulan tabel yang berisikan informasi untuk diolah yang kemudian data tersebut bisa digunakan didalam sebuah sistem
- Membuat database diperlukan software DBMS(Databases Management System)

#### Database Management System
- DBMS adalah software yang dapat digunakan oleh user untuk berkomunikasi dengan data yang ada dalam media penyimpanan
- Tipe utama pada Database management system antara lain Hierarchical Network, Relational, Non Relational, dan Object Oriented


#### Istilah pada Database
### Table
- Table adalah kumpulan value yang dibangun oleh baris dan kolom, yang didalamnya berisikan atribut dari sebuah data
Field
- Field adalah kolom dari sebuah tabel dimana masing-masing field memiliki tipe data masing-masing
Record
- Record merupakan kumpulan nilai yang saling terkait, yang merupakan isi dari sebuah tabel
SQL
- SQL atau Structured Query Language merupakan suatu bahasa yang digunakan untuk mengakses databases
- Membuat, menampilkan, dan menghapus data didalam database
- Mengatur “Permission” (siapa saja yang bisa mengakses data)
- Membuat dan menghapus database
DDL
- DDL merupakan kumpulan perintah SQL yang digunakan untuk membuat, mengubah, dan menghapus struktur dan definisi metadata dari objek-objek database
‘CREATE TABLE “nama tabel’
ALTER
- Alter digunakan untuk mengubah struktur dari tabel yang ada, seperti untuk menambahkan atau menghapus kolom
- Membuat atau menghapus primary key, mengubah jenis kolom yang ada, juga mengubah kolom atau nama tabel
‘ALTER TABLE nama_table ADD Primary key(nama_field)’
DROP
- Drop digunakan untuk menghapus database, tabel, dan view atau index
‘DROP DATABASE Nama_Database’
DML (Data Manipulation Language)
- SELECT
Perintah SELECT digunakan untuk menyeleksi data berdasarkan syarat yang diberikan. Dengan menggunakan SELECT record dalam tabel tertentu yang berjumlah ribuan bahkan jutaan dapat ditampilkan
‘SELECT * FROM nama_tabel’
- INSERT
Insert digunakan untuk memasukkan data ke kolom-kolom yang terdapat pada tabel/view
‘INSERT INTO nama_table VALUES (value1, value2,... , valueN)’
Where, And, Or, Not, Like
‘WHERE condition1 AND condition2 OR condition3 NOT condition4’
- UPDATE
Update digunakan untuk melakukan editing pada isi dari kolom yang dipilih untuk memperbaiki data lama/terjadi kesalahan
‘UPDATE nama_table SET nama_kolom = “data baru” WHERE id = 1;’
-DELETE
Delete digunakan untuk menghapus data dalam tabel yang menjadi target
‘DELETE FROM nama_tabel WHERE condition;’
DCL (Data Control Language)
- GRANT
Grant digunakan untuk memberikan hak akses pada user
- REVOKE
Revoke digunakan untuk mencabut hak akses yang telah diberikan pada user
Database Relationships
- Database relationships adalah relasi atau hubungan antara beberapa tabel dalam bahasa yang kita miliki
- Relasi antar tabel dihubungkan oleh Primary Key dan Foreign Key
- Primary Key adalah atribut yang tidak hanya mengidentifikasi secara unik suatu kejadian, tetapi juga mewakili setiap kejadian suatu entitas (NIM Mahasiswa)
- Foreign Key adalah atribut yang melengkapi relationship dan menunjukan hubungan antara tabel induk dengan tabel anak
##### Tipe Database 
One to One Relationship adalah hanya satu dari masing-masing entity yang saling berhubungan atau berelasi
One to Many and Many to One Relationship adalah dimana satu atribut dari satu entity bisa berhubungan dengan dua atau lebih atribut dari entity yang lain
Many to Many Relationship adalah relasi antar table dimana banyak dari masing-masing record tersebut memiliki banyak relasi ke tabel lainnya
SQL Table Join
Join adalah penggabungan tabel yang dilakukan melalui kolom tertentu yang memiliki nilai terkait untuk mendapatkan satu set data dengan informasi lengkap
- Inner Join adalah menampilkan data hanya yang sesuai di kedua tabe;
- Left Join adalah menampilkan semua data sebelah kiri dari tabel yang di joinkan dan menampilkan data sebelah kanan yang cocok dengan kondisi join
- Right Join adalah menampilkan semua data sebelah kanan dari tabel yang di joinkan dan menampilkan data sebelah kiri yang cocok dengan kondisi join
No SQL
- Database NoSQL adalah database yang tidak memiliki perintah SQL. Konsep penyimpanannya semi struktural atau tidak struktural dan tidak harus memiliki relasi seperti pada tabel di MySQL
- Tujuan dari NoSQL adalah untuk model data spesifik dan memiliki skema fleksibel dalam mengembangkan aplikasi modern seperti aplikasi yang bersifat real time
##### Kelebihan NoSQL dibandingkan Relasional Database
NoSQL bisa menampung data yang terstruktur, semi terstruktur dan tidak terstruktur
Menggunakan OOP dalam pengaksesan/manipulasi data
NoSQL tidak mengenal skema tabel yang kaku
Document Database
- Document adalah salah satu dari beberapa model database NoSQL yang artinya penyimpanan data dan proses manipulasinya dalam bentuk objek dokumen seperti penerapan pada pemrograman format JSON
### MySQL - Basic


#### Database
- Database adalah kumpulan terorganisir dari informasi terstruktur, atau data, biasanya disimpan secara elektronik dalam sistem komputer. 
- Sebuah database biasanya dikendalikan oleh sistem manajemen database (DBMS). Bersama-sama, data dan DBMS, bersama dengan aplikasi yang terkait dengannya, disebut sebagai sistem basis data, sering disingkat menjadi basis data saja.

#### DBMS (Database Management System)
- Sebuah database biasanya memerlukan program perangkat lunak database yang komprehensif yang dikenal sebagai sistem manajemen database (DBMS). 
- Sebuah DBMS berfungsi sebagai antarmuka antara database dan pengguna akhir atau program, memungkinkan pengguna untuk mengambil, memperbarui, dan mengelola bagaimana informasi diatur dan dioptimalkan. 
- DBMS juga memfasilitasi pengawasan dan pengendalian basis data, memungkinkan berbagai operasi administratif seperti pemantauan kinerja, penyetelan, serta pencadangan dan pemulihan.

#### MySQL
- MySQL adalah sistem manajemen basis data relasional open source berbasis SQL. Itu dirancang dan dioptimalkan untuk aplikasi web dan dapat berjalan di platform apa pun. 
- Sebagai persyaratan baru dan berbeda muncul dengan internet, MySQL menjadi platform pilihan untuk pengembang web dan aplikasi berbasis web.



## Authentication dan Authorization
### Authentication
- Authentication adalah untuk memverifikasi siapa kamu.
- Otentikasi bergantung pada satu atau lebih faktor untuk memverifikasi identitas, dan faktor-faktor ini datang dalam tiga jenis utama :
  - Pengetahuan adalah sesuatu yang Anda ketahui, seperti nama pengguna dan kata sandi.
  - Kepemilikan adalah sesuatu yang Anda miliki, seperti kartu keamanan atau perangkat seluler
  - Inheren adalah sesuatu tentang Anda, yang umumnya mengacu pada data biometrik seperti sidik jari.
### Variasi Authentication
- Single-Factor Authentication
- Multi-Factor Authentication

## Authorization
- Authorization adalah verifikasi atas apa yang boleh anda lakukan.
- Authorization sangat penting untuk keamanan web, dan bertanggung jawab atas segala hal mulai dari mencegah pengguna memodifikasi akun satu sama lain, melindungi aset back-end dari penyerang, hingga memberikan akses terbatas ke layanan eksternal.
- Otorisasi yang baik akan memungkinkan Anda membatasi pengguna dan layanan untuk hak istimewa yang mereka butuhkan, hanya karena seorang pengguna berwenang untuk mengelola satu grup tidak berarti mereka harus dapat mengelola semua grup, misalnya.

## Perbedaan Authentication, Authorization, dan Encryption
- Authentication, proses membuktikan identitas seseorang sebelum mencoba untuk mendapatkan akses ke resource tujuan.
- Authorization, proses memberikan izin kepada pengguna untuk mengakses resource.
- Encryption, Enkripsi adalah proses teknis yang mengonversikan informasi menjadi kode rahasia, sehingga mengaburkan data yang Anda kirim, terima, atau simpan

## Membuat Authentication dan Authorization

# Sequelize 
## Peserta mampu memahami dan menggunakan Sequalize
- Sequelize adalah ORM (Object Relational Mapping) Node JS yang berbasis promise. Sequelize mendukung sebagian besar relational Database seperti MySQL, PostgresQL, MariaDB, SQLite dan Miscrosoft SQL Server.
- Dengan fitur fitur di Sequelize, kita bisa mengelola dan mengatur data di database kita dengan cepat, dan efisien
## Instalasi Sequelize
> Dengan mengetikan `npm install -g sequelize-cli` untuk mengintstall Sequwlize-cli
> Dengan mengetikkan `npm install --save sequelize` lalu `npm install --save sql` untuk menginstall sequelize