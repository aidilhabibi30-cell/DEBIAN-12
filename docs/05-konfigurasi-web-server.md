Konfigurasi Web Server Apache2 Debian 12

1. Pengertian

Web Server adalah layanan yang digunakan untuk menyimpan dan menampilkan halaman website kepada pengguna melalui jaringan internet atau jaringan lokal.

Apache2 merupakan salah satu aplikasi web server yang dapat dijalankan pada Debian 12.

2. Tujuan

* Memahami fungsi Web Server.
* Mempelajari instalasi Apache2.
* Menjalankan layanan website pada Debian 12.
* Melakukan pengujian akses website.

3. Instalasi Apache2

Perbarui daftar paket:

sudo apt update

Instal Apache2:

sudo apt install apache2

4. Menjalankan Apache2

sudo systemctl start apache2

Mengaktifkan layanan otomatis:

sudo systemctl enable apache2

5. Memeriksa Status Apache2

sudo systemctl status apache2

6. Pengujian Web Server

Periksa alamat IP Debian:

ip address

Buka browser dari perangkat yang dapat mengakses server, kemudian masukkan:

http://IP-ADDRESS-SERVER

Jika berhasil, halaman default Apache2 akan muncul.

7. Kesimpulan

Apache2 merupakan aplikasi Web Server yang dapat digunakan untuk menjalankan website pada sistem operasi Debian 12.