| Nama      | Nuryadi |
| ----------- | ----------- |
| NIM     | 312010621      |
| Kelas   | TI.20.A.1        |

## Langkah langkah praktikum 2
Membuka text editor, Saya menggunakan Sublime text
![img1!](assets/img/praktikum/start.png)
 
## 1. Membuat Dokumen HTML
![img1!](assets/img/1/1.png)

Buka pada browser untuk melihat hasilnya

![img1-1!](assets/img/1/1-1.png)

## 2. Mendeklarasikan CSS Internal
![img2!](assets/img/2/2.png)

simpan perubahan yang ada, dan lakukan refresh pada browser untuk melihat hasilnya

![img2-1!](assets/img/2/2-1.png)

## 3. Menambahkan Inline CSS
tambahkan deklarasi inline CSS pada tag `<p>` seperti berikut

![img3!](assets/img/3/3-2.png)

Refresh kembali browser untuk melihat perubahannya

![img3-1!](assets/img/3/3-1.png)

## 4. Membuat CSS Eksternal
Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut

![img4!](assets/img/4/4.png)

Kemudian tambahkan tag `<link>` untuk merujuk file css yang sudah dibuat pada bagian `<head>`

![img4-1!](assets/img/4/4-1.png)

Selanjutnya refresh kembali browser untuk melihat perubahannya.

![img4-1!](assets/img/4/4-2.png)

## 5. Menambahkan CSS Selektor
Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file style_eksternal.css, tambahkan kode berikut

![img5!](assets/img/5/5.png)

Kemudian simpan kembali dan refresh browser untuk melihat perubahannya

![img5-1!](assets/img/5/5-1.png)


## Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( `<p id="paragraf-1" class="text-paragraf">` )

## Jawab
1. Saya akan mengubah dan menambah properti dan nilai pada kode CSS, dimulai dari membuat kerangka html nya

	![img1!](assets/img/praktikum/1.png)

	Kemudian membuat CSS nya dengan menambah properti dan nilai pada kode

	Saya menambahkan 4 selektor ke dalam CSS, diantaranya body, h2, .avatar, .header-profile. Masing-masing memiliki fungsi untuk mengatur tampilan pada html

	pada selektor body saya menambahkan beberapa properti, yaitu margin, width, font-size, color, dst.

	selektor h2, properti font-weight, font-size

	selektor .avatar, properti width, border-radius

	selektor .header-profile, display, justify-content, align-items

	![img1-1!](assets/img/praktikum/1-1.png)

	Pada hasil tersebut dapat dilihat, pada mode mobile lebar body terlalu ke tengah, karena widht pada selektor body diatur dengan nilai 50% pada ukuran desktop, agar dapat terlihat proporsional pada ukuran mobile dapat ditambahkan selektor `@media only screen and (max-width: 760px)`, dan hasil nya bisa dilihat 

	![img1-2!](assets/img/praktikum/1-2.png)


2. `h1{}` Untuk memberikan style pada semua element h1

	`#intro h1{}` Awalan simbol hash (#) memungkinkan kita untuk memberi style pada id.
	selector id bersifat kaku dan tidak bisa digunakan kembali pada element yang lainnya. Menurut saya lebih baik gunakan selektor class untuk mendefinisikan element yang ingin diberi nilai.
![img2!](assets/img/praktikum/2.png)

3. Setelah dilakukan pengujian, deklarasi CSS Inline lebih dahulu tampil di browser, itu dikarenakan permintaan HTTP yang sangat kecil memungkinkan untuk ditampilkan dahulu

	Berikut merupakan hasil pengujian deklarasi CSS

	CSS Inline `blue`
	
	CSS Internal `red`
	
	CSS Eksternal `yellow`
	
	![img3!](assets/img/praktikum/3.png)

4. Deklarasi `id="paragraf-1"` akan ditampilkan pada browser, karena selektor id lebih spesifik dari class atau bahkan element P itu sendiri, kecuali jika kita menambahkan property pada inline element P maka selektor id tersebut akan tertimpa, karena inline lebih spesifik daripada id, class, dan element

	![img4!](assets/img/praktikum/4.png)