# Jarkom-Modul-4-IT25-2024

# Anggota Kelompok
| Nama  | NRP  |
|----------|----------|
| Fikri Aulia As Sa'adi  | 5027231026 |
| Nayla Raissa Azzahra  | 5027231054 |

# CPT (VLSM)

# GNS3 (CIDR)
## Topologi
![image](https://github.com/user-attachments/assets/66dd358f-1a88-4676-8ead-390ce1ece390)

## Pembagian IP

## Rute dan Area Subnet

## Tree
![TREE_JARKOM_FKRI drawio](https://github.com/user-attachments/assets/1e630aab-d20e-4149-938b-16ab39f6c8c2)

## Konfigurasi
### Hololive (Gateway)
```
#A15
auto eth1
iface eth1 inet static
    address 10.76.66.5
    netmask 255.255.255.252

#A1
auto eth2
iface eth2 inet static
    address 10.78.4.5
    netmask 255.255.255.252

#A8
auto eth3
iface eth3 inet static
    address 10.76.10.25
    netmask 255.255.255.252
```

### Holo-EN (Gateway)
```
#A15
auto eth0
iface eth0 inet static
    address 10.76.66.6
    netmask 255.255.255.252
    gateway 10.76.66.5

#A16
auto eth1
iface eth1 inet static
    address 10.76.66.1
    netmask 255.255.255.252

#A21
auto eth2
iface eth2 inet static
    address 10.76.16.33
    netmask 255.255.255.252
```

### Holo-Myth (Gateway)
```
#A16
auto eth0
iface eth0 inet static
    address 10.76.66.2
    netmask 255.255.255.252
    gateway 10.76.66.1

#A17
auto eth1
iface eth1 inet static
    address 10.76.64.1
    netmask 255.255.254.0


#A19
auto eth2
iface eth2 inet static
    address 10.76.32.65
    netmask 255.255.255.248
```

### Gura_Ame_Ina
```
#A17
auto eth0
iface eth0 inet static
    address 10.76.64.2
    netmask 255.255.254.0
    gateway 10.76.64.1
```

### Kiara_Calli
```
#A17
auto eth0
iface eth0 inet static
    address 10.76.64.3
    netmask 255.255.254.0
    gateway 10.76.64.1
```

### Holo Advent (Gateway)
```
#A21
auto eth0
iface eth0 inet static
    address 10.76.16.34
    netmask 255.255.255.252
    gateway 10.76.16.33

#A22
auto eth1
iface eth1 inet static
    address 10.76.16.1
    netmask 255.255.255.224
```

### FuwaMoco (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 10.76.16.2
    netmask 255.255.255.224
    gateway 10.76.16.1
```

### Shiori_Nerissa (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 10.76.16.3
    netmask 255.255.255.224
    gateway 10.76.16.1
```

### Biboo (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 10.76.16.4
    netmask 255.255.255.224
    gateway 10.76.16.1
```

### Project-Hope (Gateway)
```
#A19
auto eth0
iface eth0 inet static
    address 10.76.32.66
    netmask 255.255.255.248
    gateway 10.76.32.65

#A18
auto eth1
iface eth1 inet static
    address 10.76.32.73
    netmask 255.255.255.248
```

### Irys (Client)

```
#A18
auto eth0
iface eth0 inet static
    address 10.76.32.74
    netmask 255.255.255.248
    gateway 10.76.32.73
```

### Holo-Council (Gateway)
```
#A19
auto eth0
iface eth0 inet static
    address 10.76.32.67
    netmask 255.255.255.248
    gateway 10.76.32.65

#A20
auto eth1
iface eth1 inet static
    address 10.76.32.1
    netmask 255.255.255.192
```

### Kronii_Mumei (Client)
```
#A20
auto eth0
iface eth0 inet static
    address 10.76.32.2
    netmask 255.255.255.192
    gateway 10.76.32.1
```

### Bae_Fauna (Client)
```
#A20
auto eth0
iface eth0 inet static
    address 10.76.32.3
    netmask 255.255.255.192
    gateway 10.76.32.1
```
