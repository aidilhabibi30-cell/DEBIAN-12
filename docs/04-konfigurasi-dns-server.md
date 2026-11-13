Konfigurasi DNS Server Debian 12

1. Pengertian

DNS (Domain Name System) adalah sistem yang menerjemahkan nama domain menjadi alamat IP sehingga perangkat dapat menemukan server tujuan.

2. Tujuan

* Memahami fungsi DNS Server.
* Mempelajari layanan DNS pada Linux.
* Mengetahui cara kerja penerjemahan nama domain menjadi IP Address.

3. Instalasi DNS Server

Pada Debian 12, DNS Server dapat menggunakan aplikasi BIND9.

Perbarui paket:

sudo apt update

Instal BIND9:

sudo apt install bind9 bind9-utils dnsutils

4. Memeriksa Status BIND9

sudo systemctl status named

5. Memeriksa Konfigurasi DNS

sudo named-checkconf

Perintah tersebut digunakan untuk memeriksa kesalahan konfigurasi BIND9.

6. Pengujian DNS

Gunakan perintah:

dig example.com

atau:

nslookup example.com

7. Hasil

Tambahkan screenshot instalasi BIND9, status layanan, dan hasil pengujian DNS.

8. Kesimpulan

DNS Server membantu menerjemahkan nama domain menjadi alamat IP sehingga komunikasi jaringan menjadi lebih mudah.