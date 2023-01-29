---
title:  "Import File Image VirtualBox Siap Pakai"
author: angga
categories: [Tutorial]
tags: [Linux]
---

# Pendahuluan

Halo teman-teman semua,

Kali ini saya akan berbagi informasi tentang langkah untuk meng-import hasil download file image dari sistem operasi linux, yang nantinya akan bisa kita gunakan untuk belajar konfigurasi.

# Langkah Import File Image ke VirtualBox

Karena perbedaan file extension yang disediakan oleh masing-masing situs, maka langkah import dan konfigurasi awal juga sedikit berbeda, yaitu 

## Hasil Download dari Situs [osboxes.org](https://www.osboxes.org)

1. Pastikan folder hasil extract download tersedia

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/01.png)

1. Buka VirtualBox

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/02.png)

1. Klik tombol "New"

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/03.png)

1. Isi kolom "Name", klik tombol "Next"

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/04.png)

1. Atur memory/RAM yang sesuai, klik tombol "Next"

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/05.png)

1. Pilih "Use an existing virtual hard disk file", klik tombol "Choose ..."

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/06.png)

1. Klik tombol "Add", abaikan sementara jendela browse file

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/07.png)

1. Pindahkan file hasil download ke folder VM yang baru saja diinisiasi
    
    1. Buka Windows Explorer, lakukan perintah `Cut`/`Copy` pada file image sistem operasi Linux yang telah diunduh

        ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/08.png)

    1. Pindah ke folder VM dari Virtualbox, biasanya di `C:\Users\<username>\VirtualBox VMs\`

        ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/09.png)

    1. Buka folder VM baru sesuai yang sudah diinisiasi sebelumnya, lakukan perintah `Paste` pada file image sistem operasi Linux

        ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/10.png)

1. Setelah file *.vdi tersedia di folder VM baru, pilih file dan klik tombol "Open"

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/11.png)

1. Pada jendela Hard Disk Selector, pilih VM yang baru saja di-import, klik tombol "Choose"

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/12.png)

1. Klik tombol "Create"

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/13.png)

1. VM siap digunakan

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/14.png)

## Hasil Download dari Situs [linuxvmimages.com](https://www.linuxvmimages.com)

1. Pastikan folder hasil extract download tersedia

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/a01.png)

1. Lakukan perintah `Cut`/`Copy` pada folder hasil extract dari hasil download

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/a02.png)

1. Pindah ke folder VM dari Virtualbox, biasanya di `C:\Users\<username>\VirtualBox VMs\`, lakukan perintah `Paste` untuk folder yang di-cut/di-copy

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/a03.png)

1. Buka VirtualBox, klik tombol "Add"

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/a04.png)
    
1. Cari file image sistem operasi Linux yang akan di-import

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/a05.png)

1. Klik tombol "Open"

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/a06.png)

1. VM siap digunakan

    ![](/assets/img/2023-01-04-import-vbox-image-linux-siap-pakai/a07.png)

# Kesimpulan

File image sistem operasi Linux dapat dengan mudah diunduh dan diimport ke VirtualBox dari beberapa situs seperti [https://www.osboxes.org](https://www.osboxes.org) dan [https://www.linuxvmimages.com](https://www.linuxvmimages.com)

File image sistem operasi Linux siap digunakan setelah proses import selesai dilakukan.

Username dan password bawaan disediakan oleh situs download tersebut, walau tidak menutup kemungkinan untuk nantinya bisa dibuat user baru.

# Penutup

Saya merasa sangat terhormat dan mengucapkan terima kasih sudah berkunjung ke blog NGLINUX ini. Saya berharap anda akan menemukan sesuatu yang bermanfaat di sini.

Salam, Angga.