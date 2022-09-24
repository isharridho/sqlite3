𝗦𝗤𝗟 𝗤𝘂𝗲𝗿𝘆 𝗶𝗻 𝗣𝗮𝗻𝗱𝗮𝘀 𝗗𝗮𝘁𝗮𝗙𝗿𝗮𝗺𝗲

Google collab adalah salah satu tools yang biasanya digunakan oleh data analyst / data scientist. Namun google collab terbatas hanya untuk bahasa program python. Sementara untuk menjalankan query databases biasanya menggunakan tools yg berbeda seperti MySQL Workbench dll. Namun adakah cara yang dapat digunakan agar kita bisa menjalankan query di google collab? Tentu saja ada.

Berikut ini saya akan membagikan salah satu tips untuk menjalankan query di google collab. Cara ini sedikit berbeda dengan cara library “mysql.connector”, dimana jika pada mysql.connector kita membuat suatu connection terlebih dahulu ke database yang sudah ada, lalu mengolahnya di IDE python yg kita gunakan

Sementara untuk cara yang akan saya bagikan ini adalah, kita menjalankan query langsung dari file .csv yang kita punya di dalam IDE python yang kita gunakan. Nantinya file csv yang kita punya akan diubah menjadi suatu local file .db sehingga kita bisa melakukan query-query SQL  umum seperti create table, update data, query data, dll.  

Library yang digunakan pada cara kali ini adalah dengan menggunakan “sqlite3” yang termasuk standard library python. Nantinya akan ada 2 buah fungsi yang digunakan. Fungsi 1 adalah untuk mengubah pandas DataFrame ke SQL DB table, dan fungsi 2 adalah untuk menjalankan SQL query pada pandas DataFrame. 
