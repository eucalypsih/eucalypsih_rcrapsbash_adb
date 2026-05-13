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
