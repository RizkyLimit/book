# Cara Install MariaDB di Debian 11+

## Pendahuluan
MariaDB adalah sistem manajemen basis data relasional sumber terbuka, biasanya digunakan sebagai alternatif MySQL sebagai bagian basis data dari tumpukan LAMP (Linux, Apache, MySQL, PHP/Python/Perl) yang populer. Ini dimaksudkan sebagai pengganti MySQL.

## Prasyarat
- Untuk mengikuti tutorial ini, Anda memerlukan server yang menjalankan Debian 11. Server ini harus memiliki pengguna administratif non-root dan firewall yang dikonfigurasi dengan UFW. Atur ini dengan mengikuti panduan pengaturan server awal kami untuk Debian 11.



# Tahap - Tahap Installasi
1. [Memperbarui Paket](#step1)
2. [Menginstall MariaDB](#step2)
### Langkah 1 - Memperbarui Paket<a name="step1"></a>
Pastikan memperbarui file indeks paket, dan memperbarui paket karena sangat penting untuk menjaga sistem Linux Anda tetap up-to-date dengan rilis paket terbaru.
```bash
apt-get update && apt-get upgrade
```
### Langkah 2 - Menginstall MariaDB<a name="step2"></a>
Install `MariaDB` dengan perintah berikut:
```bash
apt-get install mariadb-server
```

Setelah melakukan proses installasi, selanjutnya kita akan auto konfigurasi dengan `mysql_secure_installasion` agar `MariaDB` dapat digunakan  
