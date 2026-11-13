Konfigurasi SSH Server Debian 12

1. Pengertian

SSH (Secure Shell) adalah protokol jaringan yang digunakan untuk mengakses dan mengelola komputer atau server dari jarak jauh secara aman.

2. Tujuan

* Memahami fungsi SSH Server.
* Mempelajari administrasi server jarak jauh.
* Mengakses server melalui jaringan lokal.

3. Instalasi SSH Server

Jalankan perintah berikut pada terminal Debian 12:

sudo apt update
sudo apt install openssh-server

4. Memeriksa Status SSH

sudo systemctl status ssh

Perintah ini digunakan untuk melihat status layanan SSH.

5. Menjalankan SSH Server

sudo systemctl start ssh

Mengaktifkan SSH agar berjalan otomatis saat sistem dinyalakan:

sudo systemctl enable ssh

6. Pengujian

Lakukan pengujian koneksi SSH menggunakan perangkat lain dalam jaringan lokal.

7. Hasil

Tambahkan screenshot instalasi dan status SSH Server.

8. Kesimpulan

SSH Server membantu administrator mengelola server Debian 12 dari jarak jauh melalui koneksi jaringan yang aman.