# **Rangkuman Week1**

  ## Unix Command Line & Git & GitHub (19 September 2022)

 "Command Line" atau "Command Line Interface" sebenarnya yang dimaksud adalah shell 
 dan kalau menggunakan windows itu namanya command prompt untuk memiliki CLI itu kita dapatkan ketika mendownload git dan unutk cmd sendiri itu sudah bawaan dari sistem operasi windows. untuk penggunaan cli yang kita dapat dari bash itu memilki command yang berbeda.
 ###### Adapun beberapa command yang dimiliki oleh Cli :
- ### Command

  - pwd (print working directory), untuk melihat current working directory
  - dir (directory), untuk melihat directory
  - cd (change directory), untuk pindah directory
  - ls (list), untuk melihat isi file di dalam directory
  - touch, untuk membuat file directory
  - cp (copy), untuk menyalin file directory
  - mv (move), untuk memindahkan file directory
  - rm (remove), untuk menghapus file directory

- ### Apa itu Git & Github
   #### Git
    Merupakan aplikasi/software yang dapat melacaks suatu perubahan yang terjadi di suatu folder ataupun file, yang biasanya digunakan oleh programmer sebagai tempat untuk menyimpan file programan mereka karena lebih efektif.

    #### Github
    Merupakan vendor penyedia layanan git.
	
  &nbsp;

  ### Mengapa wajib menggunakan Git & Github?

  Alasan utamanya adalah sepandai apapun programmer, tidak akan mampu untuk mengerjakan semuanya sendiri selamanya. Maka dari itu dengan menggunakan Git & Github akan memudahkan programmer untuk bisa bekerja sama dalam sebuah tim. Tujuan besarnya adalah programmer bisa berkolaborasi dengan programmer lainnya dengan mengerjakan proyek yang sama tanpa harus repot copy paste folder aplikasi yang terupdate.

&nbsp;

- ### Command di dalam Git & Github

 - git init <nama_proyek>, untuk membuat repositori baru
    ```markdown
     git init rangkuman
    Initialized empty Git repository in C:/xampp/htdocs/git/rangkuman/.git/ //return yang akan dihasilka 
    ```
 -  git status, untuk lacak perubahan
    ```markdown
    git status
    ```

 - Untuk menyimpan perubahan file 
    ```markdown
    git add . 
    ```

  - git commit, untuk melakukan commit atau menyimpan perubahan pada version control pada git. Dan kita bisa menambahkan pesan untuk membeikan checkout pada setiap perbuahan. contohnya "git commit -m "pesan checkout"

    ![git-commit1](<https://raw.githubusercontent.com/Jirjatss/week-1/main/gambar/git-commit1%20(1).jpg>)

  - git push origin, untuk mempublish file atau aplikasi ke github

    ![git-push](https://raw.githubusercontent.com/Jirjatss/week-1/main/gambar/git-push%20-%20Copy.JPG)

  - git clone, untuk melakukan cloning dari github ke komputer atau local

    ![git-clone](<https://raw.githubusercontent.com/Jirjatss/week-1/main/gambar/git-clone%20(1).JPG>)

## HTML

- Definisi HTML

  <div align="justify">Merupakan bahasa komputer yang digunakan untuk membuat kerangka atau struktur untuk Web pages (halaman website) di internet. Bagaimana peran HTML pada web development? Web browser seperti Chrome, Firefox, Edge, Safari, atau Opera akan membaca dokumen HTML. Dokumen HTML yang berisi tag-tag HTML akan memberitahu browser bagaimana cara menampilkan sebuah konten.

&nbsp;

- Kerangka HTML

  HTML memiliki sebuah kerangka seperti gambar dibawah ini

  ```html
  <html>
  <head>
  <title>
      Judul Website
    </title>
  <body>
      saya sedang belajar pemrograman HTML dasar.
    </body>
  </html>
  ```

    <div align="justify">Sintak diatas biasa disebut dengan kerangka bahasa pemrograman HTML. Didalam website selalu ada title untuk tiap-tiap web, untuk memasukkan title didalam web kamu harus mengetikkan diantara tag title (dapat diisikan dengan nama website kamu atau yang lainnya). Untuk memasukkan konten-konten, kamu dapat memasukkannya atau mengetikkannya didalam program tepat diantara tag body (Ganti titik-titik dengan konten).

  &nbsp;

- Tag HTML

  <div align="justify">Tag adalah sebauh penanda awalan dan akhiran dari sebuah elemen di HTML. Tag dibuat dengan kurung siku (<...>), lalu di dalamnya berisi nama tag dan kadang juga ditambahkan dengan atribut.

  &nbsp;

  <div align="justify">Tag selalu ditulis berpasangan. Ada tag pembuka dan ada tag penutupnya. Namun, ada juga beberapa tag yang tidak memiliki pasangan penutup. Tag penutup ditulis dengan menambahkan garis miring (/) di depan nama tag.

  &nbsp;

  Contoh tag HTML

  - Tag untuk membuat tulisan tebal dan miring

    ```html
    <b>Tebal</b> <i>Miring</i>
    ```

    Hasilnya di browser

    ![](gambar/tebal-miring.JPG)

  - Tag HTML Untuk Membuat tulisan dengan link

    ```html
    <a href="">Welcome To AMMAN Coding Bootcamp BATCH 3</a>
    ```

    Hasilnya di web browser

    ![](gambar/link.jpg)

  - Tag Untuk Membuat Daftar/List

    - Ordered List

      ```html
      <ol>
        Dafunda
        <li>Dafunda Tekno</li>
        <li>Dafunda Otaku</li>
        <li>Dafunda Games</li>
      </ol>
      ```

      Hasilnya di web browser

      ![](gambar/ol.jpg)

    - Unordered List

      ```html
      <ul>
        Dafunda
        <li>Dafunda Tekno</li>
        <li>Dafunda Otaku</li>
        <li>Dafunda Games</li>
      </ul>
      ```

      Hasilnya di web browser

      ![](gambar/ul.jpg)

  - Tag HTML Untuk Menampilkan gambar

    ```html
    <img src="https://bit.ly/2FKluzq" alt="Si Kucing"></img>
    ```

    Hasilnya di web browser

    ![](gambar/gambar.jpg)

    &nbsp;

- Deploy HTML

  <div align="justify">Deploy adalah sebuah proses untuk menyebarkan aplikasi yang sudah kita kerjakan supaya bisa digunakan oleh orang-orang. Jika aplikasi kita HTML atau Web App kita perlu mendeploy ke server. Untuk melakukan hal tersebut kita bisa menggunakan layanan yang bernama Netlify

## CSS

- Definisi CSS

  <div align="justify">CSS adalah bahasa komputer yang digunakan untuk menambahkan design ke suatu halaman website di internet agar terlihat lebih cantik/menarik. CSS adalah singkatan dari Cascading Style Sheets. Kita ibaratkan HTML adalah kerangka yang memberi sturuktur pada website, maka CSS adalah baju yang memberi warna dan layout pada website.

&nbsp;

- Cara Menggunakan CSS

  1. Inline Styles

     Kita menambahkann CSS langsung pada atribut HTML

     ```html
     <p style="color:red">Tulisan ini berwarna merah</p>
     ```

     ![](gambar/inline.jpg)

  &nbsp;

  2. Internal CSS

     Kita menggunakan element/tag `<style>` untuk menyisipkan kode CSS. element/tag `<style>` diletakkan di dalam element `<head>`

     ```html
     <!DOCTYPE html>
     <html>
       <head>
         <title>Website Pertamaku</title>
         <style>
           body {
             background-color: yellow;
           }
           h1 {
             color: blue;
           }
           p {
             color: red;
           }
         </style>
       </head>
       <body>
         <h1>Website Pertamaku</h1>
         <p>Selamat Datang</p>
       </body>
     </html>
     ```

     Tampilan dari sintaks diatas adalah

     ![](gambar/internal-css.jpg)

     &nbsp;

  3. Eksternal CSS

     <div align="justify">Kita akan menyisipkan kode CSS dengan cara membuat file CSS terpisah, dan lalu menyambungkannya dengan file HTML dengan menggunakan element <link>. Element <link> tersebut diletakkan di dalam element <head>

     Contoh:

     <div align="justify">Kita memiliki dua file: index.html untuk file HTML-nya dan styles.css untuk file CSS-nya.

     ```html
     <!-- File index.html -->

     <!DOCTYPE html>
     <html>
       <head>
         <title>Website Pertamaku</title>
         <link rel="stylesheet" href="styles.css" />
       </head>
       <body>
         <h1>Website Pertamaku</h1>
         <p>Selamat Datang</p>
       </body>
     </html>
     ```

     ```css
     /* File styles.css */

     body {
       background-color: pink;
     }
     h1 {
       color: blue;
     }
     p {
       color: black;
     }
     ```

     Tampilan dari sintaks diatas adalah

     ![](gambar/ekstenal-css.jpg)

     &nbsp;

- CSS Syntax

  <div align="justify">CSS Syntax adalah syntax yang digunakan untuk menunjuk atau memilih HTML element mana yang ingin diberi style (dihias). CSS syntax terdiri dari selector, property, dan value.

  Syntaxnya seperti ini:

  ```css
  p {
    color: blue;
  }
  ```

  Penjelasan :

  - p

    Adalah sebuah selector berupa element HTML yang akan diubah

  - color

    <div align="justify">Adalah sebuah properti berupa bagian mana dari element HTML yang akan diubah. Contoh diatas kita akan mengubah warna dari teks yang ada di element p

  - blue

    Adalah value yaitu nilai/hiasan berupa warna biru

  &nbsp;

## Algoritma dan Struktur Data

- Algoritma

  - <div align="justify">Algortima Adalah deskripsi berupa step-step yang dibutuhkan untuk menyelesaikan suatu masalah. Untuk menyelesaikan suatu masalah, tentunya kita harus mempunyai data struktur, nah data inilah yang akan kita gunakan untuk menyelesaikan suatu masalah dengan menggunakan algoritma.

  &nbsp;

  - Mengapa kita memerlukan algoritma?

    Manfaat algoritma antara lain:

    - <div align="justify">Membantu menyederhanakan suatu program yang rumit dan juga besar.
    - <div align="justify">Mempermudah pembuatan program yang dapat menyelesaikan masalah tertentu.
    - <div align="justify">Membantu menyelesaikan suatu masalah dengan logika dan juga sistematis.

  &nbsp;

  - Kualitas Algortima

    Kualitas wajib dari algoritma

    - <div align="justify">Input dan output harus didefinisikan terlebih dahulu dengan tepat
    - <div align="justify">Setiap step harus benar-benar clear dan tidak ambigu
    - <div align="justify">Algoritma seharusnya tidak mengandung suatu code pada bahasa pemograman tertentu.
    - <div align="justify">Algoritma harus dibuat agar dapat digunakan dalam bahasa pemograman apapun.

    &nbsp;

  - Penggunaan Algortima

    - Soal
      <div align="justify">Buatlah Algoritma untuk menyelesaikan problem ini

      David memiliki program yang membutuhkan untuk convert data dari jumlah jam ke detik

      Contohnya jika program memiliki input 2 jam maka output yang diharapkan adalah 7200 detik

    - Jawaban

      - Mulai
      - Deklarasi variabel n, hasil_convert
      - Menambahkan nilai n
      - <div align="justify">Melakukan proses (n jam = n \* 3600" lalu disimpan ke dalam hasil_convert
      - Menampilkan hasil convert (n jam) = + "detik"
      - Stop

    &nbsp;

- Pseudocode

  - <div align="justify">Pseudocode adalah menuliskan algoritma sebelum kita implementasikan ke bahasa pemograman tertentu.

    &nbsp;

  - Bagaimana menulis pseudocode

    - <div align="justify">Menggunakan HURUF BESAR pada kata kunci (key commands).

      CONTOH: IF number is > 10 THEN …

    - 1 statement = 1 baris
    - Gunakan indentasi
    - Simpel

    Contoh :

    ```md
    STORE "width" with any number
    STORE "height" with any nummber
    STORE "area" without any value

    CALCULATE "width" times "height"
    SET "area" value with calculation result
    DISPLAY "area"
    ```

    &nbsp;

  - Pseudocode berdasarkan kondisi masalah

    - Procedural

      Procedural adalah cara berpikir secara runtun. Artinya serangkaian perintah yang berurutan.

      Contoh :

      ```md
      STORE "width" with any number
      STORE "height" with any nummber
      STORE "area" without any value

      CALCULATE "width" times "height"
      SET "area" value with calculation result
      DISPLAY "area"
      ```

      &nbsp;

    - Conditional

      Conditional digunakan saat dibutuhkan percabangan kasus. Komputer akan melakukan suatu tindakan jika suatu kondisi terpenuhi.

      Jika hari ini tidak hujan, maka Bob pergi ke pasar,

      jika tidak maka Bob dirumah aja.

      ```md
      IF "bright"
      DO "go to the market"
      ELSE
      DO "stay at home"
      ```

    &nbsp;

    - Looping

      Komputer dapat melakukan sebuah proses yang sama berulang-ulang.

      Jika membutuhkan perulangan dalam kasus tertentu, kita bisa menggunakan Looping.

      Contoh :

      ```md
      STORE "count" t0 1

      WHILE "count" < 11
      DISPLAY "count"
      CALCULATE "count" mod 2
      STORE "reminder" value with calculation result
      IF "reminder" equals to 0
      DISPLAY "EVEN!"
      ELSE
      DISPLAY "ODD!"
      ```

      &nbsp;

    - Recursive

      Recursive adalah pola pikir dalam algoritma yang memanggil method/function didalam sebuah function
