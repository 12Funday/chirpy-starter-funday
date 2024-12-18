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
Setelah memiliki file ISO proxmox, yang perlu dilakukan selanjutnya adalah membuat media instalasi. Saya menggunakan ventoy. Langkah-langkahnya adalah seperti berikut:
1. Download ventoy pada [official page](https://www.ventoy.net/en/download.html) ventoy.
2. Menghubungkan USB Drive ke komputer, kemudian install Ventoy.
3. Setelah selesai installasi, copy file ISO Proxmox ke Drive Ventoy.

### Langkah 3 : Instalasi Proxmox pada komputer
Setelah menyiapkan media instalasi, saya langsung melakukan instalasi pada HP ThinClient milik saya.

