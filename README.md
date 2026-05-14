# eucalypsih_rcrapsbash_adb

> sample
```bash
>
```bash

` ```
>
<br>

```
>
<br>


> termux-adb shell pm list packages | grep gms
```bash
termux-adb shell pm list packages | grep gms
```
>
<br>


> termux-adb shell am force-stop com.google.android.gms
```bash
termux-adb shell am force-stop com.google.android.gms
```
>
<br>


> termux-adb shell pm disable-user --user 0 com.google.android.gms
```bash
termux-adb shell pm disable-user --user 0 com.google.android.gms
```
> Menonaktifkan Aplikasi (Disable). Jika ingin menghentikan dan mencegah aplikasi berjalan kembali (lebih kuat dari force stop)
<br>


> termux-adb shell am start -S <NAMA_PAKET>
```bash
termux-adb shell am start -S <NAMA_PAKET>
```
> Membuka Aplikasi sambil Memaksa Berhenti (Reset) Pertama. Perintah ini menutup aplikasi terlebih dahulu, lalu membukanya kembali.
<br>


> termux-adb shell dumpsys accessibility
```bash
termux-adb shell dumpsys accessibility
```
>
<br>


> termux-adb shell dumpsys deviceidle whitelist +bitpit.launcher
```bash
termux-adb shell dumpsys deviceidle whitelist +bitpit.launcher
```
> Masukkan ke Daftar Putih Manajemen Daya (Battery Optimization Whitelist). Perintah ini mengecualikan Smart Launcher dari optimasi baterai bawaan Android, sehingga sistem tidak mudah menghentikannya.
<br>


> termux-adb shell cmd appops set bitpit.launcher RUN_IN_BACKGROUND allow

```bash
termux-adb shell cmd appops set bitpit.launcher RUN_IN_BACKGROUND allow
```
> Kunci Proses Menggunakan AppOps (Jika Didukung Firmware). Beberapa ponsel UNISOC mengizinkan pengaturan mode operasi aplikasi secara paksa.
<br>


> termux-adb shell settings get secure enabled_accessibility_services
```bash
termux-adb shell settings get secure enabled_accessibility_services
```
> Memastikan Layanan Aktif. Periksa apakah layanan sudah aktif
<br>


> adb shell settings put secure enabled_accessibility_services <com.package.name/com.package.name.ServiceName>
```bash
adb shell settings put secure enabled_accessibility_services <com.package.name/com.package.name.ServiceName>
```
>
<br>


> termux-adb shell settings put secure enabled_accessibility_services bitpit.launcher/bitpit.launcher.lock_screen.LockScreenService:com.quickcursor/com.quickcursor.android.services.CursorAccessibilityService
```bash
termux-adb shell settings put secure enabled_accessibility_services bitpit.launcher/bitpit.launcher.lock_screen.LockScreenService:com.quickcursor/com.quickcursor.android.services.CursorAccessibilityService
```
>
<br>


> adb shell pidof com.example.app
```bash
adb shell pidof com.example.app
```
> Memfilter Berdasarkan PID (Lebih Akurat). Cara ini paling akurat karena hanya menampilkan log yang dihasilkan oleh aplikasi Anda (bukan sekadar baris log yang mengandung nama package).
<br>


> termux-adb logcat --pid=<PID_DARI_LANGKAH_1>
```bash
termux-adb logcat --pid=<PID_DARI_LANGKAH_1>
```
>
<br>


> termux-adb uninstall -k <nama.package.aplikasi>
```bash
termux-adb uninstall -k <nama.package.aplikasi>
```
> Menghapus Aplikasi Tanpa Menghapus Data (Keep Data)
<br>


> termux-adb shell pm clear <nama.package.aplikasi>
```bash
termux-adb shell pm clear <nama.package.aplikasi>
```
> Menghapus Data & Cache Aplikasi (Clear Data)
<br>


> adb shell dumpsys window displays | grep -E "mCurrentFocus"
```bash
adb shell dumpsys window displays | grep -E "mCurrentFocus"
```
> Menemukan Nama Package. Jika Anda tidak tahu nama lengkap paket aplikasi (misal: com.android.chrome), gunakan perintah ini saat aplikasi terbuka di HP untuk mengetahuinya.
<br>


> termux-adb shell dumpsys activity <package>/<activity> (informasi aktivitas) # https://gist.github.com/Pulimet/5013acf2cd5b28e55036c82c91bd56d8
```bash
termux-adb shell dumpsys activity <package>/<activity> (informasi aktivitas) # https://gist.github.com/Pulimet/5013acf2cd5b28e55036c82c91bd56d8
```

> adb shell pm list permissions -d -f -g <nama_package>
```bash
adb shell pm list permissions -d -f -g <nama_package>
```
> List Izin Berdasarkan Package
<br>


# package
> com.rarlab.rar/com.rarlab.rar.MainActivity
```bash
com.rarlab.rar/com.rarlab.rar.MainActivity
```

> com.android.vending
> com.google.android.gms
> com.whatsapp android.permission.RECORD_AUDIO

> sprd.permission.PROTECT_PROCESS
> android.permission.RECORD_AUDIO
<br>


# source
> https://gist.github.com/Pulimet/5013acf2cd5b28e55036c82c91bd56d8
```bash
https://gist.github.com/Pulimet/5013acf2cd5b28e55036c82c91bd56d8
```
<br>


> [Cara Membuat Flashable ZIP di Android | PDF](https://id.scribd.com/document/367457577/Materi)
```bash
[Cara Membuat Flashable ZIP di Android | PDF](https://id.scribd.com/document/367457577/Materi)
```
<br>


> [Deodex Tools Classy Kitchen Download | OPREK MANIA](https://oprekmania.com/deodex-tools-classy-kitchen-download/)
```bash
[Deodex Tools Classy Kitchen Download | OPREK MANIA](https://oprekmania.com/deodex-tools-classy-kitchen-download/)
```
<br>


> [Get your Unrevoked Keybox XML File Here | Pass Strong Integrity - DroidWin](https://droidwin.com/get-your-unrevoked-keybox-xml-file-here-pass-strong-integrity/#google_vignette)
```bash
[Get your Unrevoked Keybox XML File Here | Pass Strong Integrity - DroidWin](https://droidwin.com/get-your-unrevoked-keybox-xml-file-here-pass-strong-integrity/#google_vignette)
```
>
<br>


> [CherishOS - Cherish Every Bit of Your Android](https://www.cherishos.com/keybox)
```bash
[CherishOS - Cherish Every Bit of Your Android](https://www.cherishos.com/keybox)
```
>
<br>


>[AxionOs - Keybox Updater](https://www.axionos.org/keybox.html)
```bash
[AxionOs - Keybox Updater](https://www.axionos.org/keybox.html)
```
>
<br>


