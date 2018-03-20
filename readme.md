
<div align="center"><img src="https://www.opensourcecms.com/wp-content/uploads/dotclear-logo.png" width="290" height="110"></div>

<br/>
<p align="center" style="font-size:200px"><b>Dotclear</b></p>
<br/>

[Sekilas Tentang](#sekilas-tentang) | [Instalasi](#instalasi) | [Konfigurasi](#konfigurasi) | [Maintenance](#maintenance) | [Cara Pemakaian](#cara-pemakaian) | [Pembahasan](#pembahasan) | [Referensi](#referensi)
:---:|:---:|:---:|:---:|:---:|:---:|:--:

# Sekilas Tentang
[`^ kembali ke atas ^`](#)

***Dotclear*** merupakan blogging system yang dibuat pada tahun 2002, tujuan dari web ini adalah untuk memberikan aplikasi yang nyaman bagi pengguna dalam berbagi di web. Salah satu yang menjadi kelebihan dari dotclear adalah instalasi file yang tidak banyak menggunakan space hosting karena ukurannya hanya 4,48mb, jadi saat dibuka lebih terasa ringan dibandingkan dengan blogging system lainnya.


# Instalasi
[`^ kembali ke atas ^`](#)

**Kebutuhan Sistem :**
- `PHP 5.3 or above`
- `Database (MySQL, Postgre)`


**Proses Instalasi :**
- *Update* sistem dengan versi yang terbaru
`$ sudo apt-get update -y`

- *Install* ssh
`$ sudo apt update`
`$ sudo apt install ssh`

- *Install* apache, MySQL, dan PHP
`$ sudo apt install apache2`
`$ sudo apt install mysql-server`
`$ sudo apt install php`
`$ sudo apt install libapache2-mod-php`
`$ sudo apt install php-mysql`
`$ sudo apt install php-gd php-mcrypt php-mbstring php-xml php-ssh2`
`$ sudo service apache2 restart`

- Buat database untuk Dotclear
`$ mysql -u root -p`
`CREATE DATABASE dotclear;`
`CREATE USER dotclear IDENTIFIED BY 'dotclear';`
 `GRANT ALL PRIVILEGES ON dotclear.* TO dotclear;"`

- Pindah ke direktori web di lokalhost
`$ cd /var/www/html/`

- Mendownload packages terakhir dari situs dotclear.org
`$ wget http://download.dotclear.org/latest.tar.gz`

- Mengekstrak packages yang telah didownload
`$ tar -xvzf latest.tar.gz`

-  Mengatur hak akses
`$ sudo chmod a+w cache/`
`$ sudo chmod a+w inc/`
`$ sudo chmod a+w public/`

- Mengakses web `localhost:8888/dotclear/`
# Konfigurasi
[`^ kembali ke atas ^`](#)
Untuk mengakses konfigurasi, maka memilih menu System settings lalu memilih sub menu about:config.

- ***antispam*** : mencegah agar pengguna tidak melakukan spamming dalam pembuatan akun, tipe datanya adalah integer
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/1.JPG?raw=true"></img>
- ***breadcrumb*** :
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/2.JPG?raw=true"></img>
- ***dcckeditor*** :
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/3.JPG?raw=true"></img>
- ***dclegacyeditor*** :
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/4.JPG?raw=true"></img>
- ***pings*** :
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/5.JPG?raw=true"></img>
- ***system*** :
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/6.JPG?raw=true"></img>
- ***themes*** :
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/7.JPG?raw=true"></img>


# Maintenance
[`^ kembali ke atas ^`](#)

Untuk mengakses maintenance, maka memilih menu plugins lalu memilih sub menu maintenance.

- ***servicing*** :
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/1.JPG?raw=true"></img>
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/2.JPG?raw=true"></img>
- ***backup*** :
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/3.JPG?raw=true"></img>
- ***alert settings*** :
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/4.JPG?raw=true"></img>
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/5.JPG?raw=true"></img>

# Cara Pemakaian
[`^ kembali ke atas ^`](#)
1. Akses Bludit melalui localhost anda dengan masuk ke 127.0.0.1

2. Buat akun Bludit anda.
<img src="https://raw.githubusercontent.com/pramesywaraj/bludit-asik/master/Screenshots/Screenshot%20(2).png"></img>

3. Login dengan akun anda.
<img src="https://raw.githubusercontent.com/pramesywaraj/bludit-asik/master/Screenshots/Screenshot%20(3).png"></img>

4. Untuk membuat konten baru, masuk ke halaman dashboard dengan cara klik `admin panel` dibagian `Set up your new site`
<img src="https://raw.githubusercontent.com/pramesywaraj/bludit-asik/master/Screenshots/screenshot-localhost-2018.03.19-16-27-31.png"></img>

5. Tampilan Dashboard admin
<img src="https://raw.githubusercontent.com/pramesywaraj/bludit-asik/master/Screenshots/Screenshot%20(4).png"></img>

6. Untuk membuat post baru pilih menu `New content` pada bagian `PUBLISH`
<img src="https://raw.githubusercontent.com/pramesywaraj/bludit-asik/master/Screenshots/Screenshot%20(6).png"></img>

7. PIlih `Save` dan konten telah ter-publish
<img src="https://raw.githubusercontent.com/pramesywaraj/bludit-asik/master/Screenshots/Screenshot%20(7).png"></img>

# Pembahasan
[`^ kembali ke atas ^`](#)

# Referensi
https://www.linuxhelp.com/how-to-install-dotclear-in-ubuntu/

https://dotclear.org
