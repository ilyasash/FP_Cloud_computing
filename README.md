# Final Project TKA D - Kelompok 5



| Nama                                                | NRP        |
| --------------------------------------------------- | ---------- |
| Muhammad Hilmy Adhi Pradityo  | 5027211053 |
| Rakha Aldo Nirwasita   | 5027211054 |
| Wiridlangit Suluh Jiwangga   | 5027211064 |
| Maulana Ilyasa Shafrizaliansyah  | 5027211065 | 
| Auditya Maulana Adnan  | 5027211068 |
| Evan Darya Kusuma  | 5027211069 |


# Problem Explanation

Pada suatu saat di akhir semester 5 terdapat 6 pemuda dari Jurusan Teknologi Informasi yanng diberikan sebuah projek dari dosennya untuk Final assessment mata kuliah Cloud computing yang dimana diperintahkan untuk merncang sebuah arsitektur Cloud yang efisien untuk mendukung sebuah aplikasi yang sedang dibangun bernama app.py. Namun Universitas hanya mampu memberikan dana dengan maksimal sebanyak 65 US$ atau sekitar +- 1 juta rupiah per bulan. Dengan permasalahan itu kita dituntut untuk membangun arsitektur yang efisien serta optimal demi kemajuan ITS, VIVAT!!!

# Arsitektur
- Dalam konfigurasi nya kelompok kami memilih untuk memakai Digital Ocean 
- Kelompok kami menggunakan 1 Load Balancer, 3 App Worker, dan 1 Database Server
- Load Balancer memiliki spesifikasi 512 MB/CPU dan memori 10 GB dengan harga $4
- Masing-masing App Worker memiliki spesifikasi 1 GB/CPU dan memori 35 GB dengan harga $8
- Database Server memiliki spesifikasi 2 GB/CPU dan memori 34 GB dengan harga $30
- Total biaya yang diperlukan sebesar $58

![App Screenshot](https://i.ibb.co/PxQHkJb/Whats-App-Image-2023-12-15-at-00-08-12.jpg)

# Tabel Harga
Berikut merupakan rincian biaya yang diperlukan dari project yang kami buat
![App Screenshot](https://i.ibb.co/jr94frQ/Whats-App-Image-2023-12-15-at-00-35-57.jpg)
  
# Implementasi
- Pertama-tama setelah membuat project pada Digital Ocean, buat Droplets yang nantinya akan menjadi Load Balancer dan App Worker dengan klik tombol `CREATE` di bagian kanan atas lalu pilih `DROPLETS`
![App Screenshot](https://i.ibb.co/JFB7NKV/Whats-App-Image-2023-12-14-at-22-52-57.jpg)

- Pilih Region, di sini kelompok kami memilih region Singapore
![App Screenshot](https://i.ibb.co/PW33bZY/Whats-App-Image-2023-12-14-at-22-54-43.jpg)

- Pilih OS yang akan digunakan, kelompok kami memilih OS `UBUNTU`
![App Screenshot](https://i.ibb.co/NLfhr17/Whats-App-Image-2023-12-14-at-22-55-09.jpg)

- Pilih jenis resource yang akan digunakan sesuai dengan arsitektur yang ditentukan di awal
![App Screenshot](https://i.ibb.co/LkSsTNH/Whats-App-Image-2023-12-14-at-22-55-43.jpg)

- Setelah pilih resource, setel password pada setiap `DROPLETS`
![App Screenshot](https://i.ibb.co/fkSZq2Z/Whats-App-Image-2023-12-14-at-22-56-03.jpg)

- Tentukan hostnamenya dan klik tombol `Create Droplet`
![App Screenshot](https://i.ibb.co/2580GsY/Whats-App-Image-2023-12-14-at-22-56-18.jpg)

- Jika sudah membuat semua `DROPLETS`, buat databasenya dengan klik tombol `CREATE` dan pilih `DATABASES`
![App Screenshot](https://i.ibb.co/m4NGGkh/Whats-App-Image-2023-12-14-at-23-09-19.jpg)

- Pilih region dan tipe database, kelompok kami menggunakan region Singapore dan database `MongoDB`
![App Screenshot](https://i.ibb.co/2n5rWPH/Whats-App-Image-2023-12-14-at-23-09-45.jpg)

- Pilih jenis harga sesuai dengan arsitektur yang sudah ditentukan, pada kasus ini kelompok kami memilih yang harga `$30`
![App Screenshot](https://i.ibb.co/hZJkbvx/Whats-App-Image-2023-12-14-at-23-10-03.jpg)

- Set nama cluster, lalu klik tombol `Create Database Cluster`
![App Screenshot](https://i.ibb.co/YybpVNB/Whats-App-Image-2023-12-14-at-23-10-24.jpg)

# Pengujian End Point
Pengujian Endpoint berikut menggunakan Insomnia
- Get Orders\

<p align="center">
    <img src="https://i.ibb.co/Ry9Ty0m/GET-ORDERS.png">
    
- Get Orders By ID\

<p align="center">
    <img src="https://i.ibb.co/R2j5vS8/GET-ORDERS-BY-ID.png">
    
- Post Orders\

<p align="center">
    <img src="https://i.ibb.co/d6pL0BP/POST-ORDERS.png">
    
- Update Orders\

<p align="center">
    <img src="https://i.ibb.co/gSGvDMb/UPDATE-ORDERS.png">
    
- Delete Orders\
<p align="center">
    <img src="https://i.ibb.co/j51s0bJ/DELETE-ORDER.png">
    
# Pengujian Load Testing

Pengujian yang di lakukan dengan menggunakan Locust dan dihasilkan seperti berikut :

Spawn Rate 25
<p align="center">
    <img src="https://i.ibb.co/jbgYxFP/image.png">

Spawn Rate 50
<p align="center">
    <img src="https://i.ibb.co/7r7q6Qw/image.png">

Spawn Rate 100
<p align="center">
    <img src="https://i.ibb.co/TLmYQW6/image.png">

  # Kesimpulan

  # Pembagian Tugas
  
  Pembagian Kelompok:
  
1. Arsitektur dan harga : Semua
2. Implementasi / nyetting smua vm / deploy aplikasi: Evan, Didit, Wirid
3. Test pake locust: Yasa, Hilmy, Rakha
4. Laporan di github: Yasa, Hilmy, Rakha

Dengan ini Kelompok D5 izin pamit,

<p align="center">
    <img src="https://i.ibb.co/Z6Hf5Rq/82u6f1.jpg">




