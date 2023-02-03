---
title:  "Atur Spesifikasi Sumber Daya untuk Memulai Penggunaan VM pada VirtualBox"
author: angga
categories: [Tutorial]
tags: [linux]
---

## Pendahuluan

Halo teman-teman semua,

Kali ini saya akan berbagi informasi tentang langkah untuk mengatur sumber daya/resources dan memulai hasil import file image dari sistem operasi linux, yang nantinya akan bisa kita gunakan untuk belajar konfigurasi.

## Mengatur Sumber Daya

Sebelum menjalankan linux baik server maupun desktop sebagai virtual machine (vm) di VirtualBox, Anda perlu mengatur beberapa pengaturan dasar untuk memastikan bahwa sistem dapat berjalan dengan baik. 

Untuk mengganti pengaturan sesuai kebutuhan anda, yang perlu dilakukan yaitu pilih pada suatu virtual machine, lalu klik tombol Settings

![](/assets/img/2023-01-05-memulai-vbox-image-linux/01.png)

Berikut adalah beberapa pengaturan yang perlu diperhatikan:

1. RAM/memory
   
   Pastikan Anda menetapkan jumlah RAM yang cukup untuk sistem Anda. 
   
   Misalkan untuk server pada distro seperti Debian bisa menggunakan di angka 256 MB, namun untuk desktop jumlah yang dianjurkan setidaknya 2 GB atau lebih.

   ![](/assets/img/2023-01-05-memulai-vbox-image-linux/02.png)

2. CPU
   
   Pastikan Anda menetapkan jumlah CPU yang cukup untuk sistem Anda. 
   
   Misalkan untuk server pada distro seperti Debian bisa menggunakan di angka 1, namun untuk desktop jumlah yang dianjurkan adalah setidaknya 2 atau lebih.

   ![](/assets/img/2023-01-05-memulai-vbox-image-linux/03.png)

3. GPU atau Video Memory
   
   Jika Anda ingin menjalankan aplikasi yang memerlukan dukungan GPU, pastikan Anda mengaktifkan dukungan GPU di VirtualBox.

   Misalkan untuk server pada distro seperti Debian bisa menggunakan di angka 16 MB, namun untuk desktop jumlah yang dianjurkan setidaknya 128 GB atau lebih.

   ![](/assets/img/2023-01-05-memulai-vbox-image-linux/04.png)

4. Network
   
   Pastikan Anda mengatur jenis koneksi yang sesuai dengan konfigurasi jaringan Anda. 
   
   Jika Anda ingin agar jaringan vm terisolir hanya untuk vm itu sendiri, namun tetap bisa terkoneksi dengan jaringan internet, maka Anda bisa memilih koneksi sebagai "NAT".

   Sedangkan, jika Anda hanya membutuhkan koneksi antar vm saja tanpa harus terkoneksi dengan jaringan host, maka anda bisa memilih koneksi sebagai "Internal Network".

   Namun, jika Anda ingin mengakses server dari luar jaringan internal, pastikan Anda mengatur koneksi sebagai "Bridged Adapter".

   ![](/assets/img/2023-01-05-memulai-vbox-image-linux/05.png)

   Atau bisa menggunakan pengaturan jaringan lainnya.

## Memulai Virtual Machine

Berikut 4 kombinasi username dan password untuk login virtual machine hasil download dari situs `osboxes.org` dan `linuxvmimages.com` yaitu:

### VM dari osboxes.org

Dalam hal ini menggunakan Debian 11 Server (64-bit)

1. akun root
   
    | User | Password |
    |:---:|:---:|
    | root | osboxes.org |

    ![](/assets/img/2023-01-05-memulai-vbox-image-linux/06.png)

2. akun dengan akses sudo

    | User | Password |
    |:---:|:---:|
    | osboxes | osboxes.org |

    ![](/assets/img/2023-01-05-memulai-vbox-image-linux/07.png)

List lengkap username dan password untuk distro tersedia dapat dilihat [di sini](https://www.osboxes.org/virtualbox-images/).
   
### VM dari linuxvmimages.com

Dalam hal ini menggunakan Rocky Linux 8 Server (64-bit)

1. akun root

    | User | Password |
    |:---:|:---:|
    | root | linuxvmimages.com |

    ![](/assets/img/2023-01-05-memulai-vbox-image-linux/08.png)

2. akun dengan akses sudo

    | User | Password |
    |:---:|:---:|
    | rockylinux | rockylinux |

    ![](/assets/img/2023-01-05-memulai-vbox-image-linux/09.png)

List lengkap username dan password untuk distro tersedia dapat dilihat [di sini](https://www.linuxvmimages.com/how-to-use/vm-image-password/).

## Penutup

Saya merasa sangat terhormat dan mengucapkan terima kasih sudah berkunjung ke blog NGLINUX ini. Saya berharap anda akan menemukan sesuatu yang bermanfaat di sini.

Salam, Angga.