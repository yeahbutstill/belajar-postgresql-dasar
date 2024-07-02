# Pengenalan Database Management System
- DBMS adalah aplikasi yang digunakan untuk me-manage data 
- Tanpa menggunakan DBMS, untuk me-manage data, seperti data produk, data customer, data penjualan, kita harus simpan dalam bentuk file (misal seperti ketika menggunakan Excel)
- DBMS biasanya berjalan sebagai aplikasi server yang digunakan untuk me-manage data, kita hanya tinggal memberi perintah ke DBMS untuk melakukan proses manajemen datanya, seperti menambah, mengubah, menghapus atau mengambil data 
- Contoh DBMS yang populer seperti MySQL, PostgreSQL, MongoDB, Oracle, dan lain-lain

# Pengenalan Relational Database
- Ada banyak sekali jenis-jenis DBMS, seperti Relational Database, Document Database, Key-Value Database, dan lain-lain 
- Namun yang masih populer dan kebanyakan orang gunakan adalah relational database 
- Relational database cukup mudah dimengerti dan dipelajari karena kita sudah terbiasa menyimpan data dalam bentuk tabular (tabel) seperti di Microsoft Excel atau di Google Doc Spreadsheet 
- Selain itu relational database memiliki perintah standard menggunakan SQL, sehingga kita mudah ketika ingin berganti-ganti aplikasi database (seperti MySQL, Oracle, PostgreSQL dan lain-lain)

![Cara Kerja DBMS](pic/img.png)

# Database Client
- Database client adalah aplikasi yang digunakan untuk berkomunikasi dengan DBMS 
- Biasanya DBMS sudah menyediakan database client sederhana yang bisa kita gunakan untuk berkomunikasi dengan DBMS agar lebih mudah 
- Atau kita bisa membuat aplikasi untuk berkomunikasi dengan DBMS, misal membuat aplikasi database client menggunakan Java, PHP atau bahasa pemrograman lainnya

# Database File
- Mayoritas DBMS menyimpan datanya di file, walaupun ada beberapa database yang hanya menyimpan datanya di memory (RAM)
- Namun jangan berpikir file database yang disimpan berupa file seperti Excel atau CSV (Comma Separated Value), tapi jauh lebih kompleks 
- Database File akan di optimasi oleh DBMS agar mempermudah DBMS dalam manajemen datanya, seperti insert, update, delete dan select 
- Tiap DBMS biasanya memiliki cara masing-masing mengelola Database File nya, dan kita tidak perlu harus tau, karena yang kita perlu tahu hanya cara berkomunikasi ke DBMS

# SQL
- Structured Query Language 
- Merupakan bahasa yang digunakan untuk mengirim perintah ke DBMS 
- SQL adalah bahasa yang mudah karena hanya berisi instruksi untuk menyimpan, mengubah, menghapus atau mengambil data melalui DBMS 
- Secara garis besar, semua perintah SQL di Relational Database itu hampir sama, namun biasanya tiap DBMS ada improvement yang membedakan hal-hal kecil dalam perintah SQL, namun secara garis besar perintahnya tetap sama

# PostgreSQL
- PostgreSQL adalah DBMS Relational OpenSource yang sangat populer, terutama di perusahaan enterprise 
- Tidak hanya OpenSource, PostgreSQL juga gratis untuk digunakan 
- Proyek PostgreSQL dimulai sejak tahun 1986, dibawah arahan Professor Michael Stonebreaker di Universitas California, Berkeley 
- PostgreSQL sangat populer sekali dikalangan perusahaan Enterprise
- https://www.postgresql.org/ 

![Kenapa Belajar PostgreSQL](pic/img_1.png)
https://db-engines.com/en/ranking/relational+dbms 

# PostgreSQL vs MySQL
- MySQL sampai sekarang menjadi salah satu DBMS OpenSource yang paling populer di dunia 
- Namun, banyak perusahaan besar yang menggunakan database PostgreSQL, hal ini dikarenakan PostgreSQL memiliki fitur yang lebih kaya dibandingkan MySQL 
- MySQL fokus pada performa dan kecepatan, oleh karena itu fitur nya tidak sebanyak di PostgreSQL

# Menggunakan PostgreSQL Client
- PostgreSQL Client adalah aplikasi berbasis terminal yang disediakan oleh PostgreSQL untuk berkomunikasi dengan PostgreSQL Server 
- Karena berbasis terminal, sehingga PostgreSQL Client sangat cocok untuk kita gunakan misal ketika di server production, dimana kita menginstall PostgreSQL di linux server yang berbasis terminal misal 
- Kita tidak perlu menginstall PostgreSQL Client secara terpisah, karena sudah tersedia di dalam aplikasi PostgreSQL ketika kita menginstallnya 
- PostgreSQL Client bisa diakses lewat terminal dengan nama program psql

# DBeaver
- DBeaver adalah aplikasi GUI Client berbasis Desktop yang free dan opensource yang bisa digunakan sebagai aplikasi database client 
- Aplikasi DBeaver sangat mempermudah kita melakukan manajemen data di PostgreSQL karena berbasis Desktop
- https://dbeaver.io/ 

# PGAdmin
- PGAdmin adalah aplikasi berbasis web yang bisa digunakan untuk manajemen data di PostgreSQL 
- Aplikasi PGAdmin dulunya berupa aplikasi desktop, namun diversi terbaru diubah menjadi aplikasi web
- https://www.pgadmin.org/ 

# JetBrains DataGrip
- DataGrip adalah aplikasi Database Client yang berbayar 
- DataGrip mendukung banyak sekali DBMS sehingga kita cukup menggunakan DataGrip untuk manajemen semua database yang kita gunakan 
- Selain mendukung Relational DBMS, DataGrip juga mendukung DBMS yang NoSQL seperti MongoDB, Cassandra, dan lain-lain
- https://www.jetbrains.com/datagrip/

# Run PostgreSQL with Docker Compose
- docker compose -p belajar-postgresql-dasar up
- docker exec -it <mycontainer postgresql> sh

# Database
- Database adalah tempat kita menyimpan table di PostgreSQL 
- Jika kita misalkan table di PostgreSQL adalah sebuah file, maka database adalah folder nya, dimana kita bisa menyimpan banyak table di sebuah database 
- Biasanya pembuatan kita akan membuat satu database untuk satu jenis aplikasi, walaupun satu aplikasi bisa menggunakan lebih dari satu database, namun lumrahnya, satu aplikasi akan menggunakan satu database

![DBMS](pic/img_2.png)

# Menggunakan PostgreSQL Client
- psql --host=localhost --port=5432 --dbname=postgres --username=khannedy --password

# Melihat Semua Database di PostgreSQL
- \l 
- select datname from pg_database;

# Membuat Database
- create database nama_database;

# Menghapus Database
- drop database nama_database;

# Menggunakan Database
- \c namadatabase

# Tipe Data
- Saat kita membuat tabel di Excel, kita bisa menentukan tipe data apa yang kita masukkan ke tiap kolom di Excel 
- Di PostgreSQL, kita juga bisa menentukan tipe data tiap kolom yang kita buat di sebuah tabel 
- Ada banyak sekali tipe data yang tersedia di PostgreSQL, dari yang sederhana, sampai yang kompleks. 
- Biasanya kita akan menggunakan tipe data sesuai dengan kebutuhan kolom yang perlu kita buat
 
![Tipe Data](pic/img_3.png)

# Tipe Data Number
- Secara garis besar, tipe data number di PostgreSQL ada dua jenis; 
- Integer, atau tipe number bilangan bulat 
- Floating Point, atau tipe data number pecahan

![Tipe Data Number](pic/img_4.png)

# DECIMAL / NUMERIC
- Selain Integer dan Floating Point, di PostgreSQL terdapat tipe data DECIMAL / NUMERIC 
- Ini tipe data number khusus yang bisa ditentukan jumlah precision dan scale nya

![Decimal / Numeric](pic/img_5.png)

# Tipe Data String
- Selain number, biasanya kita sering menyimpan data di dalam tabel dalam bentuk tulisan 
- Tipe data ini namanya tipe data String atau Text 
- Ada banyak tipe data String di PostgreSQL

# CHAR dan VARCHAR
- Pertama tipe data String di PostgreSQL adalah CHAR dan VARCHAR 
- Kita bisa menentukan jumlah panjang maksimal karakter yang bisa ditampung oleh CHAR dan VARCHAR dengan menggunakan kurung buka lalu masukan jumlah maksimal karakter dan diakhiri kurung tutup 
- Misal, CHAR(10) atau VARCHAR(10) artinya tipe data String dengan maksimal jumlah karakternya adalah 10 karakter 
- Maksimum ukuran CHAR atau VARCHAR adalah 65535 karakter

# Perbedaan CHAR dan VARCHAR
![Perbedaan CHAR dan VARCHAR](pic/img_6.png)

# Text
- Selain CHAR dan VARCHAR, tipe data String yang lainnya adalah TEXT 
- Berbeda dengan CHAR dan VARCHAR yang kita bisa tentukan panjang maksimum nya, TEXT tidak memiliki maksimum  panjang nya

# Tipe Data Date dan Time
- Selain tipe data Number dan String, biasanya kadang kita sering menyimpan data waktu atau tanggal 
- Sebenarnya bisa kita gunakan String untuk menyimpan data waktu atau tanggal, namun itu tidak direkomendasikan, karena akan menyulitkan kita ketika nanti butuh melakukan manipulasi waktu atau tanggal di PostgreSQL

# Jenis-Jenis Tipe Data Date dan Time
![Jenis-Jenis Tipe Data Date dan Time](pic/img_7.png)

# Format Tipe Data Date dan Time
- Format penulisan tipe data waktu, bisa menggunakan format 
- Timestamp : YYYY-MM-dd HH:mm:ss 
- Date : YYYY-MM-dd 
- Time : HH:mm:ss

# Tipe Data Boolean
- BOOLEAN adalah tipe data kebenaran, yang artinya datanya hanya ada dua jenis, benar atau salah 
- Benar direpresentasikan dengan data TRUE, sedangkan salah direpresentasikan dengan data FALSE

# Tipe Data Enum
- Saat membuat kolom, kadang ada jenis tipe data Text, namun isi datanya sudah fix, misal Jenis Kelamin, Kategori, dan sejenisnya 
- Kasus seperti itu bisa menggunakan tipe data Enum 
- Tipe data Enum harus dibuat terlebih dahulu, dan ditentukan Value yang diperbolehkan

# Membuat Tipe Data Enum
- Untuk membuat tipe data enum, kita bisa menggunakan perintah :
- CREATE TYPE NAMA_ENUM AS ENUM ('VALUE1, ‘VALUE2’, 'VALUE3');

# Dan Lain-Lain
- Sebenarnya masih banyak jenis tipe data yang lain yang didukung oleh PostgreSQL, namun itu bisa kita pelajari jika memang ada kebutuhan spesifik 
- Seperti misal tipe data binary, json, xml dan lain-lain
- https://www.postgresql.org/docs/current/datatype.html 

# Table
- Data biasanya disimpan di dalam tabel di PostgreSQL 
- Tiap tabel biasanya menyimpan satu jenis data, misal ketika kita membuat aplikasi toko online, kita akan membuat tabel barang, tabel pelanggan, tabel penjual, dan lain-lain 
- Sebelum kita bisa memasukkan data ke tabel, kita wajib terlebih dahulu membuat tabelnya terlebih dahulu 
- Dan tiap tabel yang kita buat, wajib ditentukan kolom-kolom nya, dan tipe data tiap kolom nya 
- Kita juga bisa mengubah tabel yang sudah terlanjur dibuat, seperti menambah kolom baru, mengubah kolom yang sudah ada, atau menghapus kolom

# Melihat Table
- \dt 
- select * from pg_tables where schemaname = ‘public’;

# Melihat Struktur Table
- \d nama_tabel

# Null Value
- Null adalah nilai ketika kita tidak mengisi data ke dalam kolom 
- Secara default, saat kita membuat kolom, kolom tersebut bisa bernilai NULL, jika kita tidak ingin menerima nilai NULL, kita bisa menambahkan NOT NULL ketika pembuatan kolom nya

# Default Value
- Saat kita menyimpan data ke dalam tabel, lalu kita hanya menyimpan beberapa kolom (tidak semuanya), kolom yang tidak kita beri nilai secara default nilainya adalah NULL 
- Jika kita ingin mengubah default value nya, kita bisa menambahkan perintah DEFAULT NILAI ketika pembuatan kolom nya 
- Khusus tipe data DATETIME atau TIMESTAMP, jika kita ingin menggunakan default value dengan nilai waktu saat ini, kita bisa gunakan kata kunci CURRENT_TIMESTAMP
