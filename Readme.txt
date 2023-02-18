username admin : admin@gmail.com
password admin : 1234567890

username user yang menyetujui : approval@gmail.com
password user yang menyetujui : 1234567890

username user yang menyetujui : approval2@gmail.com
password user yang menyetujui : 1234567890

Web server
Apache/2.4.51 (Win64) OpenSSL/1.1.1l PHP/8.0.12
Database client version: libmysql - mysqlnd 8.0.12
PHP extension: mysqli Documentation curl Documentation mbstring Documentation
php version : PHP 8.0.12 (cli) (built: Oct 19 2021 11:21:05) ( ZTS Visual C++ 2019 x64 )
framework : Laravel Framework 9.52.0

phpMyAdmin
Version information: 5.1.1, latest stable version: 5.2.1

Database server
Server: 127.0.0.1 via TCP/IP
Server type: MariaDB
Server connection: SSL is not being used Documentation
Server version: 10.4.21-MariaDB - mariadb.org binary distribution
Protocol version: 10
User: root@localhost
Server charset: UTF-8 Unicode (utf8mb4)

Panduan konfigurasi aplikasi 
1. Clone project dari repository github ( https://github.com/Raldienpr325/SekawanMedia ) 
2. buat database yang nantinya akan dikonfigurasi dengan project laravel 
3. npm install , composer install
4. cp .env.example .env lalu Edit bagian database di file .env
5. php artisan key:generate , lalu php artisan serve


Panduan penggunaan aplikasi
1. Masuk ke localhost setelah artisan serve
2. Login menggunakan akun yang ada, jika ingin melakukan CRUD pemesanan bisa menggunakan admin, jika ingin melakukan approval pemesanan menggunakan akun approval.
3. Jika melakukan register, otomatis user akan menjadi role "ADMIN"
4. Setelah masuk langsung ke tampilan dashboard yang menjelaskan Jumlah Permintaan Kendaraan dan Status laporan permintaan kendaraan
5. Admin dapat melakukan CRUD pemesanan dan pemilihan driver serta ditujukan kepada siapa
6. terdapat log history approval , log history akan bertambah ketika ada perubahan status laporan
7. terdapat log aktivitas dimana ini mencakup aktivitas user login dan menambahkan kendaraan
8. Ada fitur export laporan periodik yang menampilkan jumlah aktivitas perhari ( Aktivitas akan berkurang ketika user melakukan delete kedalam log history ) 

!PENTING jika admin memilih approval2 sebagai atasan maka hanya approval2 yang dapat approve atau menolak laporan




