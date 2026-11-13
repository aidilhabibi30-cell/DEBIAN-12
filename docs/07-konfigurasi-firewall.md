Konfigurasi Firewall Debian 12 Menggunakan UFW

1. Pengertian

Firewall adalah sistem keamanan jaringan yang digunakan untuk mengatur lalu lintas data yang masuk dan keluar dari perangkat.

UFW (Uncomplicated Firewall) merupakan aplikasi untuk mengelola firewall pada Linux.

2. Tujuan

* Memahami fungsi firewall.
* Mempelajari pengaturan keamanan server.
* Mengatur akses layanan jaringan.

3. Instalasi UFW

sudo apt update
sudo apt install ufw

4. Mengizinkan SSH

Sebelum mengaktifkan firewall, izinkan SSH terlebih dahulu agar akses administrasi tidak terputus.

sudo ufw allow OpenSSH

5. Mengizinkan HTTP

sudo ufw allow 80/tcp

6. Mengaktifkan Firewall

sudo ufw enable

7. Memeriksa Status Firewall

sudo ufw status verbose

8. Kesimpulan

UFW membantu administrator mengelola aturan firewall sehingga akses jaringan pada server dapat dikontrol dengan lebih mudah.