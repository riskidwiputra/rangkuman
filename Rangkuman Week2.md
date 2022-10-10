# **Rangkuman Week2**

## **JavaScript Dasar Scope and Function**

## Scope
Scope adalah konsep dalam flow data variabel, yang menentukan suatu variabel bisa diakses pada scope tertentu atau tidak, dan digunakan untuk membatasi pengaksesan suatu variabel. Scope pada javascript memiliki 2 jenis yaitu local scope dan global scope
- Global scope merupakan sebuah jenis scope yang dimana variabel diletakan diluar sebuah function
- Local scope merupakan sebuah jenis scope yang dimana variabel diletakan didalam sebuah function

![git-clone](<https://i.imgur.com/iZ9I8lV.png>)

## Function
Function merupakan sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur. Saat kita membutuhkan fitur tersebut nantinya, kita bisa kembali menggunakannya.  function ini di sebut juga sebagai fungsi. 
Ada beberapa penulisan function :
- function classic
```
	function myFuction (parameter) {
		//Perintah yang dijalankan
	} 
```

- Arrow function
```
	let myFunction = () => {
		//kode yang dijalankan
	}
```

- function variable
```
	let myFuction = function (){
		//kode yang akan dijalankan
	}
```
  &nbsp;
### **Data Type Built in Prototype & Method**

  Data type merupakan sebuah hal yang krusial pada sebuah bahasa pemograman karena berfungsi untuk mengoperasikan sebuah variabel.
  Data type terbagi menjadi dua yaitu : 
- **Primitive**
    Tipe data primitif hanya dapat menyimpan satu nilai pada satu waktu dan tidak dapat diubah menggunakan cara yang sama seperti tipe data non-primitif. Tipe data Primitif akan dianggap sama jika nilainya sama.
    Ada tujuh tipe data primitif yang bisa kita gunakan Antara Lain:
    - String,
    - Number,
    - BigInt,
    - Boolean,
    - undefined,
    - null,
    - dan Symbol.
-  **Non-Primitive**
    Tipe data non-primitif dapat menyimpan lebih dari satu nilai pada satu waktu dan dapat diubah. Tipe data non-primitif akan dianggap berbeda meskipun nilainya sama dan dalam urutan yang sama.
    Ada banyak tipe data non-primitif di JavaScript Antara Lain
    - Array,
    - Object, 
    - Map, 
    - Set, 
    - WeakMap,
    - WeakSet,
    - Date
    - dan sebagainya, semuanya adalah Object.

&nbsp;

### **DOM**
DOM merupakan sebuah interface yang digunakan untuk memanipulasi keseluruhan dokumen HTML yang dimana memiliki properties dan methods untuk memanipulasi HTML tersebut. Terdapat cara untuk mengakses dokumen HTML pada javascript yaitu :
- document.getElementById ()
 -  document.GetElementsByClassName ()
 - document.GetElementsByName ()
 -  document.GetElementsByTagName ()
 
 Menambah (Adding) 

 - document.createElement(element)  
 - document.appendChild(element)

 menghapus (removing) 

 - document.removeChild(element)

Kemudian tedapat beberapa properties yang digunakan yaitu :

 - innerHTML
 - innerText

