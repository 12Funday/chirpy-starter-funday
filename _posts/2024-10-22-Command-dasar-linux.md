---
title: Pemahaman Dasar Linux
date: 2024-10-22 14:57:03 +0800
categories: [linux]
tags: [linux, bash script]
author: 12funday
---

## Pembuka

Salam,

Linux, sebagai salah satu sistem operasi paling populer di dunia, menawarkan fleksibilitas dan kekuatan yang luar biasa. Namun, untuk benar-benar memanfaatkan potensi Linux, penting bagi kita untuk memahami perintah dasar yang menjadi fondasi interaksi dengan sistem. Memahami perintah dasar linux akan sangat membantu pengoperasian sebuah sistem. Mengapa? Berikut beberapa alasannya: 

1. **Efisiensi**: Pengelolaan sistem menggunakan *Command Line Interface* (CLI) akan lebih cepat dan menghemat penggunaan resource daripada menggunakan *graphical user interface* (GUI).

2. **Kontrol lebih luas**: Dengan menggunakan CLI, kamu bisa mengontrol sistem operasi secara lebih mendetail, melakukan pengaturan dan troubleshooting dengan lebih baik.

3. **Automatisasi**: Banyak *task* bisa diotomatisasi menggunakan *shell script*, yang sangat berguna untuk meningkatkan produktivitas.

4. **Pengembangan dan DevOps**: Banyak alat pengembangan modern dan praktik DevOps bergantung pada Linux, jadi pemahaman tentang perintah dasar linux akan sangat membantu di bidang itu.

5. **Keamanan**: Mengerti perintah dasar juga bisa membantu dalam memahami dan mengelola keamanan sistem dengan lebih baik.

## Command Dasar Linux 

Berikut beberapa perintah dasar yang sering digunakan dalam pengelolan perangkat linux.

1. Menampilkan *working directory*
    `ls`
2. Membuat folder
    `mkdir <nama folder>`
3. Masuk ke dalam folder atau *change directory*
    `cd <nama folder>`
4. Membuat file
    `touch <nama file>`
    atau menggunakan editor, dalam case ini nano editor
    `nano <nama file>`
    untuk menyimpan perubahan tekan tombol `ctrl+o` kemudian konfirmasi dengan tekan `enter`
5. Menampilkan isi file