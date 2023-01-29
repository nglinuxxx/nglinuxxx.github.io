---
title:  "Belajar Linux menggunakan Komputer Asli atau Virtual Machine"
author: angga
categories: [Blog]
tags: [Linux]
---

# Pendahuluan

Halo teman-teman semua,

Berikut pengalaman saya ketika belajar linux. Mungkin dapat membantu teman-teman semua untuk menentukan apakah cara belajar Linux yang tepat dengan menggunakan mesin asli yang terinstall sistem operasi Linux, ataukah dengan menggunakan teknologi virtualisasi seperti VirtualBox, VMware, atau Parallels Desktop.

# Mesin Asli vs Virtualisasi

## Instalasi sistem operasi

Cara pertama untuk belajar Linux adalah dengan menginstall sistem operasi Linux secara fisik di mesin asli. Hal ini membutuhkan partisi disk yang terpisah dan proses instalasi yang cukup rumit. 

Sedangkan cara kedua adalah dengan menggunakan virtualisasi, yang hanya membutuhkan file image sistem operasi Linux yang sudah terdownload dan proses import yang relatif lebih mudah. 

File image sistem operasi Linux di VirtualBox yang siap digunakan adalah file yang berisi konfigurasi sistem operasi Linux yang sudah terinstall di mesin virtual di dalam VirtualBox. 

File ini biasanya disimpan dalam format ".ova" (Open Virtualization Appliance) atau ".vmdk" (Virtual Machine Disk). 

File ini dapat dengan mudah diunduh dari web seperti 

> [https://www.osboxes.org/](https://www.osboxes.org/) 

atau 

> [https://www.linuxvmimages.com/](https://www.linuxvmimages.com/)

## Ketersediaan hardware

Mesin asli yang terinstall sistem operasi Linux membutuhkan hardware yang kompatibel dengan sistem operasi tersebut. Hal ini bisa menjadi masalah jika hardware yang dimiliki tidak kompatibel dengan sistem operasi Linux yang ingin dipelajari. 

Sedangkan dengan virtualisasi, sistem operasi Linux dapat dijalankan di atas mesin virtual yang terinstall di mesin asli, sehingga tidak terpaku pada kompatibilitas hardware.

![](/assets/img/2023-01-02-belajar-linux-real-vs-virtual/Picture1.jpg)

## Akses root

Pada sistem operasi Linux yang terinstall di mesin asli, anda biasanya memiliki akses root yang memungkinkan anda untuk mengubah konfigurasi sistem dan menginstall aplikasi dengan mudah. 

Sedangkan pada mesin virtual, anda biasanya tidak memiliki akses root dan harus menggunakan perintah-perintah tertentu untuk mengubah konfigurasi sistem atau menginstall aplikasi.

![](/assets/img/2023-01-02-belajar-linux-real-vs-virtual/Picture2.jpg)

## Kemampuan untuk menggunakan sistem operasi lain secara bersamaan

Mesin asli yang terinstall sistem operasi Linux hanya dapat menjalankan satu sistem operasi saja. 

Sedangkan dengan virtualisasi, anda dapat menjalankan beberapa sistem operasi secara bersamaan dalam satu mesin asli.

![](/assets/img/2023-01-02-belajar-linux-real-vs-virtual/Picture3.jpg)

## Kemampuan untuk membackup dan restore sistem operasi

Dengan virtualisasi, anda dapat dengan mudah membackup dan restore sistem operasi yang dijalankan di mesin virtual. 

Sedangkan pada mesin asli yang terinstall sistem operasi Linux, proses backup dan restore biasanya lebih rumit dan membutuhkan waktu yang lebih lama.

![](/assets/img/2023-01-02-belajar-linux-real-vs-virtual/Picture4.jpg)

# Penutup

Saya merasa sangat terhormat dan mengucapkan terima kasih sudah berkunjung ke blog NGLINUX ini. Saya berharap anda akan menemukan sesuatu yang bermanfaat di sini.

Salam, Angga.