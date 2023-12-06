# Jarkom-Modul-4-F09-2023
Laporan resmi praktikum jaringan komputer modul 4 kelompok F09
## Anggota Kelompok
| Nama                        | NRP        |
|-----------------------------|------------|
| Muhammad Daffa Harits       | 5025211005 |
| Muhammad Naufal Baihaqi     | 5025211103 |
## Soal Praktikum Modul 4
![Screenshot 2023-11-28 235649 (1)](https://github.com/LuvinVictii/Jarkom-Modul-4-F09-2023/assets/78089862/ad13c6f0-857a-4f50-9386-75523ff210dd)

1. Soal shift dikerjakan pada Cisco Packet Tracer dan GNS3 menggunakan metode perhitungan CLASSLESS yang berbeda.
2. Jika tidak ada pemberitahuan revisi soal dari asisten, berarti semua soal BERSIFAT BENAR dan DAPAT DIKERJAKAN.
3. Untuk di GNS3 CLOUD merupakan NAT1 jangan sampai salah agar bisa terkoneksi internet.
4. Pembagian IP menggunakan Prefix IP yang telah ditentukan pada modul pengenalan
5. Pembagian IP dan routing harus SE-EFISIEN MUNGKIN.

<br>
<hr>
<br>
> Hal yang perlu diperhatikan
1. Gunakan prefix IP sesuai dengan prefix IP masing-masing.
2. Terdapat template spreadsheet untuk mempermudah penilaian, gunakan template tersebut untuk melakukan penghitungan subnetting.
3. Hasil perhitungan subnetting dan pohon pembagian IP serta file .pkt di submit pada link di atas.
4. File yang didemokan adalah file .pkt yang telah disubmi5t
5. Pengurangan nilai akan dilakukan ketika:
   - Melanggar salah satu dari tulisan diatas.
   - Tidak menggunakan PREFIX ip yang ditetapkan sebelumnya
   - Hasil perhitungan untuk VLSM / CIDR, berbeda dengan di CPT / GNS3
   - Pembagian IP kurang efisien
   - Routing kurang efisien
   - Tidak bisa menjelaskan cara perhitungan VLSM dan CIDR

## Penamaan Subnetting
Penamaan dan pembagian subnetting kelompok kami sebagai berikut:

![image](https://github.com/LuvinVictii/Jarkom-Modul-4-F09-2023/assets/78089862/c10fd7d1-426d-48bf-b484-7e1bb694a5f9)

Lalu dari situ, kami mencatatnya dalam sheet sebagai berikut:

![image](https://github.com/LuvinVictii/Jarkom-Modul-4-F09-2023/assets/78089862/37437be1-6dae-406e-a507-9e8149d2b78f)

# CIDR
Kelompok kami menggunakan <i>Cisco Packet Tracer</i> (CPT) untuk metode CIDR
## Membuat Topologi Di CPT

![image](https://private-user-images.githubusercontent.com/115441787/288444262-0db19bdf-d318-40c1-88d2-62bee2a659b3.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE3MDE4NzQyOTQsIm5iZiI6MTcwMTg3Mzk5NCwicGF0aCI6Ii8xMTU0NDE3ODcvMjg4NDQ0MjYyLTBkYjE5YmRmLWQzMTgtNDBjMS04OGQyLTYyYmVlMmE2NTliMy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMjA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTIwNlQxNDQ2MzRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0xZTVmMThmNDRiYmU5NDRjYjMxMTM2NjlmNmQ1YTc4YmE4ODk2MjAxNDczOGFiYzFlMmMxZDEzNGQxYTg3MmJjJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.px2mmBxdBBtneNpc-gxBcoJh7ZiLS73kx2Lb714X9ME)

# VLSM
Kelompok kami menggunakan <i>GNS3</i> untuk metode VLSM


| Subnet  | IP | Alias  |  Subnet Mask  | Lenght  |
| ----- | ----- | ----- | ----- | ----- |
| A1 | 10.56.0.0 | Fern-switch4-AppetitRegion-Switch4-LaubHills | 255.255.248.0 | 1023 |
| A2 | 10.56.28.0 | Flamme-Fern | 255.255.255.252 | 2 |
| A3 | 10.56.8.0 | Flamme-Switch5-RohrRoad | 255.255.252.0 | 1001 |
| A4 | 10.56.30.0 | Himmel-Switch6-SchwerMountains | 255.255.255.248 | 6 |
| A5 | 10.56.28.4 | Himmel-Flamme | 255.255.255.252 | 2 |
| A6 | 10.56.28.8 | Flamme-Frieren | 255.255.255.252 | 2 |
| A7 | 10.56.30.96 | Frieren-Switch3-LakeKorridor | 255.255.255.224 | 25 |
| A8 | 10.56.28.12 | Frieren-Aura | 255.255.255.252 | 2 |
| A9 | 10.56.30.8 | Eisen-Switch1-Richter-Switch1-Revolte | 255.255.255.248 | 3 |
| A10 | 10.56.12.0 | Heiter-Switch8-Sein-Switch8-RiegelCanyon | 255.255.252.0 | 512 |
| A11 | 10.56.31.192 | Lawine-Switch7-BredRegion-Switch7-Heiter | 255.255.255.192 | 31 |
| A12 | 10.56.28.16 | Linie-Lawine | 255.255.255.252 | 2 |
| A13 | 10.56.24.0 | Linie-Switch11-GranzChannel | 255.255.254.0 | 255 |
| A14 | 10.56.28.20 | Eisen-Linie | 255.255.255.252 | 2 |
| A15 | 10.56.26.0 | Lugner-Switch9-GrobeForest | 255.255.255.0 | 251 |
| A16 | 10.56.16.0 | Lugner-Switch10-TurkRegion | 255.255.252.0 | 1001 |
| A17 | 10.56.29.0 | Eisen-Lugner | 255.255.255.252 | 2 |
| A18 | 10.56.29.4 | Eisen-Switch0-Stark | 255.255.255.252 | 2 |
| A19 | 10.56.29.8 | Aura-Eisen | 255.255.255.252 | 2 |
| A20 | 10.56.27.0 | Denken-Switch2-RoyalCapital-Switch2-WilleRegion | 255.255.255.0 | 127 |
| A21 | 10.56.29.12 | Aura-Denken | 255.255.255.252 | 2 |


### Network Configuration

1. Sein
```
auto eth0
iface eth0 inet static
	address 10.56.12.3
	netmask 255.255.252.0
	gateway 10.56.12.1
```

2. RiegelCanyon
```
auto eth0
iface eth0 inet static
	address 10.56.12.2
	netmask 255.255.252.0
	gateway 10.56.12.1
```
3. Heiter
```
# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.31.193
	netmask 255.255.255.192
        gateway 10.56.31.194

# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.12.1
	netmask 255.255.252.0


up route add -net 10.56.29.4 netmask 255.255.255.252 gw 10.56.31.194

up route add -net 10.56.27.0 netmask 255.255.255.0 gw 10.56.31.194
```
4. BredRegion
```
auto eth0
iface eth0 inet static
	address 10.56.31.195
	netmask 255.255.254.0
	gateway 10.56.31.194
```
5. Lawine
```

# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.28.18
	netmask 255.255.255.252
        gateway 10.56.28.17



# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.31.194
	netmask 255.255.255.192

#daftar route
up route add -net 10.56.12.0 netmask 255.255.252.0 gw 10.56.31.193

```
6. GranzChannel
```
auto eth0
iface eth0 inet static
	address 10.56.24.2
	netmask 255.255.254.0
	gateway 10.56.24.1
```
7. Linie
```
# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.28.22
	netmask 255.255.255.252
        gateway 10.56.28.21


# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.28.17
	netmask 255.255.255.252


# Static config for eth2
auto eth2
iface eth2 inet static
	address 10.56.24.1
	netmask 255.255.254.0



#routing eth1
up route add -net 10.56.28.16 netmask 255.255.255.252 gw 10.56.28.18

#daftar route
up route add -net 10.56.31.192 netmask 255.255.255.192 gw 10.56.28.18

up route add -net 10.56.12.0 netmask 255.255.252.0 gw 10.56.28.18

up route add -net 10.56.29.4 netmask 255.255.255.252 gw 10.56.28.21

up route add -net 10.56.30.8 netmask 255.255.255.248 gw 10.56.28.21
```
8. Ricther
```
auto eth0
iface eth0 inet static
	address 10.56.30.11
	netmask 255.255.255.248
	gateway 10.56.30.9
```
9. Revolte
```
auto eth0
iface eth0 inet static
	address 10.56.30.10
	netmask 255.255.255.248
	gateway 10.56.30.9
```
10. TurkRegion
```
auto eth0
iface eth0 inet static
	address 10.56.16.2
	netmask 255.255.252.0
	gateway 10.56.16.1
```
11. GrobeForest
```
auto eth0
iface eth0 inet static
	address 10.56.26.2
	netmask 255.255.255.0
	gateway 10.56.26.1
```
12. Lugner
```
# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.29.2
	netmask 255.255.255.252
        gateway 10.56.29.1

# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.26.1
	netmask 255.255.255.0

# Static config for eth2
auto eth2
iface eth2 inet static
	address 10.56.16.1
	netmask 255.255.252.0
```
13. Stark
```
auto eth0
iface eth0 inet static
	address 10.56.29.6
	netmask 255.255.255.252
	gateway 10.56.29.5
```
14. Eisen
```
# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.29.10
	netmask 255.255.255.252
        gateway 10.56.29.9


# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.29.5
	netmask 255.255.255.252


# Static config for eth2
auto eth2
iface eth2 inet static
	address 10.56.30.9
	netmask 255.255.255.248



# Static config for eth3
auto eth3
iface eth3 inet static
	address 10.56.29.1
	netmask 255.255.255.252


# Static config for eth4
auto eth4
iface eth4 inet static
	address 10.56.28.21
	netmask 255.255.255.252



#routing eth3
up route add -net 10.56.29.0 netmask 255.255.255.252 gw 10.56.29.2

#routing eth4
up route add -net 10.56.28.20 netmask 255.255.255.252 gw 10.56.28.22

#daftar route
up route add -net 10.56.24.0 netmask 255.255.254.0 gw 10.56.28.22

up route add -net 10.56.26.0 netmask 255.255.255.0 gw 10.56.29.2

up route add -net 10.56.16.0 netmask 255.255.252.0 gw 10.56.29.2

up route add -net 10.56.28.16 netmask 255.255.255.252 gw 10.56.28.22

up route add -net 10.56.31.192 netmask 255.255.255.192 gw 10.56.28.22

up route add -net 10.56.12.0 netmask 255.255.252.0 gw 10.56.28.22

up route add -net 10.56.27.0 netmask 255.255.255.0 gw 10.56.29.9
```
15. RoyalCapital
```
auto eth0
iface eth0 inet static
	address 10.56.27.2
	netmask 255.255.255.0
	gateway 10.56.27.1
```
16. WilleRegion
```
auto eth0
iface eth0 inet static
	address 10.56.27.3
	netmask 255.255.255.0
	gateway 10.56.27.1
```
17. Denken
```
# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.29.14
	netmask 255.255.255.252
        gateway 10.56.29.13

# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.27.1
	netmask 255.255.255.0

# routing eth0
up route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.56.29.13
```
18. SchweMountains
```
auto eth0
iface eth0 inet static
	address 10.56.30.2
	netmask 255.255.255.248
	gateway 10.56.30.1
```
19. Himmel
```
# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.28.6
	netmask 255.255.255.252
        gateway 10.56.28.5

# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.30.1
	netmask 255.255.255.248
```
20. RohrRoad
```
auto eth0
iface eth0 inet static
	address 10.56.8.2
	netmask 255.255.252.0
	gateway 10.56.8.1
```
21. AppetitRegion
```
auto eth0
iface eth0 inet static
	address 10.56.0.2
	netmask 255.255.248.0
	gateway 10.56.0.1
```
22. LaubHilis
```
auto eth0
iface eth0 inet static
	address 10.56.0.3
	netmask 255.255.248.0
	gateway 10.56.0.1
```
23. Fern
```
# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.28.2
	netmask 255.255.255.252
        gateway 10.56.28.1

# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.0.1
	netmask 255.255.248.0

```
24. Flamme
```
# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.28.10
	netmask 255.255.255.252
        gateway 10.56.28.9

# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.28.1
	netmask 255.255.255.252


# Static config for eth2
auto eth2
iface eth2 inet static
	address 10.56.8.1
	netmask 255.255.252.0

# Static config for eth3
auto eth3
iface eth3 inet static
	address 10.56.28.5
	netmask 255.255.255.252


up route add -net 10.56.0.0 netmask 255.255.248.0 gw 10.56.28.2
up route add -net 10.56.30.0 netmask 255.255.255.248 gw 10.56.28.6
```
25. LakeKorridor
```
auto eth0
iface eth0 inet static
	address 10.56.30.98
	netmask 255.255.255.224
	gateway 10.56.30.97
```
26. Frieren
```
# Static config for eth0
auto eth0
iface eth0 inet static
	address 10.56.28.14
	netmask 255.255.255.252
        gateway 10.56.28.13

# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.30.97
	netmask 255.255.255.224

# Static config for eth2
auto eth2
iface eth2 inet static
	address 10.56.28.9
	netmask 255.255.255.252



#routing eth2
up route add -net 10.56.0.0 netmask 255.255.248.0 gw 10.56.28.10

up route add -net 10.56.8.0 netmask 255.255.252.0 gw 10.56.28.10

up route add -net 10.56.30.0 netmask 255.255.255.248 gw 10.56.28.10
```
27. Aura
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet dhcp

# Static config for eth1
auto eth1
iface eth1 inet static
	address 10.56.29.13
	netmask 255.255.255.252

# Static config for eth2
auto eth2
iface eth2 inet static
	address 10.56.28.13
	netmask 255.255.255.252


# Static config for eth3
auto eth3
iface eth3 inet static
	address 10.56.29.9
	netmask 255.255.255.252



# routing eth1
up route add -net 10.56.27.0 netmask 255.255.255.0 gw 10.56.29.14

# routing eth2
up route add -net 10.56.30.96 netmask 255.255.255.224 gw 10.56.28.14

# routing eth3
up route add -net 10.56.29.8 netmask 255.255.255.252 gw 10.56.29.10

up route add -net 10.56.28.20 netmask 255.255.255.252 gw 10.56.29.10

up route add -net 10.56.24.0 netmask 255.255.254.0 gw 10.56.29.10

up route add -net 10.56.28.16 netmask 255.255.255.252 gw 10.56.29.10

up route add -net 10.56.12.0 netmask 255.255.252.0 gw 10.56.29.10

up route add -net 10.56.31.192 netmask 255.255.255.192 gw 10.56.29.10

#routing kiri

up route add -net 10.56.30.96 netmask 255.255.255.224 gw 10.56.28.14

up route add -net 10.56.28.8 netmask 255.255.255.252 gw 10.56.28.14

up route add -net 10.56.28.0 netmask 255.255.255.252 gw 10.56.28.14

up route add -net 10.56.0.0 netmask 255.255.248.0 gw 10.56.28.14

up route add -net 10.56.8.0 netmask 255.255.252.0 gw 10.56.28.14

up route add -net 10.56.28.4 netmask 255.255.255.252 gw 10.56.28.14

up route add -net 10.56.30.0 netmask 255.255.255.248 gw 10.56.28.14
```