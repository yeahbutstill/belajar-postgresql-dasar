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

