# Bind9
Berkeley Internet Name Domain versi 9 atau yang disingkat menjadi `bind9` adalah salah satu aplikasi linux yang dapat digunakan sebagai DNS server. Hingga artikel ini diterbitkan, Bind9 menjadi softaware yang paling banyak digunakan di Internet. Tidak hanya itu, Bind9 juga digunakan sebagai DNS server pada hampir semua distro linux.

Dengan `bind9`, kita dapat mempublikasikan informasi DNS di internet, serta memungkinkan DNS Server yang kita buat untuk meresponse permintaan DNS dari pengguna. Seperti yang kami sampaikan, `bind9` berfungsi sebagai DNS server.

## Konfigurasi pada server Debian
Berikut adalah cara install bind9 di Linux Debian.
1. Install paket `bind9` di server dengan command berikut :
```bash
apt-get install bind9 dnsutils
```
