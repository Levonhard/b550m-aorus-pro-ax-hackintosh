# B550m Aorus Pro AX Hackintosh
Opencore EFI for B550M Aorus Pro AX
<img src="https://github.com/Levonhard/b550m-aorus-pro-ax-hackintosh/blob/main/screenshot-monterey.png">

## MY PC SPECS

| COMPONENTS | MODEL                                 |
|------------|---------------------------------------|
| CPU        | AMD Ryzen 5 5600X.                    |
| RAM        | 16 GiB@3600MHz DDR4                   |
| GPU        | PowerColor Red Devil RX 6600 XT       |
| WiFi       | Intel® Wi-Fi 6 AX200                  |
| Storage    | SSD 256 GiB + HDD 320 GiB             |

### WORKS
- [x] DRM
- [x] USB
- [x] AMD GPU
- [x] Intel WiFi and Bluetooth
- [x] Internal Speakers
- [x] Apple Services (iCloud, Apple Music, Apple TV, others..)
- [x] Sleep Mode
- [x] Fan Control
- [ ] Mic

### NOT TESTED
- Airdrop

## GUIDE
### BIOS SETUP
```diff
- disable "Trusted Computing"
- disable "wake" and "boot over LAN"
- disable "CSM Support"
+ enable "Power Loading" in "Platform Power settings"
+ enable "X.M.P." memory profile
+ enable "Above 4G Decoding"
+ enable "Re-Size BAR Support"
! if applicable, set PCIe x16 slot to Gen4 instead of Auto (may contribute to a better stability)
```

### OPENCORE EFI SETUP
- Generate your own SMBIOS
