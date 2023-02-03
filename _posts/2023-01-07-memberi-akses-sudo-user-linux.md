---
title:  "Memberikan Akses Sudo untuk User pada Linux"
author: angga
categories: [Konfigurasi]
tags: [linux, server, debian, rocky]
---

## Pendahuluan

Halo teman-teman semua,

Kali ini saya akan berbagi informasi tentang langkah untuk memberikan hak akses sudo user, pada sistem operasi linux terutama server menggunakan perintah terminal.

## Akses Sudo pada User

Akses sudo pada user di sistem operasi Linux adalah hak untuk mengeksekusi perintah sebagai superuser atau administrator sistem. 

Superuser memiliki hak akses yang lebih luas dan dapat melakukan perubahan yang signifikan pada sistem, seperti menginstall software, mengubah konfigurasi sistem, atau menghapus file yang penting.

User yang memiliki akses sudo dapat mengeksekusi perintah dengan menambahkan perintah `sudo` di depan perintah yang ingin dijalankan. Contohnya, pada Debian atau Ubuntu jika ingin mengeksekusi perintah `apt update`, anda harus mengetik `sudo apt update` atau pada CentOS/Rocky Linux/Fedora jika butuh mengeksekusi perintah `yum update`, anda harus mengetik `sudo yum update`. Setelah itu, terminal akan akan meminta password superuser, setelah itu update sistem akan dijalankan dengan hak akses superuser.

Akses sudo dapat diberikan kepada user dengan menambahkan user ke grup `sudo` atau `wheel` (tergantung dari distribusi Linux yang digunakan).

Akses sudo sangat penting untuk manajemen sistem yang efektif, namun juga harus digunakan dengan hati-hati karena perintah yang dijalankan sebagai superuser dapat memiliki dampak yang signifikan pada kinerja sistem dan keamanan.

## Langkah dan Perintah Terminal untuk Memberikan Akses Sudo pada Debian 11

Untuk pemberian hak akses sudo terhadap user di sini, masih menggunakan 2 skenario yang sama seperti [artikel sebelumnya](/posts/membuat-user-linux){:target="_blank"} ketika pembuatan atau penambahan user baru pada Debian 11

1. untuk user `debian` ditambahkan menggunakan akun `root`, sedangkan 
2. untuk user `debian11` ditambahkan menggunakan akun `osboxes` (akun lain dengan akses sudo)

### Dari akun root

1. Login sistem sebagai `root`

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/d01.png)

1. Menambahkan user `debian` ke group `sudo` untuk akses sudo dengan ketik perintah berikut
   
   ```
   # usermod -aG sudo debian
   ```

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/d02.png)

1. Uji akses sudo dengan login ke user `debian`

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/d03.png)

1. Lakukan perintah update sistem, ketik perintah berikut

   ```
   $ sudo apt update
   ```

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/d04.png)

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/d05.png)

   Jika perintah dieksekusi, maka penambahkan akses sudo berhasil

### Dari akun lain dengan akses sudo

1. Login sistem sebagai `osboxes`

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/d06.png)

1. Menambahkan user `debian11` ke group `sudo` untuk akses sudo dengan ketik perintah berikut
   
   ```
   $ sudo usermod -aG sudo debian11
   ```

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/d07.png)

1. Uji akses sudo dengan login ke user `debian11`

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/d08.png)

1. Akses mode sudo, ketik perintah berikut

   ```
   $ sudo whoami
   ```

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/d09.png)

   Jika muncul informasi `root`, maka penambahkan akses sudo berhasil

## Langkah dan Perintah Terminal untuk Memberikan Akses Sudo pada Rocky Linux 8

Untuk pemberian hak akses sudo terhadap user di sini, masih menggunakan 2 skenario yang sama seperti [artikel sebelumnya](/posts/membuat-user-linux){:target="_blank"} ketika pembuatan atau penambahan user baru pada Rocky Linux 8

1. untuk user `rocky` ditambahkan menggunakan akun `root`, sedangkan
2. untuk user `rocky8` ditambahkan menggunakan akun `rockylinux` (akun lain dengan akses sudo)

### Dari akun root

1. Login sistem sebagai `root`

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/r01.png)

1. Menambahkan user `rocky` ke group `wheel` untuk akses sudo dengan ketik perintah berikut
   
   ```
   # usermod -aG wheel rocky
   ```

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/r02.png)

1. Uji akses sudo dengan login ke user `rocky`

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/r03.png)

1. Lakukan perintah update sistem, ketik perintah berikut

   ```
   $ sudo yum update
   ```

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/r04.png)

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/r05.png)

   Jika perintah dieksekusi, maka penambahkan akses sudo berhasil

### Dari akun lain dengan akses sudo

1. Login sistem sebagai `rockylinux`

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/r06.png)

1. Menambahkan user `rocky8` ke group `wheel` untuk akses sudo dengan ketik perintah berikut
   
   ```
   $ sudo usermod -aG wheel rocky
   ```

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/r07.png)

1. Uji akses sudo dengan login ke user `rocky8`

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/r08.png)

1. Akses mode sudo, ketik perintah berikut

   ```
   $ sudo whoami
   ```

   ![](/assets/img/2023-01-07-memberi-akses-sudo-user-linux/r09.png)

   Jika muncul informasi `root`, maka penambahkan akses sudo berhasil

## Penutup

Saya merasa sangat terhormat dan mengucapkan terima kasih sudah berkunjung ke blog NGLINUX ini. Saya berharap anda akan menemukan sesuatu yang bermanfaat di sini.

Salam, Angga.