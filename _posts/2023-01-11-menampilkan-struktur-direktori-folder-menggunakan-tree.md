---
layout: post
title: Menampilkan Struktur Direktori/Folder Menggunakan Tree
date: 2023-01-11 00:00 +0000
author: angga
categories: [Konfigurasi]
tags: [linux, server, debian]
---

## Pendahuluan

Halo teman-teman semua,

Kali ini saya akan berbagi informasi tentang langkah untuk instalasi dan menjalankan aplikasi terminal untuk menampilkan informasi struktur direktori/folder bernama tree.

## Apa itu tree?

Tree adalah perangkat lunak atau aplikasi baris perintah yang digunakan untuk menampilkan direktori dan struktur file sistem operasi. 

Tree membuat tampilan menjadi hierarkis dan mudah dibaca, sehingga memudahkan pengguna untuk melihat struktur file dan direktori dengan jelas. 

Tree memungkinkan pengguna untuk melihat semua direktori dan subdirektori dari sistem operasi, sehingga lebih mudah untuk mengelola file dan direktori.

## Mengapa Butuh Instal tree

Berikut adalah beberapa alasan mengapa tree perlu diinstal di suatu komputer:

1. Memudahkan navigasi direktori dan file

    Tree ini menampilkan direktori dan struktur file dalam bentuk hierarki yang jelas untuk memudahkan pengguna dalam menavigasi dan mengelola file.

2. Menghemat waktu
    
    Tree memungkinkan pengguna untuk menelusuri struktur direktori dan file dengan lebih cepat dan lebih efisien daripada menelusuri direktori satu per satu.

3. Meningkatkan produktivitas

    Tree dapat meningkatkan produktivitas pengguna dengan memberikan tampilan yang jelas tentang struktur file dan direktori sistem operasi dan dengan membuatnya lebih mudah untuk mengelola dan mengatur file.

4. Memudahkan debugging

    Tree ini juga dapat membantu pengguna melakukan debug pada program mereka, karena pohon ini dapat menunjukkan struktur direktori dan berkas-berkas yang terkait dengan program tersebut.

5. Konsistensi antar sistem operasi
    
    Tree tersedia untuk sistem operasi yang berbeda dan membantu menjaga konsistensi ketika berjalan pada sistem operasi yang berbeda.

## Penggunaan

Jika ingin menampilkan informasi detail pada saat mengeksekusi perintah tree, dapat menggunakan beberapa parameter tambahan. 

Berikut ini adalah beberapa parameter penting yang dapat digunakan:

1. -a atau --all

    Parameter ini akan menampilkan semua file dan direktori, termasuk file dan direktori yang dianggap tersembunyi oleh sistem operasi.

1. -h atau --human-readable

    Parameter ini akan menampilkan ukuran file dan direktori dalam format yang mudah dipahami oleh manusia, seperti KB, MB, atau GB.

1. -f atau --full-path

    Parameter ini akan menampilkan nama file dan direktori beserta dengan path atau alamat lengkapnya.

1. -i atau --ignore

    Parameter ini dapat digunakan untuk mengabaikan file atau direktori yang diinginkan dari tampilan tree.

1. -L atau --level
    
    Parameter ini dapat digunakan untuk menentukan kedalaman atau level direktori yang akan ditampilkan.

1. -D atau --dirsfirst

    Parameter ini akan menampilkan direktori terlebih dahulu sebelum file ketika menampilkan tampilan tree.

## Langkah Instalasi dan Eksekusi tree

1. Update sistem dengan mengeksekusi perintah berikut

    ```bash
    $ sudo apt update
    ```

    ![](/assets/img/2023-01-11-menampilkan-struktur-direktori-folder-menggunakan-tree/01.png){: .normal }

2. Install tree dengan mengeksekusi perintah berikut

    ```bash
    $ sudo apt install tree
    ```

    ![](/assets/img/2023-01-11-menampilkan-struktur-direktori-folder-menggunakan-tree/02.png){: .normal }

3. Setelah ter-install, buka suatu direktori yang berisi direktori dan file lain di dalamnya, tampilkan struktur folder dengan mengeksekusi perintah berikut

    ```bash
    $ cd folder_bertingkat
    $ tree .
    ```

    ![](/assets/img/2023-01-11-menampilkan-struktur-direktori-folder-menggunakan-tree/03.png){: .normal }

    atau jika ingin lebih detail tampilannya bisa mengeksekusi perintah berikut

    ```bash
    $ tree . -h
    ```

    ![](/assets/img/2023-01-11-menampilkan-struktur-direktori-folder-menggunakan-tree/04.png){: .normal }

## Penutup

Saya merasa sangat terhormat dan mengucapkan terima kasih sudah berkunjung ke blog [NGLINUX](https://nglinux.com){:target="_blank"} ini. Saya berharap anda akan menemukan sesuatu yang bermanfaat di sini.

Salam, Angga.