##Tutorial Membuat Repository VCS Baru

<p>Dalam petunjuk ini, saya akan membahas bagaimana cara membuat repository baru.</p>
Dimulai dari Instalasi perangkat lunak Git sampai repository baru dibuat. 
Di sini saya akan menggunakan Github.com sebagai VCS yang akan kita pakai dalam petunjuk ini, dan dengan menggunakan sistem operasi Windows. Mungkin cara yang akan 

saya gunakan disini akan sedikit berbeda dengan cara yang digunakan pada sistem operasi Linux dan Mac OS X.



## 1. Permulaan
Pertama-tama kita akan menginstall perangkat lunak yang bernama "Git", silahkan anda download dari halaman "http://git-scm.com/download" tanpa tanda petik.

![gambar web git-scm](https://github.com/muhsuprayogi/gambar-1/blob/master/Img_1.png)

### Instalasi

<p>Silahkan anda buka file instalasi git yang sudah anda download tadi.
Setelah anda membuka file tersebut, maka akan muncul tampilan seperti dibawah ini :</p>

![gambar instalasi git](https://github.com/muhsuprayogi/gambar-2/blob/master/Img_2.png)

Saya rekomendasikan anda untuk menggunakan pengaturan default. Silahkan klik **"Next"** sampai instalasi selesai.

## 2. Membuat akun Github

<p>Selanjutnya anda harus mempunyai akun github terlebih dahulu, jika anda belum pernah mendaftar, silahkan ikuti langkah-langkah berikut. Silahkan anda kunjungi 

website github.com maka akan terlihat tampilan seperti dibawah ini :</p>

![gambar halaman github](https://github.com/muhsuprayogi/gambar-3/blob/master/Img_3.png)

Klik **Sign Up** pada sudut kanan atas halaman. 
Berikut tampilan pendaftaran github :


![gambar daftar github](https://github.com/muhsuprayogi/gambar-4/blob/master/Img_4.png)


Anda akan masuk pada halaman pendaftaran **Step 1**.
Silahkan isi **Username**, **Email address** dan **Password** anda.
Silahkan lakukan **Verify account** dengan benar.
Klik **"Create an account"** di akhir halaman **Step 1**


**Catatan :**


* Pastikan pengisian Username tidak menggunakan **spasi**.
* Isi Email address dengan alamat email yang anda gunakan dan bisa anda akses saat ini.
* Pastikan pengisian data sudah berubah menjadi tanda centang "**✓**" berwarna hijau, yang menandakan **Username** atau **Email address** yang anda masukan bisa 

digunakan oleh anda.
* Usahakan untuk meminimalisir kesalahan saat melakukan **"Verify account"** pada **Step 1**.
Jika data sudah berhasil anda isi, maka anda bisa melanjutkan ke **Step 2** dan **Step 3**.
Pada **Step 3**, Verifikasi akan dikirimkan oleh Github dalam bentuk email ke alamat email yang telah anda masukan pada **tahap pengisian data** atau **Step 1**.


### Selanjutnya adalah langkah membuat repository baru dalam github.


Silahkan anda klik ikon "**+"** pada sudut kanan atas halaman lalu pilih "**New repository**" seperti gambar di bawah ini :



![Img membuat repo](https://github.com/muhsuprayogi/gambar-5/blob/master/Img_5.png)


Maka akan muncul tampilan seperti di bawah ini :


![Img tampilan membuat repository](https://github.com/muhsuprayogi/gambar-6/blob/master/Untitled.png)

Isi **"Repository name"** dengan nama yang anda inginkan. Mari kita gunakan nama **"Latihan1"** sebagai permulaan, agar bisa lebih mudah mengikuti petunjuk ini 

selanjutnya.


## 3. Menggunakan Git

Jika anda sudah menyelesaikan petunjuk nomor 1 **(1. Permulaan)**, anda bisa mengikuti petunjuk bagaimana menggunakan git. Silahkan anda buka aplikasi yang sudah anda 

install pada petunjuk nomor 1 yaitu **"Git Bash"**. Anda juga bisa menggunakan Command Prompt (CMD), namun karena menggunakan git bash lebih mudah saat ini, jadi mari 

ikuti langkah ini.  
Biasanya Git Bash ini bisa dibuka langsung dengan cara "klik kanan" di desktop maupun windows explorer. Namun sebagai permulaan, saya akan membuka aplikasi dari 

**Start Menu > All programs > Git > Git Bash** atau dengan mengetikan langsung "Git Bash" pada **Start Menu** di sistem operasi Windows.  


Silahkan ketikan kode berikut untuk memperkenalkan diri anda agar tidak terjadi kesalahan pada proses selanjutnya :
```
$ git config --global user.name "namasaya"
$ git config --global user.email emailsaya
```
**Contoh :**
```
$ git config --global user.name "namasaya"  
$ git config --global user.email emailsaya@mail.com  
```
Selanjutnya kita akan cek lokasi direktori kita saat ini :
```
$ pwd
```
Disini saya akan membuat folder lokal di **disk "D:"** dengan nama folder **"Latihan1"** :
```
$ cd d:
$ mkdir Latihan1
``` 
![img git bash](https://github.com/muhsuprayogi/gampar-7/blob/master/Img_7.png)
Lalu masukan perintah berikut untuk membuat file "README.md"  
```
$ echo "# Latihan1" >> README.md
$ git init 
$ git add README.md
$ git commit -m "File pertama saya"
$ git remote add origin [Url_Repository_anda]
$ git push -u origin master
```
Untuk mendapatkan **"Url_Repository_anda"**, silahkan buka repository **"Latihan1"** yang sudah anda buat di akun github anda.  
Lalu pilih "Clone or download" dan salin url yang tertera.


![img link repo](https://github.com/muhsuprayogi/gambar-8/blob/master/Untitled2.png)

Contoh kode perintah yang akan anda masukan :
```
$ git remote add origin https://github.com/antonmartinus72/latihan1.git
```
Setelah anda memasukan semua kode perintah, anda akan diminta memasukan **Username** dan **Password** github anda.
# Selamat~~
Anda sudah berhasil membuat file repository bernama **"Latihan1"** yang di isi dengan file **"README.md"** dan anda akan melihat teks **"Latihan1"** dengan cetak tebal 

pada repository github anda.

Silahkan refresh browser anda untuk melihat hasil yang sudah anda kerjakan tadi.
![img link repo](https://github.com/muhsuprayogi/gambar-akhir/blob/master/Untitled4.png)

Sekian dari saya, dan semoga bermanfaat~.






