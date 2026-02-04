<img align="center" src="banner.webp" width="425" alt="banner">

# Dualboot Android & Windows di POCO X3 Pro
[![Telegram](https://img.shields.io/badge/Chat-Telegram-brightgreen.svg?logo=telegram&style=flat-square)](https://t.me/kuatodevprojects)

## ⚠️ PERINGATAN!!!
Kita ga nanggung kalo HP lo brick, partisi recovery ilang, teknisi xiaomi ~bunuh diri~ kebingungan, microSD tewas, IC power/RAM/Layar/CPU angus, kelakuan aneh Xiaomi/Poco, kucing/anjing lo mati, perang nuklir, atau lo dipecat gara-gara lupa boot balik ke Android pas alarm bunyi.

Semua file di sini kontribusi dari user lain, di sini lo bakal nemu panduan pake file yang berhasil kita kumpulin. Proses ini sensitif banget, resiko tanggung sendiri (DWYOR) dan ikutin langkahnya bener-bener.

**KALO LO GA NYAMAN OPREK HP ATAU PARTISI TABELNYA, ATAU LO PARNO HP LO BAKAL BRICK, MENDING CABUT SEKARANG!!! LO UDAH DIPERINGATIN YAA, KALO HP LO BRICK LO URUS SENDIRI!!! SEKALI LAGI! SAYA UDAH PERINGATIN YA!!!**

## Install Windows tanpa PC

### Prasyarat
- POCO X3 PRO yang sudah unlock bootloader, terpasang Custom Recovery (TWRP/PBRP/OrangeFox) dan sudah root (Magisk/KSU/Etc.)

- [Modified TWRP](https://github.com/n00b69/woa-vayu/releases/tag/Recovery)

### Catatan
> [!WARNING]  
> Semua data lu akan terhapus! BACKUP sekarang!.
>
> JANGAN REBOOT HP LU kalo lu ngerasa bikin kesalahan, minta tolong di [Telegram](https://t.me/kuatodevprojects).
### Instal TWRP yang sudah dimodifikasi.
> Ganti custom recovery lu dengan modified TWRP yang sudah lu download 

#### Membuka terminal TWRP
- Setelah berhasil masuk ke TWRP, decrypt data dengan memasukkan kata sandi lu jika diminta.
- Tekan tombol **Advance** di bagian kiri bawah layar, lalu tekan **Terminal**.

### Jalankan skrip partisi
- Ganti **$** dengan jumlah penyimpanan yang lu inginkan untuk Windows (jangan tambahkan GB, cukup tulis angkanya). 

> - Device dengan 128GB variant, partisi minimal untuk Windows 32GB hingga 64GB. 

> - Device dengan 256GB Variant, partisi minimal untuk Windows 32GB hingga 192GB.

```cmd
partition $
```
> [!TIPS] kalo muncul error, coba ketik ulang command nya. 

### Cek apakah Android masih bisa booting
- Coba restart HP lu, dan lihat apakah Android masih bisa booting normal. 
Kalo normal, restore backup atau setup hp lu kaya abis clean flash biasa dan jangan lupa lu root!

### Menyiapkan berkas-berkas yang diperlukan
- [DOWNLOAD](https://arkt-7.github.io/woawin/) file **Windows versi 25H2 26200.6899** dan pastikan tetap berada di folder `Download` **penyimpanan internal lu**, BUKAN di SDCard.
- [DOWNLOAD](https://github.com/KuatoDev/Vayu-WinInstaller/releases/download/v1.0/Vayu.WinInstaller.zip) **Vayu WinInstaller** dan simpan di penyimpanan internal lu.
- [DOWNLOAD](https://xmfirmwareupdater.com/firmware/vayu/) **vayu firmware.zip** dan simpan di penyimpanan internal lu.
- [DOWNLOAD](https://github.com/WaLoVayu/POCOX3Pro-Windows-Releases/releases/download/2502.28/POCO.X3.Pro.UEFI-v2502.28.img) **UEFI** paling up to date buat Poco X3 Pro dan taroh di penyimpanan internal lu.
- Download dan instal [WIN Cross](https://www.pling.com/p/1969499/), lalu buka dan kasih akses root. Setelah itu select UEFI yang udah di download. Lalu buka settings app, matikan force backup kernel on boot dan force backup kernel if missing.
tahap paling penting nih! **BACKUP BOOT.IMG lo make WINCross sekarang!**
- Reboot ke TWRP yang telah dimodifikasi. 

### Install Vayu WinInstaller
- Di TWRP, pilih **Install** lalu cari **vayu firmware.zip** dan lakukan flashing.
- Setelah firmware berhasil diinstal, jangan lakukan reboot. Sebaliknya, instal juga **Vayu WinInstaller.zip**.
- Tunggu hingga semua proses selesai dan perangkat lu melakukan booting ke Windows. Ini akan memakan waktu sekitar 15-20 menit.
Setelah booting ke Windows, lu setup dah tuh Windows mau lu pake apa. Kalo udah selesai, booting ke android dengan klik STA di desktop lu.
> [! TIPS] Kalo STA ga muncul di desktop lu, jangan panik. Cukup lu restart (BUKAN SHUTDOWN YA!) sambil pencet volume atas supaya booting ke TWRP. 
Lalu lu flash Boot.img yang tadi udah lu backup di folder WINCross/Backup/boot.img dan flash ke boot. lalu restart HP lu. setelah booting ke Android, buka WINCross, Mount Windows, terus buka Toolbox, cari Create STA dan klik sampe proses selesai.

#### Cara booting ke Windows
- Buka WINCross, Tekan **Switch to Windows** di dalam aplikasi atau *pasang widget Switch To Windows di homscreen* lu.
#### Cara booting ke Android
- Jalankan shortcut **STA** di desktop lu.

## Selesai!