# Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server
Sebelumnya pastikan kalian sudah menginstall ubuntu server dan sudah melakukan instalasi pada virtual box. Untuk memulai, langsung saja klik ubuntu server pada box.

# Pembuatan Web Pada Ubuntu Server
## 1. Ketika kalian mengklik ubuntu server, itu akan meminta kalian untuk memasukkan username dan password.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/a4a60709-6fe2-4c98-912d-6419d3923e07)

Jika sudah memasukkan username dan password, akan tampil promp seperti ini, artinya kita siap untuk memasukkan command untuk melanjutkan instalasi.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/76557c9d-9bd5-4955-8a90-5b5a53444e4a)

## 2.	Gunakan perintah `sudo apt update`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/58c927d7-985f-486c-88a6-1864c1ee92f7)

Kita akan diminta memasukkan password pada tahap ini.  Perintah ini digunakan untuk melakukan pembaruan informasi paket dari repositori paket yang diinstal di sistem ubuntu server, jika berhasil akan tampil seperti dibawa ini:

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/d541f22a-56b3-46ae-90b8-84fdb3b9e409)

## 3. Masukkan perintah  `ping google.com`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/7000c264-b0c9-4f12-8e13-507c66bdd958)

Perintah ini digunakan untuk menguji koneksi jaringan antara server Anda dan situs web Google (google.com), jika berhasil akan tampil seperti dibawa ini:

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/211a1966-a059-46ce-94c0-18ec14daed3e)

## 4.	Gunakan perintah `sudo apt install apache2`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/af012bec-e928-4b48-828a-f5596490f344)

Perintah ini digunakan untuk menginstal server web Apache (Apache HTTP Server) di sistem ubuntu server.

## 5.	Perintah `sudo ufw app list`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/1f0e4a50-fa20-431a-8f95-8eff14b12e42)

Perintah digunakan untuk menampilkan daftar aplikasi atau layanan yang telah didefinisikan dalam konfigurasi Uncomplicated Firewall (UFW) di Ubuntu Server. Berikut tampilan dari perintah ini:

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/018cfafa-a195-444c-bb5f-0bc9caf8aaf8)

## 6.	Masukkan command `sudo systemctl status apache2`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/ce191ea9-1cbd-4b62-b657-a5b61b5252cf)

Perintah ini digunakan untuk memeriksa status layanan Apache HTTP Server (biasanya disebut sebagai Apache2) pada sistem Ubuntu. Ini memberikan informasi tentang apakah layanan Apache sedang berjalan, sedang dihentikan, atau mengalami masalah. Berikut adalah contoh apabila apache2 kalian sedang aktif dan berjalan.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/82b8b408-9651-4109-bff2-8a8f76809149)

## 7.	Gunakan perintah `ip addr` atau `hostname -I`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/bd3fadee-225c-4d6e-b20c-f9d22eca825e)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/34d18872-fc53-4b5a-b669-88edbbcbdbe5)

Perintah ip addr dan hostname -I adalah bahwa keduanya digunakan untuk menampilkan informasi jaringan di sistem Linux. Bedanya ip addr menampilkan informasi rinci tentang semua antarmuka jaringan pada sistem ubuntu server, sedangkan hostname -I  menampilkan alamat IP dari mesin yang terkait dengan nama host yang ada di sistem ubuntu server. 

## 8.	Open ip address di browser

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/b457f48b-3e24-4338-a77a-3eff451932fb)

Halaman "It works!" adalah halaman default yang akan muncul ketika mengakses alamat IP atau nama domain server melalui web browser. Ini merupakan cara cepat dan sederhana untuk memeriksa bahwa server web  berjalan dengan baik setelah menginstal Apache.

## 9.	Gunakan perintah `cd /var/www` untuk mengubah direktori kerja kita ke direktori `/var/www` untuk menyimpan file yang akan disajikan oleh server web seperti Apache. Lalu gunakan perintah `cd html`  untuk mengubah direktori kerja kita menjadi direktori dengan nama `"html"` di lokasi saat ini. Jika setelahnya kalian mengetik ls, makan akan telihat ada index,html didalamnya untuk website kita.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/98780ee8-31cf-4ea7-9ae8-29380ad6d23f)

## 10.	Lanjut dengan perintah `sudo mkdir *nama web*` untuk membuat direktori baru dengan nama `*nama web*` di sistem kita. Lalu perintah `ls` untuk melihat direktori yang baru saja kita buat.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/a2d4f04a-d2ee-4d23-bdb3-5483fad1cc9d)

## 11. Ketikkan perintah `sudo chmod 777 *namaweb*` untuk mengubah izin atau hak akses pada direktori. "777" memberikan izin penuh pada direktori atau berkas, yang berarti siapa pun dapat membaca, menulis, dan mengeksekusi berkas tersebut. Setelah itu kita ketikkan perintah `cd *nama web*` untuk beralih ke direktori web yang kita buat.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/f7c09b2c-681f-46f3-b8aa-1a9c7b16a856)

## 12.	Gunakan perintah nano index.html, dengan ini kita dapat mengedit kode HTML sesuai dengan kebutuhan. Jangan lupa simpan setiap perubahan yang kita buat akan menyimpan perubahan tersebut.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/742e4afa-2d04-453f-89c7-b686e75ca3bb)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/0639be5f-43b2-4d65-a6b0-912c71ecdf2d)

## 13.	Cek website menggunakan `ip adress/namaweb`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/12c73e75-8ec6-4c27-9dc7-c3197d4ffc36)

## 14.	Periksa website menggunakan PuTTY, CMD, dan Ubuntu Dekstop
> PuTTY

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/5dfb01f1-61d3-4219-a75a-fc6c4f18d065)

Untuk di PuTTY, kita hanya perlu memasukkan ip address, lalu klik ok, dan akan masuk ke terminal PuTTY, selanjutnya kita akan diminta untuk memasukkan username dan password, jika berhasil akan tampil seperti diatas.

> CMD

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/76b94b1d-a4b5-4cf6-a330-d845b61be6e4)

Untuk di CMD, kita hanya perlu untuk memasukkan `ssh namauser@ipadress`, lalu kita akan diminta memasukkan password, jika berhasil, akan tampil seperti diatas.

> Ubuntu Desktop

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/ed2a2686-f44b-4f89-9d6c-b22f2801625b)

Pada Ubuntu Dekstop, kita juga perlu memasukkan `ssh namauser@ipaddress`, lalu kita akan diminta memasukkan password, jika berhasil, akan tampil seperti diatas. Perlu dipastikan untuk step ini, kalian sedang membuka ip address di browser.

# Pembuatan Wordpress Pada Ubuntu Server
## Install WordPress on Ubuntu 18.04
Sebelum kita mulai, mari kita perbarui dan meningkatkan sistem. Masuk sebagai pengguna root ke sistem  dan perbarui sistem untuk memperbarui repositori.
`apt update && apt upgrade`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/960630a3-e426-47ce-834d-18e6d6206e02)

## Step 1: Install Apache
Kita telah mendownload apache2, jadi kita hanya perlu mengeceknya dengan perintah :
`systemctl status apache2`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/b424a69c-995e-484e-858f-b253d0748477)

> Untuk memverifikasi lebih lanjut, buka browser dan buka alamat IP server. 

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/d090acb8-94ce-418d-a57c-9e4b6ad0abb1)

## Step 2: Install MySQL
Selanjutnya, kita akan menginstal mesin basis data MariaDB untuk menyimpan file Wordpress kita. MariaDB adalah sebuah fork sumber terbuka dari MySQL dan sebagian besar perusahaan hosting menggunakannya sebagai pengganti MySQL.
`apt install mariadb-server mariadb-client

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/d2592b7e-5489-4db0-8f06-70237260cdbe)

> Mengamankan mesin basis data MariaDB
Sekarang mari kita amankan mesin basis data MariaDB kita dan melarang login root jarak jauh. Jawab pertanyaan yang muncul sesuai dengan preferensi masing masing.
`mysql_secure_installation`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/adaf4fc9-5a59-4ab3-bb23-def6ac342365)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/f1851443-7c60-418d-b663-477654400040)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/20eb65ea-0b72-4315-b4fd-ac0db7136a76)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/8d05ee5e-e29e-4092-b693-ec7c2128b8ec)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/85e9d855-59cc-4eed-a272-14e6b3abe0ac)

## Step 3: Install PHP
Terakhir, kita akan menginstal PHP sebagai komponen terakhir dari tumpukan LAMP.
`apt install php php-mysql`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/9db7600d-913e-45d9-ae76-1424b133d438)

Untuk mengonfirmasi bahwa PHP telah terinstal, buatlah file info.php pada /var/www/html/
`nano /var/www/html/info.php`
Tambahkan baris berikut ini:

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/824fb38b-c9b6-4a80-8186-b533e9a51948)

Simpan dan Keluar. Buka browser dan tambahkan /info.php ke URL server.
`https:??ip-adress/info.php`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/66ed3fe4-0f33-4a7c-b408-d8a3b882cd41)

## Step 4: Create WordPress Database
Sekarang saatnya untuk masuk ke database MariaDB kita sebagai root dan membuat database untuk menampung data WordPress.
`mysql -u root -p`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/b14ea21d-48e3-4e66-a3e6-90bbf392b215)

Buat database untuk instalasi WordPress kita.

`CREATE DATABASE wordpress_db;`

Selanjutnya, buatlah pengguna database untuk pengaturan WordPress kita.

`CREATE USER 'wp user'@'localhost' IDENTIFIED BY 'password';`

Selanjutnya, berikan hak istimewa kepada pengguna untuk mengakses database

`GRANT ALL ON wordpress_db.* TO 'wp_user'@'localhost' IDENTIFIED BY 'password'`

Setelah itu kalian bisa keluar dari database

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/1eca05c0-fb68-47f4-a7d6-7f54ca4da172)

Contoh :

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/962c52ad-5796-4d23-9b71-cd51dc837069)

## Step 5: Install WordPress CMS

- Buka direktori temporer dan unduh file WordPress terbaru.
`cd /tmp && wget https://wordpress.org/latest.tar.gz

- Selanjutnya, buka kompresi tarball yang akan menghasilkan folder bernama "wordpress".
`tar -xvf latest.tar.gz`

- Salin folder wordpress ke jalur /var/www/html/
`cp -R wordpress /var/www/html/`

- Jalankan perintah di bawah ini untuk mengubah kepemilikan direktori 'wordpress'.
`chown -R www-data:www-data /var/www/html/wordpress/`

- Jalankan perintah di bawah ini untuk mengubah kepemilikan direktori 'wordpress'.
`chmod -R 755 /var/www/html/wordpress`

- Buat direktori ‘uploads’.
`mkdir /var/www/html/wordpress/wp-content/uploads/`

- Terakhir, ubah izin direktori 'uploads'.
`chown -R www-data:www-data /var/www/html/wordpress/wp-content/uploads/`

- Buka URL server
`https://server-ip/wordpress`

Kita akan dihadapkan pada wizard WordPress dan daftar kredensial yang diperlukan untuk berhasil dalam pengaturannya. Isi formulir seperti yang ditunjukkan dengan kredensial yang ditentukan saat membuat basis data WordPress di basis data MariaDB. Abaikan host database dan awalan tabel dan tekan tombol 'Kirim'. Jika semua detail sudah benar, kita akan diberi lampu hijau untuk melanjutkan. Isi detail tambahan yang diperlukan seperti judul situs, nama pengguna, dan kata sandi dan simpan di tempat yang aman agar tidak lupa. Pastikan untuk menggunakan kata sandi yang kuat. Scroll ke bawah dan tekan 'Instal WordPress'. Jika semua berjalan lancar, maka kita akan mendapatkan notifikasi 'sukses' seperti yang ditunjukkan. Klik tombol 'Login' untuk mengakses halaman login dari instalasi WordPress yang baru. Masukkan informasi login dan tekan.


![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/fecabeed-a828-45c6-9302-791ca72d8489)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/4c9507b4-bc6d-41dc-ba90-d2b03400eb00)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/fa2c4a1f-c1c1-4603-8af8-95fa79301850)

Jika wordpress sudah berhasil dibuat, kita bisa mengedit wordpress tersebut sesuai keinginan kita, terdapat banyak fitur di wordpress yang bisa mengasah kreatifitas kita. Sebagai contoh saya menggunakan tema yang telah tersedia di wordpress. Lalu saya mencoba mengedit, dan memposting di wordpress saya.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/9f9212ce-f5f8-4659-8baf-abc1a1638591)

Disini terlihat saya sudah memposting 3 hal yaitu Hello, Movies Rating by Zara, dan Zara’s College Life. Kalian juga bisa mengedit sesuka kalian untuk wordpress ini. Berikut hasil akhir dari tampilan yang saya buat.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/105e9ddf-f8ea-4754-a159-65e0838efeb6)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/15c90c2d-b2f6-410e-91c5-30c8f9fcbce5)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/65ab6e5d-84b9-4510-9c52-755fb2c528d5)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/43ca26db-0be4-4288-a69f-4b0d7922a244)





