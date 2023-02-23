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

Dari [repositori github Neofetch](https://github.com/dylanaraps/neofet){:target="_blank"}, aplikasi/paket ini didefinisikan sebagai aplikasi berbasis baris perintah/terminal yang menampilkan informasi sistem di komputer.

Memang dirancang untuk tujuan bermain game, namun aplikasi Neofetch ini dapat menampilkan informasi tentang sistem operasi, perangkat lunak, dan perangkat keras Anda secara estetis dengan visual yang lebih menarik daripada teks biasa.

Informasi sistem ini kemudian dapat digunakan sebagai objek tangkapan layar yang dapat dibagikan kepada orang lain, seperti di jejaring sosial.

Jika perintah 'neofetch' berhasil dijalankan, daftar lengkap informasi akan ditampilkan di sebelah logo sistem operasi yang sedang Anda gunakan. 

## Mengapa Butuh Meng-install Neofetch

Menginstal Neofetch di komputer Anda dapat membawa sejumlah manfaat, antara lain

1. Mudah menampilkan informasi tentang sistem yang sedang berjalan

    Neofetch memungkinkan Anda dengan cepat dan mudah melihat informasi tentang sistem Anda, seperti sistem operasi, kernel, prosesor/CPU, memori/RAM, kartu grafis, dan banyak lagi.

    Tentu saja, ini dapat membantu Anda menentukan apakah semuanya berfungsi dengan baik atau dapat digunakan untuk memantau jika suatu saat terjadi kesalahan / hambatan dalam sistem.

2. Menampilkan panel informasi sistem

    Dengan Neofetch ini Anda dapat membuat tabel yang memberikan gambaran rinci tentang sistem Anda. Tentu saja, ini berguna saat memecahkan masalah perangkat keras, terutama saat mencoba membandingkan spesifikasi beberapa komputer.

3. Tangkapan layar/tangkapan layar sistem dengan cara yang lebih menyenangkan

    Dengan Neofetch, Anda dapat mengambil screenshot dari sistem Anda dan menampilkannya bersama dengan informasi dalam format visual yang menarik.

    Ini memungkinkan Anda untuk dengan mudah berbagi informasi dengan orang lain, seperti di media sosial.

    Keuntungan lainnya adalah Anda dapat membagikan informasi sistem dengan keterbacaan yang jelas, jika suatu saat Anda perlu meminta bantuan orang lain untuk menyelesaikan masalah yang Anda hadapi. 4. Sesuaikan output

4. Anda dapat menyesuaikan keluaran Neofetch sesuai keinginan Anda.

    Anda dapat memilih informasi apa yang akan ditampilkan dan menentukan bagaimana formatnya.

    Oleh karena itu, menginstal Neofetch pada sistem komputer Anda dapat memberikan berbagai manfaat yang bermanfaat dan dapat menjadi alat untuk memecahkan masalah yang dihadapi, juga dapat digunakan untuk membandingkan dengan sistem komputer lain dan berbagi informasi tentang sistem Anda dengan orang lain. 

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