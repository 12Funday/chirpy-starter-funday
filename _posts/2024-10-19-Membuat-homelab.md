---
title: Membangun Homelab Server part 1
date: 2024-10-18 15:00:03 +0800
categories: [homelab]
tags: [homelab, server, proxmox]     # TAG names should always be lowercase
author: 12funday
---

## Pembuka
Salam,

Memiliki *homelab server* merupakan kebutuhan bagi orang yang punya rasa penasaran yang tinggi seperti saya. Selain bisa jadi sarana "utak-atik", memiliki *homelab server* juga saya harap bisa menjadi sarana belajar yang "aman" karena apabila nanti saya "fucked up" saya tidak merugikan siapa pun.

Pada tulisan ini, saya akan menceritakan bagaimana saya membangun *Homelab server* pribadi saya dari nol, dan apa saja yang saya lakukan dengan *homelab* ini.

## Hardware

Adapun perangkat keras yang saya gunakan untuk membangun *homelab server* sederhana saya adalah sebagai berikut.

1. HP ThinClient T620 plus (F5A60AA)

    Memilih device yang mumpuni untuk kebutuhan *homelab* ini memakan proses yang lumayan panjang, banyak pertimbangan yang harus saya perhatikan dalam memilih perangkat yang saya gunakan. Salah satu yang paling penting adalah budget *(hehe)*. Dan akhrirnya pilihan saya jatuh pada HP ThinClient T620 plus.

    <img src="/assets/img/tc-1.png" alt="ThinClient T620 Plus" width="200"/>

    Spesifikasi dari HP ThinClient T620 plus adalah sebagai berikut:

    - Processor AMD GX-420CA 2GHz (4 cores 4 threads)
    - AMD Radeon HD 8400E
    - Memory 4 GB
    - Storage 16 GB

    Jumlah core pada processor yang dimiliki oleh HP ThinClient T620 plus menjadi salah satu alasan penting dalam saya memilih perangkat ini sebagai senjata utama saya membangun *homelab server* pribadi saya. Dengan harga yang cukup terjangkau, kita ditawarkan processor dengan jumlah inti 4 cores dan 4 threads dan kecepatan hingga 2GHz. Selain itu, device ini juga sudah mendukung *virtualization*. Saya harap device ini nanti bisa menjalankan beberapa *virtual machine* bersamaan.

    Namun, untuk menjalankan beberapa *virtual machine* secara bersamaan tidak akan mungkin dengan memory hanya 4GB dan Storage 16GB. Untuk itu, saya melakukan upgrade memory 8GB dan storage menjadi 128GB.

2. TPLINK TL-WR840N
    
    Benar! Apa itu *homelab* tanpa koneksi internet?
    Beruntungnya saya, fasilitas koneksi internet telah disediakan oleh penyedia kost dengan kualitas koneksi yang stabil dan *transfer rate* yang lumayan cepat.

    Namun, sayangnya HP ThinClient T620 plus tidak disertai oleh wifi adaptor. Saya memiliki 2 pilihan agar *homelab* ini dapat koneksi internet. Membeli wifi adaptor atau menghubungkan device ini dengan kabel LAN dan konektor RJ-45. 

    Berbagai pertimbangan saya lakukan hingga akhirnya saya memimilih untuk membeli TPLINK TL-WR840N. Selain harganya yang terjangkau, device ini juga memiliki 4 mode penggunaan yaitu *Router mode, Access Point mode, Range extender mode,* dan *WISP mode*. Wah... mungkin kedepan alat ini bisa kita "utak-atik" juga hehe.

    <img src="/assets/img/tplink.png" alt="TPLINK TL-WR840N" width="200"/>


3. Video Capture


    Monitor! Tentu saja kita perlu alat untuk menampilkan output device yang kita gunakan. Baik dalam proses instalasi maupun ketika menggunakannya sehari-hari nanti. Tapi, karena meja saya sempit dan sehari-hari kerja dengan laptop yang udah ada monitornya. Sepertinya tidak butuh-butuh amat untuk membeli monitor.

    Lalu, bagaimana saya akan mengoperasikan *homelab* ini nantinya? Setelah riset beberapa hari akhirnya ketemulah solusinya, *video capture card*. Alat ini biasanya digunakan oleh para streamer untuk menampilkan output video dari source yang berbeda seperti PS3, PS4, dll. Wah.. Keren banget, pasti harganya mahal? Oh tidak juga, ternyata ada yang menjualnya dengan harga di bawah Rp. 100 ribu.

    <img src="/assets/img/vccard.png" alt="Video Capture Card" width="200"/>


## Operating System

Pemilihan sistem operasi merupakan satu hal yang sangat krusial dalam membangun *homelab*. Karena pemilihan sistem operasi akan sangat mempengaruhi *environment* ritual "utak-atik" kita nantinya.

Ada beberapa pilihan sistem operasi yang menjadi pertimbangan saya dalam membanung *homelab* ini.

**1. OS dengan Dekstop Environment**

 <img src="/assets/img/linux-1.png" alt="linux" width="200"/>

Menggunakan dekstop environment berbasis linux ataupun windows tentunya akan sangat memudahkan dalam pengoperasian *homelab* ini nanti. Pada dekstop kita gunakan virtualbox untuk menginstal beberapa *virtual machine*. Namun, menggunakan *dekstop environment* saya kira akan sangat boros resorce nantinya. Dalam keadaan *idle* pun penggunaan CPU dan Memory mesin dengan *desktop environment* lumayan gede.

**2. Casa OS**

<img src="/assets/img/casa-1.png" alt="casa OS" width="200"/>

Casa OS sangat populer digunakan sebagai sistem operasi dalam pembuatan *homelab server* karena pengoperasiaannya sangat mudah, cukup buka browser dan klik klik klik. Namun, kemudahan yang ditawarkan ini sangat berseberangan dengan semangat "utak-atik" yang saya miliki *(hehe)*

**3. Virtualization Platform**

Virtualization adalah teknologi yang mampu membuat satu komputer atau server menjalankan beberapa sistem operasi secara berasamaan menggunakan satu mesin fisik yang sama. Salah satu platform yang digunakan untuk virtualization adalah **Proxmox Virtual Environment**

<img src="/assets/img/proxmox-1.png" alt="Proxmox Virtual Environment" width="200"/>

**Proxmox** dapat melakukan 2 jenis *virtualization* yaitu *Kernel Based Virtualization* dan *Container-based virtualization*. Proxmox dilengkapi dengan *web-based management interface* sehingga dalam pengoperasiannya bisa sangat mudah melalui browser. Berarti, saya dapat mengoperasikan proxmox melalui HP atau tablet. Konon katanya, proxmox juga ada mobile appsnya yang bisa diinstall melalui playstore.

> Keren parah!! Yaudah kita pakai proxmox aja.


## Penutup

Sekian tulisan hari ini, untuk proses setup dan installasi, akan saya ceritakan di part 2.