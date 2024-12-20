---
title: Instalasi Proxmox versi 8.3
date: 2024-10-22 14:57:03 +0800
categories: [linux]
tags: [linux, proxmox]
author: 12funday
---

## Pembuka

Salam,

Pada tulisan sebelumnya, saya telah memutuskan menggunakan proxmox sebagai tools untuk mengelola homelab saya nanti. Bagaimana langkah-langkah dalam instalasi proxmox, silakan simak tulisan berikut!

---
## Persiapan

Untuk menginstal Proxmox VE pada perangkat komputer, ada beberapa hal yang perlu saya siapkan, antara lain:
1. Komputer atau laptop untuk membuat media instalasi
2. Media Instalasi (USB Drive) minimal 2GB

---
## Instalasi

### Langkah 1: Download Proxmox ISO
Mengunduh file ISO proxmox pada situs [official proxmox](https://www.proxmox.com/en/downloads). Pada saat tulisan ini dibuat, versi terbaru dalah versi 8.3. 

### Langkah 2: Menyiapkan media instalasi
Setelah memiliki file ISO proxmox, yang perlu dilakukan selanjutnya adalah membuat media instalasi, saya menggunakan rufus. Langkah-langkahnya adalah seperti berikut:
1. Download rufus pada [official page](https://rufus.ie/en/) rufus.

    ![ins_2_rufus_a.png](/images/ins_2_rufus_a.png)
    *Official web rufus*
2. Menghubungkan USB Drive ke komputer, kemudian membuat media instalasi menggunakan rufus.
    ![ins_2_rufus_b.png](/images/ins_2_rufus_b.png)
    *Tampilan rufus*

    ![ins_2_rufus_c.png](/images/ins_2_rufus_c.png)
    *Memilih file ISO*



### Langkah 3 : Instalasi Proxmox pada komputer
Setelah menyiapkan media instalasi, saya langsung melakukan instalasi pada HP ThinClient milik saya.

1. Menghubungkan USB bootable media ke komputer
2. Masuk ke boot menu

    ![ins_3_bootmenu.png](/images/ins_3_bootmenu.png)
    *Masuk boot menu*

3. Melakukan instalasi
    
    ![ins_3_proxmox_a.png](/images/ins_3_proxmox_a.png)
    *Memilih Instalasi dengan GUI*

    ![ins_3_proxmox_b.png](/images/ins_3_proxmox_b.png)
    *Boot Instalasi proxmox GUI*

    ![ins_3_proxmox_c.png](/images/ins_3_proxmox_c.png)
    *Menyetujui license agreement*

    ![ins_3_proxmox_d.png](/images/ins_3_proxmox_d.png)
    *Memilih disk target instalasi*

    ![ins_3_proxmox_e.png](/images/ins_3_proxmox_e.png)
    *Memilih location dan timezone*

    ![ins_3_proxmox_f.png](/images/ins_3_proxmox_f.png)
    *Mengatur password untuk proxmox*

    ![ins_3_proxmox_g.png](/images/ins_3_proxmox_g.png)
    *Mengatur IP dan network driver*

    ![ins_3_proxmox_h.png](/images/ins_3_proxmox_h.png)
    *Summary*

    ![ins_3_proxmox_i.png](/images/ins_3_proxmox_i.png)
    *Proses Instalasi*

    Setelah proses instalasi selesai, buka web browser dan buka IP proxmox yang telah ditentukan sebelumnya, dan masukan user dan password.

    ![ins_3_proxmox_j.png](/images/ins_3_proxmox_j.png)
    *Login proxmox*

    ![ins_3_proxmox_k.png](/images/ins_3_proxmox_k.png)
    *Web GUI proxmox*

Voila!! :tada: :tada: :tada: proxmox berhasil diinstal.


## Penutup

Sekian tulisan kali ini, untuk proses setup dan installasi vm akan saya lanjutkan nanti.