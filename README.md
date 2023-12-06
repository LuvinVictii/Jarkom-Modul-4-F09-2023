# Jarkom-Modul-4-F09-2023

# CIDR - CPT

# VLSM - GNS3


| Subnet | Alias | IP | Subnet Mask | Lenght |

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