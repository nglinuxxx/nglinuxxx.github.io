---
layout: post
title: Menghapus User pada Linux
date: 2023-01-08 00:00 +0000
author: angga
categories: [Konfigurasi]
tags: [linux, server, debian, rocky]
---

## Pendahuluan

Halo teman-teman semua,

Kali ini saya akan berbagi informasi tentang langkah untuk menghapus user yang sudah tidak diperlukan, pada sistem operasi linux terutama server menggunakan perintah terminal.

## Catata Penting Sebelum Menghapus User

Beberapa catatan penting yang perlu dipertimbangkan ketika menghapus user pada Linux adalah:

1. Backup data
   
   Sebelum menghapus user, pastikan untuk membuat cadangan dari semua file yang dibuat oleh user tersebut. Setelah user dihapus, semua file yang dibuat oleh user tersebut akan hilang.

2. Pemindahan file
   
   Jika Anda ingin menyimpan file yang dibuat oleh user yang akan dihapus, pastikan untuk memindahkan file tersebut ke lokasi yang aman.

3. Pemindahan hak akses
   
   Jika ada file atau direktori yang dibagikan dengan user lain, pastikan untuk memindahkan hak akses ke user lain sebelum menghapus user.

4. Pemindahan konfigurasi
   
   Jika user yang dihapus memiliki konfigurasi yang digunakan oleh sistem, pastikan untuk memindahkan konfigurasi tersebut ke user lain atau mengubah konfigurasi sistem sebelum menghapus user.

5. Pemindahan tugas
   
   Jika user yang dihapus memiliki tugas yang harus dilakukan, pastikan untuk memindahkan tugas tersebut ke user lain sebelum menghapus user.

6. Audit
   
   Pastikan untuk melakukan audit setelah menghapus user, untuk memastikan tidak ada masalah yang terjadi.

## Perintah Terminal untuk Menghapus User pada Debian 11

Terdapat 2 skenario penghapusan user,

1. jika hanya butuh untuk menghapus akun user saja maka perintah terminal sebagai berikut

    ```bash
    root@debian:~# deluser `username`
    ```

    sedangkan

1. jika kebutuhan untuk menghapus akun user beserta folder home-nya maka perintah terminal sebagai berikut

    ```bash
    root@debian:~# deluser `username` --remove-home
    ```

## Langkah untuk Menghapus User pada Debian 11

Untuk proses penghapusan terhadap suatu user di Debian 11 ini, masih menggunakan 2 skenario yang sama seperti [artikel sebelumnya](/posts/membuat-user-linux){:target="_blank"} ketika pembuatan atau penambahan user baru

1. untuk user `debian` proses hapus hanya user dilakukan menggunakan akun `root`, sedangkan 
2. untuk user `debian11` proses hapus sekaligus folder home dilakukan menggunakan akun `osboxes` (akun lain dengan akses sudo)

### Dari akun root

1. Login sistem sebagai `root`
2. Menghapus user `debian` dengan ketik perintah berikut
   
    ![](/assets/img/2023-01-08-menghapus-user-pada-linux/01.png)

3. Menguji apakah user sudah terhapus dengan login ke user `debian`

    ![](/assets/img/2023-01-08-menghapus-user-pada-linux/02.png)

    Jika muncul informasi `Login incorrect`, maka penghapusan user berhasil dilakukan karena user tidak bisa ditemukan dalam sistem.
   
### Dari akun lain dengan akses sudo

1. Login sistem sebagai `osboxes`
2. Menghapus user `debian11` dengan ketik perintah berikut

    ![](/assets/img/2023-01-08-menghapus-user-pada-linux/03.png)

3. Menguji apakah user sudah terhapus dengan login ke user `debian11`

    ![](/assets/img/2023-01-08-menghapus-user-pada-linux/04.png)

    Jika muncul informasi `Login incorrect`, maka penghapusan user berhasil dilakukan karena user tidak bisa ditemukan dalam sistem.

## Perintah Terminal untuk Menghapus User pada Rocky Linux 8

Terdapat 2 skenario penghapusan user,

1. jika hanya butuh untuk menghapus akun user saja maka perintah terminal sebagai berikut

    ```bash
    [root@rocky ~]# userdel `username`
    ```

    sedangkan

1. jika kebutuhan untuk menghapus akun user beserta folder home-nya maka perintah terminal sebagai berikut

    ```bash
    [root@rocky ~]# userdel -r `username`
    ```

## Langkah untuk Menghapus User pada Rocky Linux 8

Untuk proses penghapusan terhadap suatu user di Rocky Linux 8 ini, masih menggunakan 2 skenario yang sama seperti [artikel sebelumnya](/posts/membuat-user-linux){:target="_blank"} ketika pembuatan atau penambahan user baru

1. untuk user `rocky` proses hapus hanya user dilakukan menggunakan akun `root`, sedangkan
2. untuk user `rocky8` proses hapus sekaligus folder home dilakukan menggunakan akun `rockylinux` (akun lain dengan akses sudo)

### Dari akun root

1. Login sistem sebagai `root`
2. Menghapus user `rocky` dengan ketik perintah berikut
   
    ![](/assets/img/2023-01-08-menghapus-user-pada-linux/05.png)

3. Menguji apakah user sudah terhapus dengan login ke user `rocky`

    ![](/assets/img/2023-01-08-menghapus-user-pada-linux/06.png)

    Jika muncul informasi `Login incorrect`, maka penghapusan user berhasil dilakukan karena user tidak bisa ditemukan dalam sistem.

### Dari akun lain dengan akses sudo

1. Login sistem sebagai `rockylinux`
2. Menghapus user `rocky8` dengan ketik perintah berikut

    ![](/assets/img/2023-01-08-menghapus-user-pada-linux/07.png)

3. Menguji apakah user sudah terhapus dengan login ke user `rocky8`

    ![](/assets/img/2023-01-08-menghapus-user-pada-linux/08.png)

    Jika muncul informasi `Login incorrect`, maka penghapusan user berhasil dilakukan karena user tidak bisa ditemukan dalam sistem.

## Penutup

Saya merasa sangat terhormat dan mengucapkan terima kasih sudah berkunjung ke blog NGLINUX ini. Saya berharap anda akan menemukan sesuatu yang bermanfaat di sini.

Salam, Angga.