# **Rangkuman Week3**


## Js Intermediate-Array and JS Intermediate-Multidimensional Array
Array adalah variable yang mempunyai index sehingga dapa menyimpan sebuah data yang bertipe sama. array juga data yang dapat menampung banyak data yang memiliki tipe data yang berbeda

Contoh Struktur array :

```javascript
        let nama = ["Rizky Dwi Putra"];
```
Varible yang mempunyai beberapa index yang dimulai dari index ke-0 dihitung dari kiri. Dan cara mengakses atau memanggil array sebagai berikut :

##### Length
Array memiliki properti length yang memberi tahu berapa banyak item dalam array dan diperbarui secara otomatis saat Anda menambahkan atau menghapus item ke array.
```
var arr = [];
arr[0] = "cat"; // this adds to the array
arr[1] = "mouse"; // this adds to the array
arr.length; // returns 2

arr["favoriteFood"] = "pizza";  
arr.length; // returns 2, not 3
```
##### forEach
Metode array Javascript forEach digunakan untuk mengulangi melalui array dan kemudian menjalankan fungsi panggilan balik pada setiap nilai pada array dan kemudian mengembalikan tidak terdefinisi

```
const array1 = ['a', 'b', 'c'];

array1.forEach(element => console.log(element));

// expected output: "a"
// expected output: "b"
// expected output: "c"

```

##### Map
metode membuat array baru yang diisi dengan hasil pemanggilan fungsi yang disediakan pada setiap elemen dalam array pemanggil.

```
const array1 = [1, 4, 9, 16];

// pass a function to map
const map1 = array1.map(x => x * 2);

console.log(map1);
// expected output: Array [2, 8, 18, 32]
```

##### Find
metode find mengembalikan elemen pertama dalam larik yang disediakan yang memenuhi fungsi pengujian yang disediakan. Jika tidak ada nilai yang memenuhi fungsi pengujian, undefined dikembalikan.

```
const array1 = [5, 12, 8, 130, 44];

const found = array1.find(element => element > 10);

console.log(found);
// expected output: 12

```


### JavaScript multidimensional array
Kita dapat menggunakan metode Array seperti push() dan splice() untuk memanipulasi elemen array multidimensi.

Array Multidimensi adalah array didalam array atau bisa dianalogikan dengan array of array.
contoh struktur dalam array multidimensi adalah
```
let nama =[
            [1, 21, 4 ],
            [2, 3, 4 ],
            [9, 20, 11 ],
    ];
```
Cara mengakses array multidimensi adalah :
```
    console.log(nama[0][2]);
    console.log(nama[1][1])
    console.log(nama[2][0])
```


### JS Intermeidiate-Object
Object adalah dalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method). Object kita dapat menyimpan properti dengan tipe data apapun.

contoh struktur object
```
let data = { 
        nama : 'Rizky`
        umur : 21,
        hobi : 'Bermain Game',
    }
```
Cara memanggil object dan mengaksesnya
```
  console.log(data)
    console.log(data.nama);
    console.log(data.umur);
    console.log(data.hobi);
```
Kita bisa mengubah data yang ada pada object melalui sebuah function dan memasukkan object sebagai parameter function. Pada real application nanti kalian pasti menemukan data object yang kompleks. Object yang berasal dari turunan object lainnya. Jika kita ingin menampilkan seluruh object properti. Kita bisa menggunakan looping. Jadi tidak perlu mengakses secara manual memanggil setiap propertinya.

### JS Intermeiadte-Recursive
Recursive adalah function yang memanggil dirinya sendiri sampai kondisi tertentu. Yang kebanyakan digunakan untuk case matematika, fisika, kimia, dan yang berhubungan dengan calculation.

Struktur rekursiv
```javascript
    function rekursiv(){
        if(){
        
        } else {
            rekursiv();
        }
        }
```

 Ciri - ciri rekursif sebagai berikut :
* Fungsi rekursif selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. Kondisi ini harus dapat dibuktikan akan tercapai, karena jika tidak tercapai maka kita tidak dapat membuktikan bahwa fungsi akan berhenti, yang berarti algoritma kita tidak benar.
    
* Fungsi rekursif selalu memanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya. Hal ini penting diingat, karena tujuan utama dari rekursif ialah memecahkan masalah dengan mengurangi masalah tersebut menjadi masalah-masalah kecil.

 Contoh penerapan rekursiv
```
        function deretAngka(n){
          if (n == 1) {
            console.log(n)
          } else {
            deretAngka(n-1)
            console.log(n);
          }
        }
        
        console.log(5)    
```

Rekursif ini bisa dilakukan dengan looping atau if statement.


### JS Intermeiadte-Asynchronous-Introduction and Promise

Asynchronous mengizinkan komputer memproses task yang lain sambil menunggu proses yang masih berlangsung. Yang artinya hanya dapat mengeksekusi satu task pada satu waktu atau biasa. Pada konsep pemrograman (web development pada case kita) dikenal istilah Asynchronous.

Membuat asynchronous secara simulasi artinya tidak murni asynchronous dengan beberapa cara: 
    * Callback
    * Promises
    * Async/Await

Callback function adalah function yang kita letakan di dalam argumen/parameter pada function, dan function tersebut akan dieksekusi setelah function pertama menyelesaikan tugasnya. 
```
        setTimeout(() => {
            console.log("B")
            }, 1000)

            console.log("C")
```
Promise adalah salah satu fitur baru di ES6, biasa digunakan untuk melakukan http request/fetch data dari API. 
```javascript
        let nontonPromise = new Promise((resolve, reject) => {
        if (true) {
            resolve("nonton terpenuhi") // berhasil
          } 
        reject("gagal"); // gagal
        });
```
     
Async - await adalah salah satu fitur baru dari javascript yang digunakan untuk menangani hasil dari sebuah Promise. Await berfungsi untuk menunda sebuah kode dijalankan sampai proses asynchronous berhasil.
```javascript
async function asyncNonton() {
try {
    let result = await nonton("jalan")
    console.log(result);
      } catch (error) {
            console.log(error)
      }
    }
    asyncNonton()
```
    
Fetch adalah native web API untuk melakukan HTTP calls dari external network.
```javascript
    fetch("https://digimon-api.vercel.app/api/digimon")
    .then(result => result.json())
    .then(result => {
      console.log(result)
    })
```
fetch() memiliki parameter utama yaitu URL/endpoint API, dan parameter kedua yaitu options, options ini berisi method, headers dan body. Tergantung keinginan kita.

cotoh penerapan nya :
```javascript
        let asyncApi = async() => {
        let api = ("url");
        let option = {
            method: "GET"
        }
        let response = await fetch(api, option)
        response = await response.json()
        console.log(response);
        }
        asyncApi();
```

### JS Intermediate Web Storage
Web Storage adalah menyimpan data pengguna seperti pencarian, artikel berita, dan lain-lain ke lokal (browser) menggunakan web storage seperti cookies, local storage, dan session storage. Data ini dimanfaatkan oleh situs web tersebut untuk merekam kebiasaan pengguna agar dapat memberikan rekomendasi sesuai preferensi si pengguna tersebut.

Cookies adalah data kecil yang dikirim dari situs web dan disimpan di komputer kita oleh web browser saat kita menjelajah.

Local storage memiliki karakteristik sebagai berikut: <br>
    * Menyimpan data tanpa tanggal kadaluarsa.
    * Data tidak akan dihapus ketika web browser ditutup dan akan tersedia seterusnya selama kita tidak menghapus data local storage pada web browser.
    * Dapat menyimpan data hingga 5MB.
    * Hanya dapat menyimpan data string.

Struktur dasar local storage 
```javascript
        if (localStorage.getItem("theme") === "dark") { 
    document.body.classList.add("dark");
    } else {
      document.body.classList.remove("dark");
    }

    document.getElementById("toggle").onclick = () => {
      if (localStorage.getItem("theme")) {
        localStorage.removeItem("theme");
        document.body.classList.remove("dark");
        } else {
        localStorage.setItem("theme", "dark");
        document.body.classList.add("dark");
        }
        };
```




