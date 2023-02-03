---
title:  "Membuat User Baru pada Linux"
author: angga
categories: [Konfigurasi]
tags: [linux, server, debian, rocky]
---

## Pendahuluan

Halo teman-teman semua,

Kali ini saya akan berbagi informasi tentang langkah untuk membuat user baru, pada sistem operasi linux terutama server menggunakan perintah terminal.

Pada tulisan kali ini, saya menggunakan 2 distro yaitu Debian 11 dan Rocky Linux 8.

## Kebutuhan Menambah User

Beberapa alasan mengapa Anda mungkin ingin menambah user baru pada sistem operasi Linux, antara lain:

1. Keamanan
   
   Menambah user baru memungkinkan Anda untuk memberikan hak akses yang sesuai kepada setiap individu atau grup, sehingga Anda dapat mengontrol aktivitas yang diizinkan pada sistem. Ini akan meningkatkan keamanan sistem dari akses yang tidak diizinkan.

1. Pembagian tugas
   
   Menambah user baru memungkinkan Anda untuk membagikan tugas yang berbeda kepada setiap user, sehingga Anda dapat mengoptimalkan produktivitas kerja.

1. Pemantauan aktivitas
   
   Dengan menambah user baru, Anda dapat mencatat aktivitas yang dilakukan oleh setiap user. Ini memungkinkan Anda untuk mengetahui apa yang telah dilakukan user dan mengambil tindakan yang diperlukan jika terjadi masalah.

1. Pemisahan data
   
   Menambah user baru memungkinkan Anda untuk memisahkan data dan aktivitas yang berbeda, sehingga Anda dapat menjaga privasi dan keamanan data.

1. Audit
   
   Menambah user baru memungkinkan untuk memantau dan mengevaluasi aktivitas dari setiap user, sehingga anda dapat mengevaluasi efektifitas dari setiap user dalam sistem operasi.

## Langkah dan Perintah Terminal untuk Menambah User pada Debian 11

Berikut 2 skenario dalam pembuatan atau penambahan user baru pada Debian 11

1. User `debian` dibuat menggunakan akun `root`
2. User `debian11` dibuat menggunakan akun `osboxes` (akun lain dengan akses sudo)
 
### Menggunakan akun root

1. Login sebagai `root`

    ![](/assets/img/2023-01-06-membuat-user-linux/01.png)

2. Buat user dengan ketik perintah berikut

    ```
    # useradd debian
    ```

3. Atur password untuk user baru dengan ketik perintah berikut

    ```
    # passwd debian
    ```

4. Ketik password dan konfirmasi

    ![](/assets/img/2023-01-06-membuat-user-linux/02.png)
   
5. Login dengan user baru
   
    ![](/assets/img/2023-01-06-membuat-user-linux/03.png)

6. Konfirmasi user yang sedang login dengan ketik perintah berikut
   
   ```
   $ whoami
   ```

   ![](/assets/img/2023-01-06-membuat-user-linux/04.png)

### Menggunakan akun lain dengan akses sudo

1. Login sebagai user dengan akses sudo
   
    ![](/assets/img/2023-01-06-membuat-user-linux/05.png)

1. Buat user dengan ketik perintah berikut
   
    ```
    $ sudo useradd debian11
    ```
1. Ketik password untuk user dengan akses sudo

    ![](/assets/img/2023-01-06-membuat-user-linux/06.png)
   
2. Atur password untuk user baru dengan ketik perintah berikut

    ```
    $ sudo passwd debian11
    ```

3. Ketik password dan konfirmasi

    ![](/assets/img/2023-01-06-membuat-user-linux/07.png)

4. Login dengan user baru
   
    ![](/assets/img/2023-01-06-membuat-user-linux/08.png)

5. Konfirmasi user yang sedang login dengan ketik perintah berikut
   
   ```
   $ whoami
   ```

   ![](/assets/img/2023-01-06-membuat-user-linux/09.png)

## Langkah dan Perintah Terminal untuk Menambah User pada Rocky Linux 8

Berikut 2 skenario dalam pembuatan atau penambahan user baru pada Rocky Linux 8

1. User `rocky` dibuat menggunakan akun `root`
2. User `rocky8` dibuat menggunakan akun `rockylinux` (akun lain dengan akses sudo)

### Menggunakan akun oot

1. Login sebagai `root`

    ![](/assets/img/2023-01-06-membuat-user-linux/10.png)

2. Buat user dengan ketik perintah berikut

    ```
    # useradd rocky
    ```

3. Atur password untuk user baru dengan ketik perintah berikut

    ```
    # passwd rocky
    ```

4. Ketik password dan konfirmasi

    ![](/assets/img/2023-01-06-membuat-user-linux/11.png)
   
5. Login dengan user baru
   
    ![](/assets/img/2023-01-06-membuat-user-linux/12.png)

6. Konfirmasi user yang sedang login dengan ketik perintah berikut
   
   ```
   $ whoami
   ```

   ![](/assets/img/2023-01-06-membuat-user-linux/13.png)

### Menggunakan akun lain dengan akses sudo

1. Login sebagai user dengan akses sudo
   
    ![](/assets/img/2023-01-06-membuat-user-linux/14.png)

1. Buat user dengan ketik perintah berikut
   
    ```
    $ sudo useradd rocky8
    ```
   
1. Atur password untuk user baru dengan ketik perintah berikut

    ```
    $ sudo passwd rocky8
    ```

1. Ketik password dan konfirmasi

    ![](/assets/img/2023-01-06-membuat-user-linux/15.png)

4. Login dengan user baru
   
    ![](/assets/img/2023-01-06-membuat-user-linux/16.png)

5. Konfirmasi user yang sedang login dengan ketik perintah berikut
   
   ```
   $ whoami
   ```

   ![](/assets/img/2023-01-06-membuat-user-linux/17.png)

## Penutup

Saya merasa sangat terhormat dan mengucapkan terima kasih sudah berkunjung ke blog NGLINUX ini. Saya berharap anda akan menemukan sesuatu yang bermanfaat di sini.

Salam, Angga.