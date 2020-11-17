---
title: "Mengenal Elasticsearch"
date: 2020-11-17T09:46:03+07:00
draft: false
author: "Teten Nugraha"
tags: ["Elasticsearch", "Lucene","Search engine"]
categories: ["Elasticsearch"]
---


![I wish all my images had alt text 🤦‍♂️](/img/post/elastic.png)



## Pengenalan

Elasticsearach adalah sebuah mesin pencari yang menggunakan libary Lucene yang juga dikhususkan untuk melakukan pencarian cepat. Elasticsearch menyediakan layanan untuk memudahkan user melakukan fungsi search full text pada aplikasinya dengan menggunakan protocol HTTP dan JSON document. Elasticsearch dibuat menggunakan bahasa pemrograman Java. Sebagian product elasticsearch sudah dibawah lisensi opensource dan sebagian lagi dibawah lisensi Elasticsearch itu sendiri. Official client yang sudah stable saat ini yaitu Java, .NET, PHP, Python, Apache Groovy, Ruby dan bahasa pemrograman Lainnya.



## Bedanya dengan RDBMS ?

Karena Elasticsearch adalah bagian dari database NoSQL dimana tidak ada relasi seperti yang sering kita gunakan misalkanya menggunakan MySQL atau Postgresql. Ada beberapa perbedaan yang major antara RDBMS vs NoSQL

| RDBMS (MySQL, PostgreSQL, Oracle, SQLServer dll) | ElasticSearch |
| ------------------------------------------------ | ------------- |
| Database                                         | Index         |
| Table                                            | Type          |
| Row                                              | Document      |



## Permasalahan apa yang solve pakai Elasticsearch ?

Kebanyakan ecommerce menggunakan elasticsearch untuk melakukan pencarian cepat terhadap suatu product. Kita bisa lihat pada salah satu estore Blibli, seperti dibawah ini.

![I wish all my images had alt text 🤦‍♂️](/img/post/blibli.png)

Ketika mengetikan satu product di bagian text pencarinya, maka blibli mengeluarkan informasi tentang

1. Pencarian Populer
2. Product Popuper
3. Seller yang menjual product tersebut

informasi itu di keluarkan dalam hitungan detik, kita ingat bahwa sebuah estore mungkin mempunyai jutaan data product dan seller ditambah data pembeliannya, bisa dibayangkan kalau sugesti diatas menggunakan RDBMS, mungkin blibli bisa mengeluarkan informasi sugesti itu dalam waktu yang cukup lama. Nah untuk permasalah seperti itu lah Elasticsearch menyediakan solusinya, disamping itu Elasticsearch juga bisa digunakan untuk menyimpan log aplikasi menggunakan Logstach dan Kibana.



## Kapan kita menggunakan Elasticsearch ?

Yaa seperti contoh kasus diatas, kita bisa menggunakan elasticsearch ketika kita ingin mengeluarkan informasi data secara cepat yang mempunyai spesifikasi yang sangat beragam, misalkan kalian mempunyai toko online, dan kalian ingin mengeluarkan data secara cepat tentang suatu product yaitu:

- Product Terbaru
- Stok Product
- Siapa Penjual nya
- Top Testimony product tersebut
- Barang termurah ke barang termahal
- dll 

Oke pada post selanjut nya, kita akan membahas cara instalassi Elasticsearch di windows 10 dan kita akan melakukan CRUD Sederhana.