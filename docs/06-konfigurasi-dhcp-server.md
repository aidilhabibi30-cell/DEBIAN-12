Konfigurasi DHCP Server Debian 12

1. Pengertian

DHCP (Dynamic Host Configuration Protocol) adalah protokol jaringan yang memberikan konfigurasi IP Address secara otomatis kepada perangkat client.

2. Tujuan

* Memahami fungsi DHCP Server.
* Mempelajari pembagian IP Address otomatis.
* Mengelola konfigurasi jaringan client dan server.

3. Instalasi DHCP Server

Perbarui daftar paket:

sudo apt update

Instal aplikasi DHCP Server:

sudo apt install isc-dhcp-server

4. Konfigurasi DHCP Server

File konfigurasi utama:

sudo nano /etc/dhcp/dhcpd.conf

Contoh konfigurasi jaringan laboratorium:

subnet 192.168.10.0 netmask 255.255.255.0 {
    range 192.168.10.100 192.168.10.200;
    option routers 192.168.10.1;
    option subnet-mask 255.255.255.0;
    option domain-name-servers 8.8.8.8;
}

Konfigurasi tersebut merupakan contoh untuk jaringan dengan alamat IP 192.168.10.0/24.

5. Memeriksa Konfigurasi

sudo dhcpd -t

6. Menjalankan DHCP Server

sudo systemctl restart isc-dhcp-server

Memeriksa status layanan:

sudo systemctl status isc-dhcp-server

7. Pengujian

Hubungkan perangkat client ke jaringan laboratorium dan periksa apakah perangkat mendapatkan IP Address secara otomatis.

8. Kesimpulan

DHCP Server mempermudah administrator jaringan dalam membagikan IP Address secara otomatis kepada perangkat client.