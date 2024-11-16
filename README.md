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

## Rute dan Area Subnet
![image](https://github.com/user-attachments/assets/207c4883-8f00-4a12-8f59-b583578f004b)

## Penggabungan
### Langkah 1
![Langkah 1](https://github.com/user-attachments/assets/73b5a01c-c708-4f6e-a271-dbb25cf9730f)

### Langkah 2
![Langkah 2](https://github.com/user-attachments/assets/3f7310b7-3257-438a-b326-85df7c2fb553)
![image](https://github.com/user-attachments/assets/636227d5-04d5-40c6-a1c7-b36ea6074425)

### Langkah 3
![Langkah 3](https://github.com/user-attachments/assets/e67b5cef-4045-43ad-965b-b53573cb2a03)
![image](https://github.com/user-attachments/assets/dde80184-0c66-40b6-91fb-8532ff4d9bee)

### Langkah 4
![Langkah 4](https://github.com/user-attachments/assets/bbebf72f-b3fd-4077-958d-194c33c261c4)
![image](https://github.com/user-attachments/assets/ac6e315e-acf9-49d1-a8aa-6fe2d7541d33)

### Langkah 5
![Langkah 5](https://github.com/user-attachments/assets/9a472580-2cc9-448d-a98b-c0e0484cd5c7)
![image](https://github.com/user-attachments/assets/b02dfa15-399a-458f-9ba0-92d3567b96e4)

### Langkah 6
![Langkah 6](https://github.com/user-attachments/assets/006e3c23-0520-45fb-885f-eb8a5777fd20)
![image](https://github.com/user-attachments/assets/db10634d-da92-40ed-82dd-1c35c050626c)

### Langkah 7
![Langkah 7](https://github.com/user-attachments/assets/c1cefb47-6ed2-44c8-8802-694be8e89f44)
![image](https://github.com/user-attachments/assets/2c4a589a-e9ea-40a8-9db4-8712e5a39147)

### Langkah 8
![Langkah 8](https://github.com/user-attachments/assets/bc22281e-c441-45eb-8e93-8267cf575244)
![image](https://github.com/user-attachments/assets/d9a8a4cd-13d5-4c13-9184-d7d64e1a1917)

### Langkah 9
![Langkah 9](https://github.com/user-attachments/assets/b5f105d2-8ec3-4ff9-9d19-566346845a0a)
![image](https://github.com/user-attachments/assets/42a5a7f4-c79d-440b-ae71-651dfae0d598)

### Langkah 10
![Langkah 10](https://github.com/user-attachments/assets/4121bfc0-df8b-4bbd-a7af-d359c35ab1e6)
![image](https://github.com/user-attachments/assets/1bf463e0-898d-49d1-83be-4932b5c99a5e)

### Langkah 11
![Langkah 11](https://github.com/user-attachments/assets/eb6d9958-c762-48f6-ac5a-dbc0afa2a492)
![image](https://github.com/user-attachments/assets/1ddd7b0d-39e3-4713-919c-1d7257270681)

## Pembagian IP
![image](https://github.com/user-attachments/assets/0e765711-0f1f-49b7-96ab-3c5f1ac0dc49)

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

### Gura_Ame_Ina (Client)
```
#A17
auto eth0
iface eth0 inet static
    address 10.76.64.2
    netmask 255.255.254.0
    gateway 10.76.64.1
```

### Kiara_Calli (Client)
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

### Holo-ID (Gateway)
```
#A1
auto eth0
iface eth0 inet static
    address 10.78.4.6
    netmask 255.255.255.252

#A2
auto eth1
iface eth1 inet static
    address 10.78.4.1
    netmask 255.255.255.252

#A4
auto eth2
iface eth2 inet static
    address 10.78.16.65
    netmask 255.255.255.252

#A6
auto eth3
iface eth3 inet static
    address 10.78.34.1
    netmask 255.255.255.252
```

### AREA15 (Gateway)
```
#A2
auto eth0
iface eth0 inet static
    address 10.78.4.2
    netmask 255.255.255.252
    gateway 10.76.4.1

#A3
auto eth1
iface eth1 inet static
    address 10.78.0.1
    netmask 255.255.252.0
```

### lofi (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 10.78.0.2
    netmask 255.255.252.0
    gateway 10.78.0.1
```

### Moona (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 10.78.0.3
    netmask 255.255.252.0
    gateway 10.78.0.1
```

### Risu (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 10.78.0.4
    netmask 255.255.252.0
    gateway 10.78.0.1
```

### holoro (Gateway)
```
#A4
auto eth0
iface eth0 inet static
    address 10.78.16.66
    netmask 255.255.255.252
    gateway 10.78.16.65

#A5
auto eth1
iface eth1 inet static
    address 10.78.16.1
    netmask 255.255.252.192
```

### Ollie (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 10.78.16.2
    netmask 255.255.252.192
    gateway 10.78.16.1
```

### Anya (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 10.78.16.3
    netmask 255.255.252.192
    gateway 10.78.16.1
```

### Reine (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 10.78.16.4
    netmask 255.255.252.192
    gateway 10.78.16.1
```

### holoh3ro (Gateway)
```
#A6
auto eth0
iface eth0 inet static
    address 10.78.34.2
    netmask 255.255.255.252
    gateway 10.78.34.1

#A7
auto eth1
iface eth1 inet static
    address 10.78.32.1
    netmask 255.255.254.0
```

### Zeta (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 10.78.32.2
    netmask 255.255.254.0
    gateway 10.78.32.1
```

### Kaela (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 10.78.32.3
    netmask 255.255.254.0
    gateway 10.78.32.1
```

### Kobo (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 10.78.32.4
    netmask 255.255.254.0
    gateway 10.78.32.1
```

### Holo-JP (Gateway)
```
#A8
auto eth0
iface eth0 inet static
    address 10.76.10.25
    netmask 255.255.255.252

#A9
auto eth1
iface eth1 inet static
    address 10.76.10.1
    netmask 255.255.255.252
```

### DEV_IS (Gateway)
```
#A9
auto eth0
iface eth0 inet static
    address 10.76.10.2
    netmask 255.255.255.252
    gateway 10.78.10.1

#A10
auto eth1
iface eth1 inet static
    address 10.76.10.9
    netmask 255.255.255.240
```

### Ririka_Raden (Client)
```
#A10
auto eth0
iface eth0 inet static
    address 10.76.10.10
    netmask 255.255.255.240
    gateway 10.78.10.9
```

### Ao (Client)
```
#A10
auto eth0
iface eth0 inet static
    address 10.76.10.11
    netmask 255.255.255.240
    gateway 10.78.10.9
```

### Hajime_Kanade (Client)
```
#A10
auto eth0
iface eth0 inet static
    address 10.76.10.12
    netmask 255.255.255.240
    gateway 10.78.10.9
```

### GEN:0 (Gateway)
```
#A9
auto eth0
iface eth0 inet static
    address 10.76.10.3
    netmask 255.255.255.252
    gateway 10.78.10.1

#A11
auto eth1
iface eth1 inet static
    address 10.76.0.1
    netmask 255.255.248.0
```

### MiComet (Client)
```
#A11
auto eth0
iface eth0 inet static
    address 10.76.0.2
    netmask 255.255.248.0
    gateway 10.76.0.1
```

### Sora_Robo_AZKi (Client)
```
#A11
auto eth0
iface eth0 inet static
    address 10.76.0.3
    netmask 255.255.248.0
    gateway 10.76.0.1
```

### GEN:1 (Gateway)
```
#A11
auto eth0
iface eth0 inet static
    address 10.76.0.4
    netmask 255.255.248.0
    gateway 10.76.0.1

#A12
auto eth1
iface eth1 inet static
    address 10.76.8.1
    netmask 255.255.254.0

#A13
auto eth2
iface eth2 inet static
    address 10.76.4.129
    netmask 255.255.255.252
```

### FBK_Matsuri (Client)
```
#A12
auto eth0
iface eth0 inet static
    address 10.76.8.2
    netmask 255.255.248.0
    gateway 10.76.8.1
```

### Aki_Hachama (Client)
```
#A12
auto eth0
iface eth0 inet static
    address 10.76.8.3
    netmask 255.255.248.0
    gateway 10.76.8.1
```

### Gamers (Gateway)
```
#A13
auto eth0
iface eth0 inet static
    address 10.76.4.130
    netmask 255.255.255.252
    gateway 10.76.4.129

#A14
auto eth1
iface eth1 inet static
    address 10.76.4.1
    netmask 255.255.255.128
```

### Korone (Client)
```
#A14
auto eth0
iface eth0 inet static
    address 10.76.4.2
    netmask 255.255.255.128
    gateway 10.76.4.1
```

### Okayu (Client)
```
#A14
auto eth0
iface eth0 inet static
    address 10.76.4.3
    netmask 255.255.255.128
    gateway 10.76.4.1
```

### Mio (Client)
```
#A14
auto eth0
iface eth0 inet static
    address 10.76.4.4
    netmask 255.255.255.128
    gateway 10.76.4.1

```
