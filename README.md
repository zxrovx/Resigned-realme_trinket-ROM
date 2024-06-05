
## README.md

### Instructions in English and Indonesian

#### English

1. **Ensure UKA is Installed**
2. **Create a Folder on /sdcard (Name it anything you like)**
3. **Extract the system.img and vendor.img files into the newly created folder**
4. **Open Terminal Emulator (Termux) and run UKA with the command `su -c menu` (Ensure Termux has root access)**
5. **Type `3` (Menu: Unpacking .img) to start unpacking .img, then choose `7` to specify the location of the image file**
6. **When prompted to provide the location of the image file, type `cd /sdcard/yourfoldername`. UKA will automatically read the filesystem images there**
7. **Select the file you want to unpack, such as system or vendor, or choose unpack all to unpack all image files in that directory**
8. **Once unpacking is complete, open MT Manager (Ensure MT Manager has root access)**
9. **Go to the Root tab and navigate to `/data/local/UnpackerSystem`**
10. **If you have specified the directories for system, vendor, and config, go to the config section for system or vendor and delete the avb.img file**
11. **If you want to modify the system/vendor, you can do so in the "UnpackerSystem" directory**
12. **Now we will repack it into .br**
13. **Return to UKA and choose menu `9` (Menu: Build and convert to .br)**
14. **Select number `2` (Build .img with size input -> .br), this will repack into .br based on the input size we provide**
15. **If you want to save the compressed file to /sdcard, type `cd /sdcard/yourfoldername`, otherwise just press enter, the compressed file will be in `/data/local/UnpackerSystem`**
16. **Choose the file you want to compress (e.g., system). If prompted to input size:**
    - **Open MT, go to the UnpackerSystem/config directory, find the system_size.txt file, open and copy its contents, then return to Termux and paste it, then press enter**
    - **If there's a selection for Android version, choose number `4`**
    - **If you want to compress with high compression, select `7`, or for standard compression, choose `5` or `6`. High compression (`7`) is recommended for smaller final size, but it may take longer, so you can wait while watching YouTube or doing other activities**

17. **After everything is complete, move all files from `/data/local/UnpackerSystem` to the folder you desire**
18. **Then create a flashable zip with META-INF or other necessary files following the proper structure. When zipping files with MT Manager, it is recommended to select the Fastest compression level**
19. **Once everything is done, clean up the UKA directory by returning to Termux UKA, select `12` then `8`**
20. **After completion, you can exit and test flash the ROM in recovery**

**Make sure your system and vendor are resized, as failing to resize may result in the system/vendor becoming R/O or mismatched sizes causing Gapps installation failures.**

#### Indonesian

1. **Pastikan UKA Sudah Terinstall**
2. **Buat Folder Di /sdcard (beri nama apa saja, bebas)**
3. **Ekstrak file system.img dan vendor.img ke dalam folder yang baru saja Anda buat**
4. **Buka Terminal Emulator (Termux) dan jalankan UKA dengan perintah `su -c menu` (Pastikan Termux diberi akses root)**
5. **Ketik `3` (Menu: Unpacking .img) untuk memulai unpack .img, dan pilih `7` untuk menentukan lokasi image file**
6. **Setelah ada perintah memberikan lokasi image file, ketik `cd /sdcard/namafolderanda`. Maka otomatis UKA akan membaca filesystem image yang ada di sana**
7. **Pilih file yang ingin Anda unpack, misalkan system atau vendor, atau unpack all untuk melakukan unpack seluruh file image yang ada di direktori itu**
8. **Setelah selesai unpacking, buka MT Manager (Pastikan MT Manager diberi akses root)**
9. **Ke tab Root, masuk ke `/data/local/UnpackerSystem`**
10. **Kalau Anda sudah menentukan direktori system, vendor, dan config, masuk pada bagian config ke system atau vendor, hapus file avb.img**
11. **Apabila Anda ingin memodifikasi system/vendor terserah Anda, mereka ada di direktori "UnpackerSystem"**
12. **Sekarang kita akan repack itu ke dalam .br**
13. **Kembali ke UKA, pilih menu `9` (Menu: Build and convert to .br)**
14. **Pilih nomor `2` (Build .img with size input -> .br), ini akan merepack ke dalam .br sesuai input size yang kita masukkan**
15. **Apabila Anda ingin menyimpan hasil kompresi ke /sdcard, ketik `cd /sdcard/namafolderanda`, apabila tidak klik enter saja, nanti file hasil kompresi ada di `/data/local/UnpackerSystem`**
16. **Pilih file yang ingin Anda kompres (misalkan: system), apabila diminta menginput size:**
    - **Buka MT, masuk ke direktori UnpackerSystem/config, cari file system_size.txt, buka dan salin isinya, lalu kembali ke Termux dan pastekan, lalu klik enter**
    - **Apabila ada pemilihan versi Android, klik nomor `4`**
    - **Apabila Anda ingin mengompresi dengan (KOMPRESI TINGGI) pilih `7`, sementara apabila Anda ingin mengompresi dengan (KOMPRESI STANDARD) pilih `5` atau `6`. Tapi saya sarankan `7` agar size akhirnya kecil, namun memang kompresi ini agak lama, jadi Anda bisa menunggunya sambil menonton YouTube atau melakukan hal lain**

17. **Setelah semua selesai, pindahkan semua file di `/data/local/UnpackerSystem` ke folder yang Anda inginkan**
18. **Setelah itu Anda buat zip flashable dengan META-INF atau file lain sesuai struktur file yang seharusnya. Disaat membuat zip dengan MT Manager, saya sarankan ketika memulai zipping file pilih level kompresi Fastest**
19. **Setelah semua selesai, bersihkan direktori UKA dengan kembali ke Termux UKA, klik `12` lalu klik `8`**
20. **Setelah selesai sekarang Anda bisa keluar dan tes flash ROM-nya di recovery**

**Pastikan system dan vendor Anda resize, karena kalau tidak di resize system/vendor akan menjadi R/O, atau size tidak sesuai yang membuat penginstalan Gapps gagal.**
