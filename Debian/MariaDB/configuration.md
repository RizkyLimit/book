# Cara Install MariaDB di Debian 11

## Pendahuluan
MariaDB adalah sistem manajemen basis data relasional sumber terbuka, biasanya digunakan sebagai alternatif MySQL sebagai bagian basis data dari tumpukan LAMP (Linux, Apache, MySQL, PHP/Python/Perl) yang populer. Ini dimaksudkan sebagai pengganti MySQL.

## Prasyarat
- Untuk mengikuti tutorial ini, Anda memerlukan server yang menjalankan Debian 11. Server ini harus memiliki pengguna administratif non-root dan firewall yang dikonfigurasi dengan UFW. Peraturan ini mengikuti panduan pengaturan server awal kami untuk Debian 11.

# Tahap - Tahap Installasi
1. [Memperbarui Paket](#step1)
2. [Menginstall MariaDB](#step2)

### Langkah 1 — Memperbarui Paket<a name="step1"></a>
Pastikan memperbarui file indeks paket, dan memperbarui paket karena sangat penting untuk menjaga sistem Linux Anda tetap up-to-date dengan rilis paket terbaru.
```bash
apt-get update && apt-get upgrade
```

### Langkah 2 — Menginstall MariaDB<a name="step2"></a>
Saat tulisan ini dibuat, repositori _software_ bawaan Debian 11 menyertakan `MariaDB versi 10.5.15`. Ini ditandai sebagai varian MySQL default oleh tim pengemasan Debian MySQL/MariaDB.

Install MariaDB dengan perintah berikut:
```bash
apt-get install mariadb-server
```
Perintah ini akan menginstal MariaDB, tetapi tidak akan meminta Anda menyetel kata sandi atau membuat perubahan konfigurasi lainnya. Karena konfigurasi default membuat instalasi MariaDB Anda tidak aman, Anda akan menggunakan skrip yang disediakan paket `mariadb-server` untuk membatasi akses ke server dan menghapus akun yang tidak digunakan.

### Langkah 2 — Konfigurasi MariaDB<a name="step3"></a>
Untuk instalasi MariaDB baru, langkah berikutnya adalah menjalankan skrip keamanan yang disertakan. Skrip ini mengubah beberapa opsi default yang kurang aman untuk hal-hal seperti login root jarak jauh dan pengguna sampel.

Jalankan skrip keamanan:
```bash
mysql_secure_installation
```
