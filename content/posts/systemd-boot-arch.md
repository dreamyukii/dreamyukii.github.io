+++
title = 'Konfigurasi systemd-boot dengan GPU AMD'
date = 2024-02-19T01:22:40+07:00
draft = true
+++

Hari ini 5 April 2024 saya memutuskan mencoba menggunakan ArchLinux lagi sebagai os utama di komputer saya, instalasi berjalan lancar sampai ketika ingin menkonfigurasi plymouth ada masalah, plymouth tidak mau muncul dan stuck saat booting.
Lalu saya mencari solusi di archwiki dan archlinux forum, ternyata solusinya mudah sekali, yaitu menambahkan hook amdgpu di /etc/mkinitcpio.conf dan amdgpu modeset di kernel argument.
[archforum post](https://bbs.archlinux.org/viewtopic.php?id=258397)