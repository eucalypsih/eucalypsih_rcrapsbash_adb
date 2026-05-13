# eucalypsih_rcrapsbash_adb

>
```bash

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


>termux-adb shell settings get secure enabled_accessibility_services
```bash
termux-adb shell settings get secure enabled_accessibility_services
```
>
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

