# Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server
Sebelumnya pastikan kalian sudah menginstall ubuntu server dan sudah melakukan instalasi pada virtual box. Untuk memulai, langsung saja klik ubuntu server pada box.

# 1. Ketika kalian mengklik ubuntu server, itu akan meminta kalian untuk memasukkan username dan password.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/a4a60709-6fe2-4c98-912d-6419d3923e07)

Jika sudah memasukkan username dan password, akan tampil promp seperti ini, artinya kita siap untuk memasukkan command untuk melanjutkan instalasi.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/76557c9d-9bd5-4955-8a90-5b5a53444e4a)

# 2.	Gunakan perintah `sudo apt update`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/58c927d7-985f-486c-88a6-1864c1ee92f7)

Kita akan diminta memasukkan password pada tahap ini.  Perintah ini digunakan untuk melakukan pembaruan informasi paket dari repositori paket yang diinstal di sistem ubuntu server, jika berhasil akan tampil seperti dibawa ini:

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/d541f22a-56b3-46ae-90b8-84fdb3b9e409)

# 3. Masukkan perintah  `ping google.com`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/7000c264-b0c9-4f12-8e13-507c66bdd958)

Perintah ini digunakan untuk menguji koneksi jaringan antara server Anda dan situs web Google (google.com), jika berhasil akan tampil seperti dibawa ini:

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/211a1966-a059-46ce-94c0-18ec14daed3e)

# 4.	Gunakan perintah `sudo apt install apache2`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/af012bec-e928-4b48-828a-f5596490f344)

Perintah ini digunakan untuk menginstal server web Apache (Apache HTTP Server) di sistem ubuntu server.

# 5.	Perintah `sudo ufw app list`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/1f0e4a50-fa20-431a-8f95-8eff14b12e42)

Perintah digunakan untuk menampilkan daftar aplikasi atau layanan yang telah didefinisikan dalam konfigurasi Uncomplicated Firewall (UFW) di Ubuntu Server. Berikut tampilan dari perintah ini:

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/018cfafa-a195-444c-bb5f-0bc9caf8aaf8)

# 6.	Masukkan command `sudo systemctl status apache2`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/ce191ea9-1cbd-4b62-b657-a5b61b5252cf)

Perintah ini digunakan untuk memeriksa status layanan Apache HTTP Server (biasanya disebut sebagai Apache2) pada sistem Ubuntu. Ini memberikan informasi tentang apakah layanan Apache sedang berjalan, sedang dihentikan, atau mengalami masalah. Berikut adalah contoh apabila apache2 kalian sedang aktif dan berjalan.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/82b8b408-9651-4109-bff2-8a8f76809149)

# 7.	Gunakan perintah `ip addr` atau `hostname -I`

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/bd3fadee-225c-4d6e-b20c-f9d22eca825e)

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/34d18872-fc53-4b5a-b669-88edbbcbdbe5)

Perintah ip addr dan hostname -I adalah bahwa keduanya digunakan untuk menampilkan informasi jaringan di sistem Linux. Bedanya ip addr menampilkan informasi rinci tentang semua antarmuka jaringan pada sistem ubuntu server, sedangkan hostname -I  menampilkan alamat IP dari mesin yang terkait dengan nama host yang ada di sistem ubuntu server. 

# 8.	Open ip address di browser

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/b457f48b-3e24-4338-a77a-3eff451932fb)

Halaman "It works!" adalah halaman default yang akan muncul ketika mengakses alamat IP atau nama domain server melalui web browser. Ini merupakan cara cepat dan sederhana untuk memeriksa bahwa server web  berjalan dengan baik setelah menginstal Apache.

# 9.	Gunakan perintah `cd /var/www` untuk mengubah direktori kerja kita ke direktori `/var/www` untuk menyimpan file yang akan disajikan oleh server web seperti Apache. Lalu gunakan perintah `cd html`  untuk mengubah direktori kerja kita menjadi direktori dengan nama `"html"` di lokasi saat ini. Jika setelahnya kalian mengetik ls, makan akan telihat ada index,html didalamnya untuk website kita.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/98780ee8-31cf-4ea7-9ae8-29380ad6d23f)

# 10.	Lanjut dengan perintah `sudo mkdir *nama web*` untuk membuat direktori baru dengan nama `*nama web*` di sistem kita. Lalu perintah ls untuk melihat direktori yang baru saja kita buat.

![image](https://github.com/ZahraMaharaniP/Step-by-Step-Membuat-Wordpress-Melalui-Ubuntu-Server/assets/149281915/a2d4f04a-d2ee-4d23-bdb3-5483fad1cc9d)

# 11. Ketikkan perintah sudo chmod 777 *namaweb* untuk mengubah izin atau hak akses pada direktori. "777" memberikan izin penuh pada direktori atau berkas, yang berarti siapa pun dapat membaca, menulis, dan mengeksekusi berkas tersebut. Setelah itu kita ketikkan perintah cd *nama web* untuk beralih ke direktori web yang kita buat.






