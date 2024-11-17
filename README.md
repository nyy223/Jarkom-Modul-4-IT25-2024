# Anggota Kelompok
| Nama  | NRP  |
|----------|----------|
| Fikri Aulia As Sa'adi  | 5027231026 |
| Nayla Raissa Azzahra  | 5027231054 |

## Rute dan Area Subnet
<img width="482" alt="Screenshot 2024-11-16 at 13 02 22" src="https://github.com/user-attachments/assets/572beee2-56bd-471c-b010-4740c4e52f71">


# CPT (VLSM)
## Topologi
![Group 1](https://github.com/user-attachments/assets/065fbbef-76d8-44f1-ab64-d47ea97ec35e)

## Tree

## Pembagian IP
<img width="574" alt="Screenshot 2024-11-16 at 13 10 38" src="https://github.com/user-attachments/assets/2fd94626-44a8-44fe-b7b8-1f7488bfcc8d">

## Konfigurasi
### Hololive (Router)
Interfaces
```
Fast Ethernet0/1 (A1)
- IPv4 Address : 10.76.19.73
- Subnet Mask : 255.255.255.252
Fast Ethernet1/0 (A8)
- IPv4 Address : 10.76.19.89
- Subnet Mask : 255.255.255.252
Fast Ethernet1/1 (A15)
- IPv4 Address : 10.76.19.97
- Subnet Mask : 255.255.255.252
```
Static Routes
```
(A2)
- Network : 10.76.19.76
- Mask : 255.255.255.252
- Next Hop : 10.76.19.74

(A3)
- Network : 10.76.8.0
- Mask : 255.255.252.0
- Next Hop : 10.76.19.74

(A4)
- Network : 10.76.19.80
- Mask : 255.255.255.252
- Next Hop : 10.76.19.74

(A5)
- Network : 10.76.18.128
- Mask : 255.255.255.192
- Next Hop : 10.76.19.74

(A6)
- Network : 10.76.19.84
- Mask : 255.255.255.252
- Next Hop : 10.76.19.74

(A7)
- Network : 10.76.12.0
- Mask : 255.255.254.0
- Next Hop : 10.76.19.74

(A10)
- Network : 10.76.19.32
- Mask : 255.255.255.240
- Next Hop : 10.76.19.90

(A11)
- Network : 10.76.0.0
- Mask : 255.255.248.0
- Next Hop : 10.76.19.90

(A12)
- Network : 10.76.14.0
- Mask : 255.255.254.0
- Next Hop : 10.76.19.90

(A13)
- Network : 10.76.19.92
- Mask : 255.255.255.252
- Next Hop : 10.76.19.90

(A14)
- Network : 10.76.18.0
- Mask : 255.255.255.128
- Next Hop : 10.76.19.90

(A16)
- Network : 10.76.19.100
- Mask : 255.255.255.252
- Next Hop : 10.76.19.98

(A17)
- Network : 10.76.16.0
- Mask : 255.255.254.0
- Next Hop : 10.76.19.98

(A18)
- Network : 10.76.19.56
- Mask : 255.255.255.248
- Next Hop : 10.76.19.98

(A20)
- Network : 10.76.18.192
- Mask : 255.255.255.192
- Next Hop : 10.76.19.98

(A21)
- Network : 10.76.19.104
- Mask : 255.255.255.252
- Next Hop : 10.76.19.98

(A22)
- Network : 10.76.19.0
- Mask : 255.255.255.224
- Next Hop : 10.76.19.98
```
### Holo-ID (Router)
Interfaces
```
Fast Ethernet0/0 (A1)
- IPv4 Address : 10.76.19.74
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A2)
- IPv4 Address : 10.76.19.77
- Subnet Mask : 255.255.255.252

Fast Ethernet1/0 (A4)
- IPv4 Address : 10.76.19.81
- Subnet Mask : 255.255.255.252

Fast Ethernet1/1 (A6)
- IPv4 Address : 10.76.19.85
- Subnet Mask : 255.255.255.252
```
Static Routes
```
(Default to Hololive)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.73

(A3)
- Network : 10.76.8.0
- Mask : 255.255.252.0
- Next Hop : 10.76.19.77

(A5)
- Network : 10.76.18.128
- Mask : 255.255.255.192
- Next Hop : 10.76.19.82

(A7)
- Network : 10.76.12.0
- Mask : 255.255.254.0
- Next Hop : 10.76.19.86
```
### Holo-JP
Interfaces
```
Fast Ethernet0/0 (A8)
- IPv4 Address : 10.76.19.90
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A9)
- IPv4 Address : 10.76.19.49
- Subnet Mask : 255.255.255.248
```
Static Routes
```
(Default to Hololive)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.89

(A10)
- Network : 10.76.19.32
- Mask : 255.255.255.240
- Next Hop : 10.76.19.50

(A11)
- Network : 10.76.0.0
- Mask : 255.255.248.0
- Next Hop : 10.76.19.51

(A12)
- Network : 10.76.14.0
- Mask : 255.255.254.0
- Next Hop : 10.76.19.51

(A13)
- Network : 10.76.19.92
- Mask : 255.255.255.252
- Next Hop : 10.76.19.51

(A14)
- Network : 10.76.18.0
- Mask : 255.255.255.128
- Next Hop : 10.76.19.51
```
### Holo-EN (Router)
Interfaces
```
Fast Ethernet0/0 (A15)
- IPv4 Address : 10.76.19.98
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A16)
- IPv4 Address : 10.76.19.101
- Subnet Mask : 255.255.255.252

Fast Ethernet1/0 (A21)
- IPv4 Address : 10.76.19.105
- Subnet Mask : 255.255.255.252
```
Static Routes
```
(Default to Hololive)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.97

(A17)
- Network : 10.76.16.0
- Mask : 255.255.254.0
- Next Hop : 10.76.19.102

(A18)
- Network : 10.76.19.56
- Mask : 255.255.255.248
- Next Hop : 10.76.19.102

(A20)
- Network : 10.76.18.192
- Mask : 255.255.255.192
- Next Hop : 10.76.19.102

(A22)
- Network : 10.76.19.0
- Mask : 255.255.255.224
- Next Hop : 10.76.19.106
```
### AREA15
Interfaces
```
Fast Ethernet0/0 (A2)
- IPv4 Address : 10.76.19.77
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A3)
- IPv4 Address : 10.76.8.1
- Subnet Mask : 255.255.252.0
```
Static Routes
```
(Default to Holo-ID)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.77
```
### Risu (Laptop)
```
Fast Ethernet0/0 (A3)
- IPv4 Address : 10.76.8.2
- Subnet Mask : 255.255.252.0
- Default Gateway : 10.76.8.1
```
### Moona (Laptop)
```
Fast Ethernet0/0 (A3)
- IPv4 Address : 10.76.8.3
- Subnet Mask : 255.255.252.0
- Default Gateway : 10.76.8.1
```
### lofi (Laptop)
```
Fast Ethernet0/0 (A3)
- IPv4 Address : 10.76.8.4
- Subnet Mask : 255.255.252.0
- Default Gateway : 10.76.8.1
```
### holoro (Router)
Interfaces
```
Fast Ethernet0/0 (A4)
- IPv4 Address : 10.76.19.82
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A5)
- IPv4 Address : 10.76.18.129
- Subnet Mask : 255.255.255.192
```
Static Routes
```
(Default to Holo-ID)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.81
```
### Ollie (Laptop)
```
Fast Ethernet0/0 (A5)
- IPv4 Address : 10.76.18.130
- Subnet Mask : 255.255.255.192
- Default Gateway : 10.76.18.129
```
### Anya (Server)
```
Fast Ethernet0/0 (A5)
- IPv4 Address : 10.76.18.131
- Subnet Mask : 255.255.255.192
- Default Gateway : 10.76.18.129
```
### Reine (PC)
```
Fast Ethernet0/0 (A5)
- IPv4 Address : 10.76.18.132
- Subnet Mask : 255.255.255.192
- Default Gateway : 10.76.18.129
```
### holoh3ro (Router)
Interfaces
```
Fast Ethernet0/0 (A6)
- IPv4 Address : 10.76.19.86
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A7)
- IPv4 Address : 10.76.12.1
- Subnet Mask : 255.255.254.0
```
Static Routes
```
(Default to Holo-ID)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.85
```
### Zeta (Laptop)
```
Fast Ethernet0/0 (A7)
- IPv4 Address : 10.76.12.2
- Subnet Mask : 255.255.255.192
- Default Gateway : 10.76.12.1
```
### Kaela (Server)
```
Fast Ethernet0/0 (A7)
- IPv4 Address : 10.76.12.3
- Subnet Mask : 255.255.255.192
- Default Gateway : 10.76.12.1
```
### Kobo (Laptop)
```
Fast Ethernet0/0 (A7)
- IPv4 Address : 10.76.12.4
- Subnet Mask : 255.255.255.192
- Default Gateway : 10.76.12.1
```
### DEV_IS (Router)
Interfaces
```
Fast Ethernet0/0 (A9)
- IPv4 Address : 10.76.19.50
- Subnet Mask : 255.255.255.248

Fast Ethernet0/1 (A10)
- IPv4 Address : 10.76.19.33
- Subnet Mask : 255.255.255.240
```
Static Routes
```
(Default to Holo-JP)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.49
```
### Ririka_Raden (Laptop)
```
Fast Ethernet0/0 (A10)
- IPv4 Address : 10.76.19.34
- Subnet Mask : 255.255.255.240
- Default Gateway : 10.76.19.33
```
### Ao (PC)
```
Fast Ethernet0/0 (A10)
- IPv4 Address : 10.76.19.35
- Subnet Mask : 255.255.255.240
- Default Gateway : 10.76.19.33
```
### Hajime_Kanade (Laptop)
```
Fast Ethernet0/0 (A10)
- IPv4 Address : 10.76.19.36
- Subnet Mask : 255.255.255.240
- Default Gateway : 10.76.19.33
```
### GEN: 0 (Router)
Interfaces
```
Fast Ethernet0/0 (A9)
- IPv4 Address : 10.76.19.51
- Subnet Mask : 255.255.255.248

Fast Ethernet0/1 (A11)
- IPv4 Address : 10.76.0.1
- Subnet Mask : 255.255.248.0
```
Static Routes
```
(Default to Holo-JP)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.49

(A12)
- Network : 10.76.14.0
- Mask : 255.255.254.0
- Next Hop : 10.76.0.4

 (A13)
- Network : 10.76.19.92
- Mask : 255.255.255.252
- Next Hop : 10.76.0.4

 (A14)
- Network : 10.76.18.0
- Mask : 255.255.255.128
- Next Hop : 10.76.0.4
```
### MiComet (PC)
```
Fast Ethernet0/0 (A11)
- IPv4 Address : 10.76.0.2
- Subnet Mask : 255.255.255.240
- Default Gateway : 10.76.0.1
```
### Sora_Robo_AZKi (PC)
```
Fast Ethernet0/0 (A11)
- IPv4 Address : 10.76.0.3
- Subnet Mask : 255.255.255.240
- Default Gateway : 10.76.0.1
```
### GEN: 1 (Router)
Interfaces
```
Fast Ethernet0/0 (A11)
- IPv4 Address : 10.76.0.4
- Subnet Mask : 255.255.248.0

Fast Ethernet0/1 (A12)
- IPv4 Address : 10.76.14.1
- Subnet Mask : 255.255.254.0

Fast Ethernet1/0 (A13)
- IPv4 Address : 10.76.19.93
- Subnet Mask : 255.255.255.252
```
Static Routes
```
(Default to GEN: 0)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.0.1

(A14)
- Network : 10.76.18.0
- Mask : 255.255.255.128
- Next Hop :10.76.19.94 
```
### FBK_Matsuri (Server)
```
Fast Ethernet0/0 (A12)
- IPv4 Address : 10.76.14.2
- Subnet Mask : 255.255.254.0
- Default Gateway : 10.76.14.1
```
### Aki_Hachama (Laptop)
```
Fast Ethernet0/0 (A12)
- IPv4 Address : 10.76.14.3
- Subnet Mask : 255.255.254.0
- Default Gateway : 10.76.14.1
```
### GAMERS (Router)
Interfaces
```
Fast Ethernet0/0 (A13)
- IPv4 Address : 10.76.19.94
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A14)
- IPv4 Address : 10.76.18.1
- Subnet Mask : 255.255.255.128
```
Static Routes
```
Default to GEN: 1)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.93
```
### Korone (Server)
```
Fast Ethernet0/0 (A14)
- IPv4 Address : 10.76.18.2
- Subnet Mask : 255.255.255.128
- Default Gateway : 10.76.18.1
```
### Okayu (Laptop)
```
Fast Ethernet0/0 (A14)
- IPv4 Address : 10.76.18.3
- Subnet Mask : 255.255.255.128
- Default Gateway : 10.76.18.1
```
### Mio (Server)
```
Fast Ethernet0/0 (A14)
- IPv4 Address : 10.76.18.4
- Subnet Mask : 255.255.255.128
- Default Gateway : 10.76.18.1
```
### Holo-Myth (Router)
Interfaces
```
Fast Ethernet0/0 (A16)
- IPv4 Address : 10.76.19.102
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A17)
- IPv4 Address : 10.76.16.1
- Subnet Mask : 255.255.254.0

Fast Ethernet1/0 (A19)
- IPv4 Address : 10.76.19.65
- Subnet Mask : 255.255.255.248
```
Static Routes
```
(Default to Holo-EN)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop : 10.76.19.101

(A18)
- Network : 10.76.19.56
- Mask : 255.255.255.248
- Next Hop : 10.76.19.66

(A20)
- Network : 10.76.18.192
- Mask : 255.255.255.192
- Next Hop : 10.76.19.67
```
### Gura_Ame_Ina (Laptop)
```
Fast Ethernet0/0 (A17)
- IPv4 Address : 10.76.16.2
- Subnet Mask : 255.255.254.0
- Default Gateway : 10.76.16.1
```
### Kiara_Calli (PC)
```
Fast Ethernet0/0 (A17)
- IPv4 Address : 10.76.16.3
- Subnet Mask : 255.255.254.0
- Default Gateway : 10.76.16.1
```
### Router4 (Router)
Interfaces
```
Fast Ethernet0/1 (A18)
- IPv4 Address : 10.76.19.57
- Subnet Mask : 255.255.255.248

Fast Ethernet0/0 (A19)
- IPv4 Address : 10.76.19.66
- Subnet Mask : 255.255.255.248
```
Static Routes
```
(Default to Holo-Myth)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop :  10.76.19.65

(A20)
- Network : 10.76.18.192
- Mask : 255.255.255.192
- Next Hop :10.76.19.67
```
### Irys (Server)
```
Fast Ethernet0/0 (A18)
- IPv4 Address : 10.76.19.58
- Subnet Mask : 255.255.255.248
- Default Gateway : 10.76.19.57
```
### Holo-Council (Router)
Interfaces
```
Fast Ethernet0/0 (A19)
- IPv4 Address : 10.76.19.67
- Subnet Mask : 255.255.255.248
Fast Ethernet0/1 (A20)
- IPv4 Address : 10.76.18.193
- Subnet Mask : 255.255.255.192
```
Static Routes
```
(Default to Holo-Myth)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop :  10.76.19.65
```
### Kronii_Mumei (Laptop)
```
Fast Ethernet0/0 (A20)
- IPv4 Address : 10.76.18.194
- Subnet Mask : 255.255.255.192
- Default Gateway : 10.76.18.193
```
### Bae_fauna (Server)
```
Fast Ethernet0/0 (A20)
- IPv4 Address : 10.76.18.195
- Subnet Mask : 255.255.255.192
- Default Gateway : 10.76.18.193
```
### HoloAdvent (Router)
Interfaces
```
Fast Ethernet1/0 (A21)
- IPv4 Address : 10.76.19.106
- Subnet Mask : 255.255.255.252

Fast Ethernet1/0 (A22)
- IPv4 Address : 10.76.19.1
- Subnet Mask : 255.255.255.224
```
Static Routes
```
(Default to Holo-EN)
- Network : 0.0.0.0
- Mask : 0.0.0.0
- Next Hop :  10.76.19.105
```
### FuwaMoco (Laptop)
```
Fast Ethernet0/0 (A22)
- IPv4 Address : 10.76.19.2
- Subnet Mask : 255.255.255.224
- Default Gateway : 10.76.19.1
```
### Shiori_nerissa (PC)
```
Fast Ethernet0/0 (A22)
- IPv4 Address : 10.76.19.3
- Subnet Mask : 255.255.255.224
- Default Gateway : 10.76.19.1
```
### Biboo (server)
```
Fast Ethernet0/0 (A22)
- IPv4 Address : 10.76.19.4
- Subnet Mask : 255.255.255.224
- Default Gateway : 10.76.19.1
```

## Testing
Kronii_Mumei ke Anya 

<img width="700" alt="Screenshot 2024-11-16 at 12 32 38" src="https://github.com/user-attachments/assets/d2ec0458-b66a-439d-88ca-70b84c447aab">

Gura_Ame_Ina ke Mio 

<img width="694" alt="Screenshot 2024-11-16 at 12 33 25" src="https://github.com/user-attachments/assets/1438e72b-1e5b-48fc-b680-0a3233c4c624">

Aki_Hachama ke Kaela 

<img width="700" alt="Screenshot 2024-11-16 at 12 34 21" src="https://github.com/user-attachments/assets/df344318-53d7-4dff-8745-6d8c746075ce">

# GNS3 (CIDR)
## Topologi
![image](https://github.com/user-attachments/assets/66dd358f-1a88-4676-8ead-390ce1ece390)

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
![image](https://github.com/user-attachments/assets/0dbc50b1-6f16-4e38-b4ec-cfa8c8c82dab)

## Tree
![TREE_JARKOM_FKRI](https://github.com/user-attachments/assets/1642665d-ac09-4558-b39e-c50914c8a04e)

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
    address 10.77.4.5
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
    address 10.77.4.6
    netmask 255.255.255.252

#A2
auto eth1
iface eth1 inet static
    address 10.77.4.1
    netmask 255.255.255.252

#A4
auto eth2
iface eth2 inet static
    address 10.77.16.65
    netmask 255.255.255.252

#A6
auto eth3
iface eth3 inet static
    address 10.77.34.1
    netmask 255.255.255.252
```

### AREA15 (Gateway)
```
#A2
auto eth0
iface eth0 inet static
    address 10.77.4.2
    netmask 255.255.255.252
    gateway 10.76.4.1

#A3
auto eth1
iface eth1 inet static
    address 10.77.0.1
    netmask 255.255.252.0
```

### lofi (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 10.77.0.2
    netmask 255.255.252.0
    gateway 10.77.0.1
```

### Moona (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 10.77.0.3
    netmask 255.255.252.0
    gateway 10.77.0.1
```

### Risu (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 10.77.0.4
    netmask 255.255.252.0
    gateway 10.77.0.1
```

### holoro (Gateway)
```
#A4
auto eth0
iface eth0 inet static
    address 10.77.16.66
    netmask 255.255.255.252
    gateway 10.77.16.65

#A5
auto eth1
iface eth1 inet static
    address 10.77.16.1
    netmask 255.255.252.192
```

### Ollie (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 10.77.16.2
    netmask 255.255.252.192
    gateway 10.77.16.1
```

### Anya (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 10.77.16.3
    netmask 255.255.252.192
    gateway 10.77.16.1
```

### Reine (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 10.77.16.4
    netmask 255.255.252.192
    gateway 10.77.16.1
```

### holoh3ro (Gateway)
```
#A6
auto eth0
iface eth0 inet static
    address 10.77.34.2
    netmask 255.255.255.252
    gateway 10.77.34.1

#A7
auto eth1
iface eth1 inet static
    address 10.77.32.1
    netmask 255.255.254.0
```

### Zeta (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 10.77.32.2
    netmask 255.255.254.0
    gateway 10.77.32.1
```

### Kaela (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 10.77.32.3
    netmask 255.255.254.0
    gateway 10.77.32.1
```

### Kobo (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 10.77.32.4
    netmask 255.255.254.0
    gateway 10.77.32.1
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
    gateway 10.76.10.1

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
    gateway 10.76.10.9
```

### Ao (Client)
```
#A10
auto eth0
iface eth0 inet static
    address 10.76.10.11
    netmask 255.255.255.240
    gateway 10.76.10.9
```

### Hajime_Kanade (Client)
```
#A10
auto eth0
iface eth0 inet static
    address 10.76.10.12
    netmask 255.255.255.240
    gateway 10.76.10.9
```

### GEN:0 (Gateway)
```
#A9
auto eth0
iface eth0 inet static
    address 10.76.10.3
    netmask 255.255.255.252
    gateway 10.76.10.1

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
