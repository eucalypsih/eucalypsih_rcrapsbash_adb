# eucalypsih_rcrapsbash_adb

>
```bash

```
>
<br>


> termux-adb shell am force-stop com.whatsapp
```bash
termux-adb shell am force-stop com.whatsapp
```
>
<br>


> termux-adb shell pm disable-user --user 0 com.whatsapp
```bash
termux-adb shell pm disable-user --user 0 com.whatsapp
```
> Menonaktifkan Aplikasi (Disable). Jika ingin menghentikan dan mencegah aplikasi berjalan kembali (lebih kuat dari force stop)
<br>


> termux-adb shell am start -S <NAMA_PAKET>
```bash
termux-adb shell am start -S <NAMA_PAKET>
```
> Membuka Aplikasi sambil Memaksa Berhenti (Reset) Pertama. Perintah ini menutup aplikasi terlebih dahulu, lalu membukanya kembali.
<br>
