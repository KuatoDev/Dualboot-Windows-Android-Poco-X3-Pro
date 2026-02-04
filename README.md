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



## Maintainers
[<img alt="Project Aloha" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/118143494?s=200&v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/Project-Aloha)
[<img alt="remtrik" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/69907487?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/remtrik)
[<img alt="degdag" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/22778181?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/degdag)


## Contributors
[<img alt="adomerlee" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/109386069?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/adomerlee)
[<img alt="Morc" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/13377926?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/TheMorc)
[<img alt="map220v" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/14368485?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/map220v)
[<img alt="halal-beef" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/78730004?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/halal-beef)
[<img alt="Renegade Project" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/63859504?s=200&v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/edk2-porting)
[<img alt="gus33000" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/3755345?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/gus33000)
[<img alt="Renegade Project Discord Members" src="https://images.weserv.nl/?url=https://cdn.discordapp.com/icons/736563593058713690/68f67bfddf4390b11effc99917b16338.webp?size=256&w=45&fit=cover&mask=circle&maxage=7d" />](https://discord.gg/XXBWfag)
[<img alt="ArturoGC06" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/76574534?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/ArturoGC06)
[<img alt="SebastianZSXS" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/111822607?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/SebastianZSXS)
[<img alt="MollySophia" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/20746884?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/MollySophia)
[<img alt="haouarihk" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/57036855?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/haouarihk)
[<img alt="bibarub" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/73599925?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/bibarub)
[<img alt="Ilya114" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/93242944?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/Ilya114)
[<img alt="proganime1200" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/32473502?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/proganime1200)
[<img alt="KuatoDev" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/17999613?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/KuatoDev)
[<img alt="belomaxorka" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/54049465?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/belomaxorka)
[<img alt="Nx0Ri" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/152011726?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/Nx0Ri)
[<img alt="Misha803" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/118528504?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/Misha803)
[<img alt="n00b69" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/83274506?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/n00b69)
[<img alt="TrustedFloppa" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/85476585?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/TrustedFloppa)
[<img alt="Dawid2849" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/77780707?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/Dawid2849)
[<img alt="Kumar-Jy" src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/20044626?v=4&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/Kumar-Jy)
[<img alt="yusufyorunc" src="https://images.weserv.nl/?url=https://github.com/yusufyorunc.png&w=45&fit=cover&mask=circle&maxage=7d" />](https://github.com/yusufyorunc)
