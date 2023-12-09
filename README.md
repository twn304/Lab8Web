# Lab8Web
## Praktikum-8
## PHP dan DataBase MySQL
## Langkah Langkah Praktikum
### Menjalankan MySQL server
Untuk menjalankan MySQL Server dari menu XAMPP Contol.

![ss1](/image/ss1.png)
### Mengakses MySQL Client menggunakan PHP MyAdmin
Pastikan webserver Apache dan MySQL server sudah dijalankan. Kemudian buka
melalui browser: http://localhost/phpmyadmin/


### Membuat Database: Studi Kasus Data Barang
- Membuat Database 
```
Create Database latihan1;
```
- Membuat Table 
```
CREATE TABLE data_barang (
    id_barang int(10) auto_increment Primary Key,
    kategori varchar(30),
    nama varchar(30),
    gambar varchar(100),
    harga_beli decimal(10,0),
    harga_jual decimal(10,0),
    stok int(4)
);
```


### Menambahkan Data 
```
INSERT INTO data_barang (kategori, nama, gambar, harga_beli, harga_jual, stok)
VALUES ('Elektronik', 'HP Samsung Android', 'hp_samsung.jpg', 2000000, 2400000, 5),
('Elektronik', 'HP Xiaomi Android', 'hp_xiaomi.jpg', 1000000, 1400000, 5),
('Elektronik', 'HP OPPO Android', 'hp_oppo.jpg', 1800000, 2300000, 5);
```
