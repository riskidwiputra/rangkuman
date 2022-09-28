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
    
    ##### Setelah menginstal git lakukan setup awal
    &nbsp;
    ```markdown
    git config --global user.name "FaizalRajib"
    git config --global user.email "muhfaizalrajib@gmail.com"
    ```
 - git init <nama_proyek>, untuk membuat repositori baru
    ```markdown
     git init rangkuman
    Initialized empty Git repository in C:/xampp/htdocs/git/rangkuman/.git/ //return yang akan dihasilka 
    ```
 -  git status, untuk lacak perubahan
    ```markdown
    git status
    On branch master
    No commits yet
    Untracked files:
    (use "git add <file>..." to include in what will be committed)
        Rangkuman Week1.md
    ```

 - git add ,Untuk menyimpan perubahan file 
    ```markdown
    git add . 
    ```

  - git commit, untuk melakukan commit atau menyimpan perubahan pada version control pada git. Dan kita bisa menambahkan pesan untuk membeikan checkout pada setiap perbuahan. contohnya "git commit -m "pesan checkout"

       ```markdown
     git commit -m "rangkuman pertama"
    [master (root-commit) 3206437] rangkuman pertama
    1 file changed, 440 insertions(+)
    create mode 100644 Rangkuman Week1.md
    ```
 - git remote, menambahkan remote di dalam repository lokal
    ```markdown
    git remote add origin https://github.com/riskidwiputra/rangkuman.git
    ```
  - git push origin, untuk mempublish file atau aplikasi ke github

    ```markdown
    git push origin master
    Enumerating objects: 3, done.
    Counting objects: 100% (3/3), done.
    Delta compression using up to 8 threads
    Compressing objects: 100% (2/2), done.
    Writing objects: 100% (3/3), 4.47 KiB | 4.47 MiB/s, done.
    Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
    To https://github.com/riskidwiputra/rangkuman.git
    * [new branch]      master -> master
    ```
    Biasaya ketika belum pernah menghubungkan github di git local kita biasanya akan diminta Authorize Git ini hanya akan diminta 1 kali saja 
    ![git-clone](<https://i.ibb.co/NZZHGnP/gac.png>)
  - git clone, untuk melakukan cloning dari github ke komputer atau local
    ```markdown
        git clone https://github.com/riskidwiputra/rangkuman.git
    ```

  ## HTML (HyperText Markup Language) (20 September 2022)

- Definisi HTML

    Merupakan bahasa komputer yang digunakan untuk membuat kerangka atau struktur untuk Web pages (halaman website) di internet. Digunakan akan memberitahu browser bagaimana cara menampilkan sebuah konten.


- Kerangka HTML

  HTML memiliki sebuah kerangka seperti gambar dibawah ini

  ```html
    <html>
    	<head>
        	<title>Document</title>
    	</head>
    	<body>
    	Isi Konten
    	</body>
    </html>
    ```
-  Html Comment
   ```html
   <!-- ini adalah syntax comment html -->
   <p style="color: red;">Belajar Bersama Skilvul</p> 
   ```
   Dengan menggunakan HTML Comment, kita dapat memberikan penjelasan maksud dari line code yang kita kerjakan atau bisa digunakan untuk mematikan code.




###   contoh tag HTML

  - Tag untuk membuat tulisan tebal dan miring

    ```html
    <b>Tebal</b> <i>Miring</i>
    ```


  - Tag HTML Untuk Membuat tulisan dengan link

    ```html
    <a href="">Welcome To AMMAN Coding Bootcamp BATCH 3</a>
    ```


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

    - Unordered List

      ```html
      <ul>
        Dafunda
        <li>Dafunda Tekno</li>
        <li>Dafunda Otaku</li>
        <li>Dafunda Games</li>
      </ul>
      ```

  - Tag HTML Untuk Menampilkan gambar

    ```html
    <img src="https://bit.ly/2FKluzq" alt="Si Kucing"></img>
    ```
    
    - ### **Semantic Html**
      Semantic HTML yaitu menggunakan elemen HTML sesuai dengan kebutuhan konten. Contoh yaitu header, footer, nav, section, aside, dll.
    
      ```html
          <body>
        
          <header>
            <h1>My Blog</h1>
          </header>
        
          <nav>
            <a href="#">Home</a> |
            <a href="#">About</a> |
            <a href="#">Contact</a>
          </nav>
        
          <article>
            <h1>Welcome To My Blog!</h1>
            <p>Perkenalkan nama saya Rizky dwi putra lubis . Biasa dipanggil rizky. Saat ini aku tenggah mengikuti Studi Independen Program Skilvul Tech4Impact: Back-end Web Development. 
            </p>
          </article>
        
          <footer>
            Copyright &copy; 2022 by Rizky Dwi putra
          </footer>
        
          </body>
        ```
    &nbsp;

## CSS (Cascading Style Sheets) (21 September 2022)

- Definisi CSS

  CSS adalah  bahasa yang digunakan untuk mendesain halaman website.dan biasanya digunakan untuk mengatur tampilan elemen yang tertulis dalam bahasa markup, seperti HTML. Kita ibaratkan HTML adalah kerangka yang memberi sturuktur pada website, maka CSS adalah baju yang memberi warna dan layout pada website.

- Cara Menggunakan CSS

  #### 1. Inline Styles

     Kita menambahkann CSS langsung pada atribut HTML

     ```html
     <p style="color:red">Tulisan ini berwarna merah</p>
     ```

  #### 2. Internal CSS

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

  #### 3. Eksternal CSS

     Kita akan menyisipkan kode CSS dengan cara membuat file CSS terpisah, dan lalu menyambungkannya dengan file HTML dengan menggunakan element <link>. Element <link> tersebut diletakkan di dalam element <head>

     Contoh:

     Kita memiliki dua file: index.html untuk file HTML-nya dan styles.css untuk file CSS-nya.

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
 - ### **CSS Class Name**

    Cara menggunakan attribute class pada elemen HTML yaitu dengan cara memanggil nama class tersebut pada file CSS

      ```html
      <!-- File Html -->
      <h1 class="title">My Profile</h1>
      ```

      ```css
      <!-- File Css -->
      .title {
        color : aqua;
      }
      ```
- ### **CSS - ID Name**

  Berbeda dengan Class Name. ID Name bersifat unik artinya hanya ada 1 nama ID pada 1 element HTML.

  ```html
  <!-- File Html -->
  <p id="paragrafSatu">Namaku Krizz</p>
  ```
  ```css
  <!-- File Css -->
  #paragrafSatu {
    border: solid red;
  }
  ```

## Algoritma dan Introduction JavaScript (22 September 2022)

- ### Algoritma

  - Algortima Adalah deskripsi berupa step-step yang dibutuhkan untuk menyelesaikan suatu masalah. Untuk menyelesaikan suatu masalah, tentunya kita harus mempunyai data struktur, nah data inilah yang akan kita gunakan untuk menyelesaikan suatu masalah dengan menggunakan algoritma.



  - Mengapa kita memerlukan algoritma?

    Manfaat algoritma antara lain:

    - Membantu menyederhanakan suatu program yang rumit dan juga besar.
    - Mempermudah pembuatan program yang dapat menyelesaikan masalah tertentu.
    - Membantu menyelesaikan suatu masalah dengan logika dan juga sistematis.

    Algoritma sederhana dalam bahasa pemrograman javascript.
    ```javascript
        let angka = 2;
        let hasil;

        hasil = angka * 5;
        console.log(hasil);
    ```
    Algoritma sederhana dalam kehidupan sehari-hari.
    ```javascript
        1. Pergi ke kekamar
        2. Berangkat ke kampus
    ```
  &nbsp;
  - ### Javascipt Dasar
    __JavaScript__ merupakan bahasa pemrograman yang digunakan untuk membuat web menjadi lebih interaktif dan responsive.
    Untuk menjalankan javascript pada umumnya menggunakan web browser seperti Chrome, Microsoft Edge, Mozila Firefox, kalau pakai code editor Visual Studio Code bisa di bagian console.

    Adapun Macam - macam Tipe Data di JavaScript :
    - `String`
    - `Number`
    - `Boolean`
    - `Object`
    - `Array`
    ### Penggunaan Javascript 
    Hal yang pertama harus kita lakukan pada penggunaan javascript adalah menghubungkan HTML dengan Javascript karena JS bukanlah bahasa pemograman yang bisa berdiri sendiri. `<script src = "Script.js"></script> ` javascript siap digunakan. Pada bahasa pemograman ini terdapat beberapa operator dasar yang wajib dipahami bagi seseorang developer yaitu
    
     &nbsp;
     
    ## Js Dasar Condicional dan Looping (23 September 2022)
    __Conditional__ merupakan statement percabangan yang menggambarkan suatu kondisi, statement akan mengecek kondisi spesifik dan menjalankan perintah berdasarkan kondisi tersebut. Yang dicek adalah apakah kondisi tersebut TRUE (benar).
    Adapun beberapa kondisi javascipt:
    - `Kondisi if`  untuk mengeksekusi suatu kumpulan perintah apabila kondisi tertentu bernilai true
    - `Kondisi else`   untuk mengeksekusi suatu kumpulan perintah apabila kondisi tertentu bernilai false
    - `Kondisi else if`  untuk pemeriksaan kondisi berikutnya apabila kondisi sebelumnya bernilai false
    - `Kondisi switch`  untuk mengeksekusi suatu kumpulan perintah berdasarkan beberapa pilihan
    
     &nbsp;
    **Penulisan IF**
    ```
    	if (umur < 30) {
          return "anda sudah Dewasa";
        }
    ```
    
    **Penulisan Else**
    ```
    	if (umur < 30) {
          return "anda sudah Dewasa";
        } else {
           return "anda masih dibawah umur";
        }
    ```
    **Penulisan Else if**
    ```
         if (umur < 30) {
          return "anda sudah Dewasa";
        } else  if (umur < 18) {
            return "anda sudah remaja";
        } else {
          return "anda masih dibawah umur";
        }
    ```
    **Penulisan Else if**
    ```
         if (umur < 30) {
          return "anda sudah Dewasa";
        } else  if (umur < 18) {
            return "anda sudah remaja";
        } else {
          return "anda masih dibawah umur";
        }
    
    ```
    **Penulisan Else if**
     ```
            switch (grade) {
               case 'A': 
                return "Nilai anda luarbiasa";
               break;
               case 'B': 
                   return "Nilai anda sangat bagus";
               break;
               case 'C':
                   return "nilai anda cukup";
               break;
               case 'D': 
                 return "nilai anda buruk";
               break;
               case 'F': 
                 return "nilai sangat anda buruk";
               break;
               default:  
                    return "tidak dikenal";
            }
     ```
     &nbsp;
     
      __Looping__ adalah statement yang mengulang atau perulangan sebuah instruksi hingga kondisi terpenuhi atau jika kondisi stop atau berhenti tercapai. Misal menggunakan perulangan For Loop contoh statement
      
      for loop memiliki aturan tersendiri dalam penulisannya
    ```
        for(initialization; condition; post-expression){
            
        }
    ```
    
    contoh penggunaan for loop 
    ```
        let angka = 1;
        for (angka; angka <= 10; angka++){
            console.log(angka);
        }
        //outputnya : 1 2 3 4 5 6 7 8 9 10
    ```
 

  
