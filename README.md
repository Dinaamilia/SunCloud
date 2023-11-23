# SUN CLOUD
Sun Cloud merupakan sebuah sistem yang dibuat untuk memberikan layanan penyimpanan bagi siswa maupun guru dalam menunjang kegiatan akademik di sekolah sesuai dengan kebutuhan yang dibutuhkan dimana hanya pengguna mempunyai akun saja yang dapat mengakses, sehingga data-data akan lebih aman.

## Feature

- Pengguna dapat menambahkan file ke next cloud
- Pengguna dapat memindahkan file ke next cloud 
- Pengguna dapat menghapus file next cloud 
- Berbagi secara online di internet (melakukan file sharing kepada user lain dan juga dapat sharing melalui tautan)
- Pengguna dapat membuka dokumen secara langsung tanpa mengunduhnya.



## Tech
sistem ini dibangun menggunakan : 
- Sebuah laptop
- Domain Name Server 
- Laptop Client 
- Mouse 
- Keyboard 
- Lynux operating system (Ubuntu Server) 
- PHP 
-  PostgreSQL  
-  Next Cloud
-  Firewall
-   Oracle VM Virtual Box


## Tahap Konfigurasi Penyimpanan Awan
Pada tahapan konfigurasi penyimpanan awan kami menggunakan nextcloud pada linux ubuntu yang dijalankan melalui virtual machine agar sistem penyimpanan bisa diakses melalui jaringan internet atau public.

# Konfigurasi Router Indihome 

- Masuk ke pengaturan router Indihome dengan mengakses alamat IP router melalui browser
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/konfig%20router%201.png?raw=true)
- Selanjutnya masuk ke menu Application kemudian pilih Port Forwarding 
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/konfig%20router%202.png?raw=true)
- Selanjutnya centang kolom enable agar port aktif. Kemudian isi kolom Name sesuai dengan kebutuhan, Pada kolom Protocol pilih TCP. Pada WAN Port Start dan WAN Port End isi dengan angka 80. Pada LAN Host IP Address isi dengan alamat IP Server nextcloud, kemudian pada LAN Port Start dan LAN Port End isi dengan angka 80, kemudian klik Add.
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/konfig%20router%203.png?raw=true)
# Konfigurasi DNS menggunakan No-IP
- Buka situs www.noip.com melalui browser. Kemudian masuk dengan akun yang telah didaftarkan.
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/konfig%20DNS%201.png?raw=true)
- Pilih menu Dynamic DNS, kemudian pilih No-IP Hostnames. Kemudian klik Create Hostname untuk membuat hostname baru.
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/konfig%20DNS%202.png?raw=true)
- Isi Hostname dan pilih Domain yang tersedia, disini kami memilih domain sytes.net. Pada IPv4 Address secara otomatis membaca IP Public Jaringan yang kami gunakan, jika sudah klik Create Hostname.
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/konfig%20DNS%203.png?raw=true)
- Setelah melakukan konfigurasi, sistem penyimpanan awan yang sudah dibuat sekarang dapat diakses di luar jaringan lokal melalui jaringan internet dengan cara mengakses suncloud.sytes.net melalui browser. 
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/konfig%20DNS%204.png?raw=true)

# Tahap Modifikasi Nextcloud
Pada tahap modifikasi nextcloud dilakukan untuk memenuhi tujuan penyimpanan awan yang diimplementasikan. Adapun beberapa modifikasi yang dilakukan : 
- Memberikan kapasitas penyimpanan yang berbeda setiap user.
- Merubah tampilan dari nextcloud, dengan tampilan suncloud.
- Menambahkan fitur Document viewer.

Setiap user memiliki kapasitas penyimpanan yang berbeda sesuai dengan kebutuhan hanya administrator yang mempunyai kapasitas penyimpanan unlimited atau tidak terbatas. Adapun pembagian kapasitas penyimpanan pada masing-masing user sebagai berikut : 

| USER | KAPASITAS |
| ------ | ------ |
| Admin | Unlimited |
| Guru | 10 GB |
| Siswa | 5 GB |

# Tahap Pengujian
Pada tahapan ini akan dilakukan pengujian terhadap aktivitas dalam jaringan sistem penyimpanan menggunakan nextcloud. 

- Pada Nextcloud kita dapat membuat user sesuai dengan kebutuhan. Hanya pengguna yang mempunyai akun saja yang dapat mengakses, sehingga data-data akan lebih aman.
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/PENGUJIAN%201.png?raw=true)
- Setiap user dapat menambahkan, memindahkan, menghapus, mengubah data ke nextcloud. 
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/pengujian%202.png?raw=true)
- Pengguna juga dapat melakukan file sharing kepada user lain dan juga dapat sharing melalui tautan. 
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/pengujian%203.png?raw=true)
- Pengguna dapat membuka dokumen secara langsung tanpa mengunduhnya.
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/pengujian%204.png?raw=true)
- Pengguna juga dapat memutar media pada nextcloud. 
![alt text](https://github.com/Dinaamilia/Sun-Cloud/blob/main/pengujian%205.png?raw=true)

implementasi penyimpanan awan menggunakan Nextcloud pada mesin virtual di bidang pendidikan adalah langkah yang bermanfaat dan relevan. Hal ini memungkinkan akses data yang mudah, kolaborasi yang lebih baik, dan manajemen data yang lebih efisien. Dengan demikian, teknologi ini memiliki potensi untuk memperkaya pengalaman pendidikan dan memungkinkan lembaga pendidikan untuk mengoptimalkan sumber daya mereka.


##### Sistem ini disusun oleh :
> Yoga Putra R.		21050974043
> Arju Kurnia		21050974029
> Dina Amilia		21050974008
> Awwalia Arofatun 	21050974030
> Yusi Eka Sonia F.	21050974040

