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


> adb shell settings put secure enabled_accessibility_services <com.package.name/com.package.name.ServiceName>
```bash
adb shell settings put secure enabled_accessibility_services <com.package.name/com.package.name.ServiceName>
```
>
<br>


> termux-adb shell settings put secure enabled_accessibility_services bitpit.launcher/bitpit.launcher.lock_screen.LockScreenService
```bash
termux-adb shell settings put secure enabled_accessibility_services bitpit.launcher/bitpit.launcher.lock_screen.LockScreenService
```
>
<br>



