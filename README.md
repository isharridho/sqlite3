๐ฆ๐ค๐ ๐ค๐๐ฒ๐ฟ๐ ๐ถ๐ป ๐ฃ๐ฎ๐ป๐ฑ๐ฎ๐ ๐๐ฎ๐๐ฎ๐๐ฟ๐ฎ๐บ๐ฒ

Google collab adalah salah satu tools yang biasanya digunakan oleh data analyst / data scientist. Namun google collab terbatas hanya untuk bahasa program python. Sementara untuk menjalankan query databases biasanya menggunakan tools yg berbeda seperti MySQL Workbench dll. Namun adakah cara yang dapat digunakan agar kita bisa menjalankan query di google collab? Tentu saja ada.

Berikut ini saya akan membagikan salah satu tips untuk menjalankan query di google collab. Cara ini sedikit berbeda dengan cara library โmysql.connectorโ, dimana jika pada mysql.connector kita membuat suatu connection terlebih dahulu ke database yang sudah ada, lalu mengolahnya di IDE python yg kita gunakan

Sementara untuk cara yang akan saya bagikan ini adalah, kita menjalankan query langsung dari file .csv yang kita punya di dalam IDE python yang kita gunakan. Nantinya file csv yang kita punya akan diubah menjadi suatu local file .db sehingga kita bisa melakukan query-query SQL  umum seperti create table, update data, query data, dll.  

Library yang digunakan pada cara kali ini adalah dengan menggunakan โsqlite3โ yang termasuk standard library python. Nantinya akan ada 2 buah fungsi yang digunakan. Fungsi 1 adalah untuk mengubah pandas DataFrame ke SQL DB table, dan fungsi 2 adalah untuk menjalankan SQL query pada pandas DataFrame. 
