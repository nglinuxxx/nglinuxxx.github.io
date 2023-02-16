---
layout: post
title: Menampilkan Informasi Sistem Menggunakan Neofetch
date: 2023-01-09 00:00 +0000
author: angga
categories: [Konfigurasi]
tags: [linux, server, debian, rocky]
---

## Pendahuluan

Halo teman-teman semua,

Kali ini saya akan berbagi informasi tentang langkah untuk instalasi dan menjalankan aplikasi terminal bernama neofetch.

## Apa itu Neofetch

Dari [github repo Neofetch](https://github.com/dylanaraps/neofetch){:target="_blank"}, aplikasi/package ini didefinisikan sebagai adalah aplikasi yang berjalan secara command line/terminal based yang menampilkan informasi sistem suatu komputer. 

Memang didesain untuk kebutuhan main-masin, namun aplikasi Neofetch ini dapat menampilkan informasi tentang sistem operasi, perangkat lunak, dan perangkat keras Anda dengan cara yang estetis dengan visual yang lebih menarik ketimbang teks biasa.

Informasi sistem ini nantinya dapat digunakan sebagai objek screenshot yang bisa dibagikan kepada orang lain, misalkan saja di media sosial.

Jika perintah `neofetch` berhasil dieksekusi, hasil daftar informasi selengkapnya akan ditampilkan di sebelah logo sistem operasi yang sedang anda pakai. 

## Mengapa Butuh Meng-install Neofetch

Melakukan instalasi Neofetch pada komputer Anda dapat memberikan beberapa kemudahan, antara lain

1. Kemudahan melihat informasi sistem yang berjalan

    Neofetch memungkinkan Anda untuk dengan cepat dan mudah melihat informasi tentang sistem Anda, seperti sistem operasi, kernel, prosesor/CPU, memori/RAM, kartu grafis dan lebih banyak lagi. 
    
    Hal ini tentunya dapat membantu Anda menentukan apakah semuanya berjalan dengan benar atau bisa digunakan untuk melakukan tracing jika suatu saat terjadi masalah/kendala pada sistem.

2. Menampilkan tabel informasi sistem

    Dengan Neofetch ini, Anda dapat membuat tabel yang memberikan gambaran rinci tentang sistem Anda. 
    
    Tentunya hal ini dapat berguna sebagai bahan troubleshoot khusunya ketika Anda mencoba melakukan perbandingan spesifikasi beberapa komputer.

3. Mengambil tangkapan layar/screenshot sistem dengan lebih menarik

    Dengan Neofetch, Anda dapat mengambil tangkapan layar dari sistem Anda dan menampilkannya dengan informasi dalam format visual yang menarik. 
    
    Ini memungkinkan Anda untuk dengan mudah berbagi informasi dengan orang lain seperti di media sosial.
    
    Manfaat lain juga Anda dapat melakukan berbagi informasi sistem dengan keterbacaan yang jelas, jika suatu saat Anda harus meminta bantuan orang lain dalam menyelesaikan suatu pemasalah yang dihadapi.

4. Penyesuaian terhadap output yang dihasilkan

    Anda dapat menyesuaikan output Neofetch sesuai keinginan Anda. 
    
    Anda dapat memilih informasi apa yang akan ditampilkan dan menentukan bagaimana informasi tersebut harus diformat.

Maka, melakukan installasi Neofetch pada sistem komputer Anda dapat memberikan berbagai manfaat yang berguna dan dapat menjadi alat bantu untuk pemecahan masalah yang dihadapi, bisa juga digunakan untuk membandingkan dengan sistem komputer lain, serta berbagi informasi sistem Anda kepada orang lain.

## Langkah Instalasi dan Eksekusi Neofetch

### Pada Debian 11

1. Buka Terminal
2. Update repository dengan perintah 

    ```bash
    $ sudo apt update
    ```

    ![](/assets/img/2023-01-09-menampilkan-informasi-sistem-menggunakan-neofetch/01.png){: .normal }

3. Install Neofetch dengan perintah

    ```bash
    $ sudo apt install neofetch
    ```

    ![](/assets/img/2023-01-09-menampilkan-informasi-sistem-menggunakan-neofetch/02.png){: .normal }

    ![](/assets/img/2023-01-09-menampilkan-informasi-sistem-menggunakan-neofetch/03.png){: .normal }

4. Jalankan Neofetch dengan perintah

    ```bash
    $ neofetch
    ```

    ![](/assets/img/2023-01-09-menampilkan-informasi-sistem-menggunakan-neofetch/04.png){: .normal }

### Pada Rocky 8

1. Buka Terminal
2. Menambahkan repository EPEL dengan perintah berikut

    ```bash
    $ sudo yum install epel-release
    ```
    
    ![](/assets/img/2023-01-09-menampilkan-informasi-sistem-menggunakan-neofetch/05.png){: .normal }

3. Update repository dengan perintah 
   
   ```bash
    $ sudo yum makecache --refresh
    ```

    ![](/assets/img/2023-01-09-menampilkan-informasi-sistem-menggunakan-neofetch/06.png){: .normal }

4. Install Neofetch dengan perintah
   
   ```bash
    $ sudo yum install neofetch
    ```

    ![](/assets/img/2023-01-09-menampilkan-informasi-sistem-menggunakan-neofetch/07.png){: .normal }

5. Jalankan Neofetch dengan perintah

    ```bash
    $ neofetch
    ```

    ![](/assets/img/2023-01-09-menampilkan-informasi-sistem-menggunakan-neofetch/08.png){: .normal }

## Penutup

Saya merasa sangat terhormat dan mengucapkan terima kasih sudah berkunjung ke blog [NGLINUX](https://nglinux.com){:target="_blank"} ini. Saya berharap anda akan menemukan sesuatu yang bermanfaat di sini.

Salam, Angga.