# praktikum-sistem-operasi-SK3B
- Buatlah laporan proses instalasi di komputer mahasiswa dan tampilkan screenshotnya

1. install linux ubuntu 24.04 dari google
![Screenshot 2024-08-30 145559](https://github.com/user-attachments/assets/43d9c676-787a-43b7-9da1-bf8a75b0d08a)

2. setelah install linux berikutnya install rufus, untuk membuat USB bootable untuk menginstal sistem operasi seperti Linux dari file ISO.
![Screenshot 2024-08-30 145651](https://github.com/user-attachments/assets/9836a9e6-db46-4f39-885c-2e2d16d33644)

3. pada rufus kita akan memlihi USB yang kita gunakan dengan kapasitas minimal 8gb, lalu pilih ubuntu untuk Boot selection setelah itu click START
   
![Screenshot 2024-08-30 091509](https://github.com/user-attachments/assets/70f61d65-68a1-4409-9857-5b54f6c71f87)

4. untuk dual boot dari satu storage pastikan kita melakukan partisi terlebih dahulu pada storage kita, minimun untuk ubuntu adalah 25gb,
![Screenshot 2024-08-30 150125](https://github.com/user-attachments/assets/c20ed1b8-b489-4896-b32e-2238e5090796)

5. jika sudah semua selanjutnya kita akan masuk ke bios untuk mematikan secure boot dan matikan juga Bitlocker jika perlu
![secureboot](https://github.com/user-attachments/assets/05ce799c-799c-4f26-aa6c-10879197dfa4)

6. setelah itu save dan kita akan kembali ke windows, tekan tombol power lalu tekan shift dan tekan restart, kita akan masuk ke menu option
   pada menu itu pilih Use a device dan pilih usb yang sudah kita install linux
![20240830_154416](https://github.com/user-attachments/assets/7406e134-59b4-4f2e-a63f-619f71b6419e)
![20240830_154421](https://github.com/user-attachments/assets/4496f003-9508-4a96-a889-417f4f07b48b)

7. pilih Try or Install Ubuntu
![20240830_154437](https://github.com/user-attachments/assets/67070592-16c0-40ea-9c45-1e73cbdd4e18)
   
8. jika sudah masuk ubuntu kita akan melakukan instalasi ubuntu pada pc kita
![20240830_154623](https://github.com/user-attachments/assets/231d18ba-0d72-450c-8c92-376beb8cd8d5)

9. pada opsi what do you want to do with ubuntu? kita pilih opsi install ubuntu
![20240830_154714](https://github.com/user-attachments/assets/cf5bf82f-4951-4c3d-94b8-0f4469bfde56)

10. lalu di opsi bagaiman kita ingin menginstall ubuntu kita dapat memilih opsi pertama, jika memilih itu ubuntu akan langsung terinstall ke storage yang sudah kita partisi
    sebelumnya, namun disini kita memilih opsi ketiga
![20240830_154813](https://github.com/user-attachments/assets/f95585c1-33bf-49cb-8d8e-2ee8b8ce3cfb)

11. pilih storage partisi kita lalu klik change di bagian bawah kiri
![20240830_154825](https://github.com/user-attachments/assets/118ccca0-f001-446d-af75-eec043f761c8)

12. pada opsi change kita pilih mount point /
![20240830_154837](https://github.com/user-attachments/assets/3d29a994-cab1-4f3a-ad53-aa46f481d672)

13. buat nama akun dan pasword kita
![20240830_154916](https://github.com/user-attachments/assets/4575fd05-9494-48c3-b36b-2185f91432d2)

14. pilih zona waktu kita, kita bisa mencarinya secara manual atau ketik kota kita pada kolom atas kanan
![20240830_154938](https://github.com/user-attachments/assets/0bc687f6-c234-493f-b3f6-a3c4b2ebf670)

15. jika sudah semua klik install dan tunggu beberapa saat
![20240830_154951](https://github.com/user-attachments/assets/60e131ce-0d52-49e0-8546-14b868c1a7b5)

16. jika sudah masuk lagi ke bios dan di opsi boot kita akan merubah boot priorities ubuntu menjadi yang pertama jadi kita bisa memilih untuk boot ke windows
    atau ubuntu saat booting pc
![20240830_155533](https://github.com/user-attachments/assets/3c61fb61-f6aa-4875-bd85-5ad4d6880604)
![20240830_155616](https://github.com/user-attachments/assets/be1e359c-0ea1-4407-8c3c-b3aca70cc0bf)

17. selesai
![Screenshot from 2024-08-30 15-56-56](https://github.com/user-attachments/assets/6e72cffd-97bc-4b8c-a817-4ccc645e0f6a)


- Analisalah pada gambar kenapa saat instalasi perlu dipilih "/" pada opsi Mount Point?
  
Saat instalasi Ubuntu, memilih "/" sebagai opsi mount point berarti kita mengatur partisi tersebut untuk menjadi root directory dari sistem.
Direktori "/" adalah tempat utama di mana semua file sistem, aplikasi, dan data pengguna disimpan. Dengan memilih "/" untuk partisi ini, kita memastikan bahwa
seluruh struktur file sistem Linux akan berada di partisi tersebut


- Berikan penjelasan tentang ext4, ext3, swap, ntfs, fat32, btrfs

1. Ext4 adalah sistem file yang sering digunakan di Linux Ext4 menggunakan jurnal yang lebih efisien untuk melindungi data dan mengurangi fragmentasi file
   sehingga memberikan kecepatan dan stabilitas yang lebih baik

2. Ext3 adalah sistem file Linux yang menggunakan jurnal untuk melindungi data dan mempermudah pemulihan dari kegagalan
   Ext3 memiliki batasan ukuran file dan kinerja dibandingkan dengan Ext4 yang menawarkan peningkatan dalam kapasitas dan kecepatan

3. Swap adalah ruang di hard drive yang digunakan sebagai tambahan memori ketika RAM penuh memungkinkan sistem untuk menyimpan data yang tidak aktif di RAM ke disk
   sehingga memori fisik dapat digunakan untuk proses yang lebih penting swap membantu mencegah kehabisan memori meski akses ke swap lebih lambat dibandingkan dengan RAM

4. NTFS adalah sistem file yang dikembangkan oleh Microsoft dan digunakan terutama di Windows NTFS mendukung fitur-fitur canggih seperti izin file, enkripsi,
   dan kompresi data ini juga dapat menangani file dan partisi yang sangat besar dengan efisien NTFS sering digunakan untuk hard drive dan SSD di komputer Windows tetapi Linux juga dapat membaca dan menulis ke partisi NTFS dengan alat tambahan

5. FAT32 adalah sistem file yang kompatibel dengan banyak sistem operasi dan sering digunakan pada drive USB dan kartu memori dan memiliki batas ukuran file maksimal 4gb dan partisi maksimal 8TB FAT32 menawarkan kompatibilitas luas tanpa fitur canggih seperti enkripsi

6. Btrfs adalah sistem file modern di Linux yang menawarkan fitur seperti snapshot, kompresi, dan cek integritas data Btrfs dirancang untuk menggantikan Ext4 dengan keunggulan dalam manajemen ruang, pemulihan data, dan skalabilitas, mendukung partisi dan file besar dengan efisiensi tinggi
