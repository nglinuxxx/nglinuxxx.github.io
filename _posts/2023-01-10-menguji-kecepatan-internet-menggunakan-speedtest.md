---
layout: post
title: Menguji Kecepatan Internet Menggunakan Speedtest (speedtest-cli)
date: 2023-01-10 00:00 +0000
author: angga
categories: [Konfigurasi]
tags: [linux, server, debian]
---

## Pendahuluan

Halo teman-teman semua,

Kali ini saya akan berbagi informasi tentang langkah untuk instalasi dan menjalankan aplikasi terminal penguji jaringan internet bernama speedtest-cli.


## Apa itu speedtest-cli

Speedtest-cli adalah aplikasi berbasis text/terminal yang dapat digunakan untuk memeriksa kecepatan koneksi internet Anda. 

Aplikasi ini menggunakan layanan [speedtest.net](https://www.speedtest.net/){:target="_blank"} untuk mengukur kecepatan unduh, unggah, dan ping dari koneksi internet yang Anda gunakan. 

Speedtest-cli memungkinkan pengguna untuk menguji koneksi internet melalui terminal tanpa harus membuka web browser atau mengunduh aplikasi pihak ketiga untuk menguji koneksi internet melalui terminal. 

Selain itu, speedtest-cli dapat digunakan untuk mengotomatiskan pengujian kecepatan internet dengan skrip atau aplikasi lain. 

Speedtest-cli tersedia untuk berbagai sistem operasi, termasuk Linux, macOS, dan Windows, dan dapat diinstal melalui terminal atau dapat dengan mudah diinstal melalui package manager.

## Mengapa Butuh Instal speedtest-cli

Berikut adalah beberapa alasan mengapa kita harus menginstal Speedtest-cli pada komputer Linux kita.

1. Menguji kecepatan internet
   
    Speedtest-cli memungkinkan pengguna untuk dengan mudah memeriksa kecepatan unduh, unggah, dan ping koneksi Internet mereka saat ini melalui terminal.

2. Otomatisasi pengukuran kecepatan internet

    Speedtest-cli juga dapat digunakan untuk mengotomatiskan pengujian kecepatan Internet dengan skrip atau aplikasi lain. Ini sangat berguna untuk memantau kualitas koneksi Internet Anda dan memberi tahu Anda jika kecepatan Internet Anda turun di bawah batas tertentu.

3. Membantu memecahkan masalah berkaitan dengan koneksi Internet. 

    Jika terjadi masalah koneksi Internet, Speedtest-cli dapat digunakan untuk menentukan pihak mana yang bermasalah - klien atau ISP.

4. Mempertahankan kinerja sistem. 

    Kecepatan internet yang rendah dapat menyebabkan kinerja sistem menjadi lambat, sehingga dengan menggunakan Speedtest-cli untuk mengecek kecepatan internet secara teratur, pengguna dapat memonitor kinerja sistem dan mengidentifikasi masalah koneksi internet yang mempengaruhi kinerja sistem.
    
    Speedtest-cli dapat pula digunakan untuk memonitor performa sistem dan mengidentifikasi masalah koneksi internet yang mempengaruhi performa sistem.

5. Aplikasi berbasis terminal

    Speedtest-cli adalah aplikasi baris perintah yang berjalan pada terminal. Hal ini memungkinkan pengguna untuk memeriksa kecepatan internet melalui terminal tanpa harus membuka browser atau memuat aplikasi pihak ketiga.

Kesimpulannya, menginstal Speedtest-cli di komputer Linux dapat membantu pengguna memonitor kualitas koneksi internet, mengatasi masalah koneksi internet, dan menjaga kinerja sistem.

## Kebutuhan Dasar untuk Instal speedtest-cli

Persyaratan dasar untuk menginstal dan menjalankan speedtest-cli pada Linux adalah sebagai berikut.

1. Sistem operasi

    dapat diinstal pada berbagai distribusi Linux, termasuk Ubuntu, Debian, dan CentOS. 
    
    Pastikan bahwa sistem operasi mendukung instalasi Python 2.4 atau yang lebih baru.

    Pada postingan ini akan dicoba instalasi speedtest-cli menggunakan Debian 11.

1. Python

    karena Speedtest-cli ditulis dalam bahasa pemrograman Python, pastikan Python telah terinstal pada sistem Anda.

1. Koneksi internet

    Instalasi dilakukan menggunakan package manager mengambil sumber dari repository masing-masing distro, untuk itu dibutuhkan koneksi internet.
    
    Selain itu juga, untuk dapat memeriksa kecepatan koneksi internet Anda, tentu saja pastikan sistem Anda terhubung ke jaringan internet.

1. Terminal

    Speedtest-cli adalah aplikasi baris perintah yang berjalan pada terminal. 
    
    Pastikan sistem Anda memiliki akses ke terminal.

    Jika di-install pada Linux server, maka tidak perlu khawatir karena bahkan interaksi dilakukan secara terminal based/cli.

## Langkah Instalasi dan Eksekusi speedtest-cli

Dari halaman resmi [panduang instalasi speedtest-cli](https://www.speedtest.net/apps/cli){:target="_blank"} dapat diikuti langkah untuk melakukan instalasi sebagai berikut

1. Download package curl dengan mengeksekusi perintah berikut

    ```bash
    $ sudo apt install curl
    ```

    ![](/assets/img/2023-01-10-menguji-kecepatan-internet-menggunakan-speedtest/01.png){: .normal }

1. Tambahkan alamat speedtest-cli ke file repository source dengan mengeksekusi perintah berikut

    ```bash
    $ curl -s https://packagecloud.io/install/repositories/ookla/speedtest-cli/script.deb.sh | sudo bash
    ```

    ![](/assets/img/2023-01-10-menguji-kecepatan-internet-menggunakan-speedtest/02.png){: .normal }

2. Update sistem dengan mengeksekusi perintah berikut

    ```bash
    $ sudo apt update
    ```

    ![](/assets/img/2023-01-10-menguji-kecepatan-internet-menggunakan-speedtest/03.png){: .normal }

3. Install speedtest-cli dengan mengeksekusi perintah berikut

    ```bash
    $ sudo apt install speedtest-cli
    ```

    ![](/assets/img/2023-01-10-menguji-kecepatan-internet-menggunakan-speedtest/04.png){: .normal }

4. Setelah ter-install, uji jaringan dengan mengeksekusi perintah berikut

    ```bash
    $ speedtest-cli
    ```

    ![](/assets/img/2023-01-10-menguji-kecepatan-internet-menggunakan-speedtest/05.png){: .normal }

    atau jika ingin lebih simple tampilan hanya upload dan download bisa mengeksekusi perintah berikut

    ```bash
    $ speedtest-cli --simple
    ```

    ![](/assets/img/2023-01-10-menguji-kecepatan-internet-menggunakan-speedtest/06.png){: .normal }

## Penutup

Saya merasa sangat terhormat dan mengucapkan terima kasih sudah berkunjung ke blog [NGLINUX](https://nglinux.com){:target="_blank"} ini. Saya berharap anda akan menemukan sesuatu yang bermanfaat di sini.

Salam, Angga.