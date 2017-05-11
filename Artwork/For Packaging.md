#Apa yang perlu di ganti : 

##Window Manager :
* Font: `URW Gothic L Demi 10`
* theme: Working-Theme (atau boleh di rename)
* title alignment: center

##Appearance: 
* font: URW Gothic L book 10
* Tema:
   * Light : 
	* Theme = Working-Theme (sama dengan window manager)
	* icon  = paper
   * Dark :
        * Theme = Working-Theme-Dark
        * icon = paper2
* LightDM GTK Greeter :
  * Theme: Working-Theme-Greet
  * Icons: Paper
  * Font: URW Gothic L Demi 11
  * Background: wallpaper utama

#Plymouth New : 
/Artwork/plymouth/

cek tealinuxos.plymouth
pastikan image dir sama script file mengarah ke folder & file yang sesuai

file konfigurasi:
```[Plymouth Theme]
Name=tealinuxos
Description=tealinuxos plymouth 
ModuleName=script
```

```[script]
ImageDir=/lib/plymouth/themes/tealinuxos
ScriptFile=/lib/plymouth/themes/tealinuxos/tealinuxos.script
```

jalankan:
```sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/newtealinuxos/newtealinuxos.plymouth 300
sudo update-alternatives --config * pilih yang tadi baru di install default.plymouth                                                                                                                 
sudo update-initramfs -u 
```

Ubiquity Slideshow :
masukkan di tempatnya

Background bootloader:

Logo tealinuxos di ubiquity (pas milih try / install):
seperti tahun lalu

logo install tealinuxos di desktop:
seperti tahun lalu

wallpaper default:
Artwork/bg/bg wp web ver.png

wallpaper lain:
Artwork/bg/\*.png
