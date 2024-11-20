Berikut adalah tutorial lengkap untuk menginstal Apache ActiveMQ Artemis di CentOS 9:
Persyaratan : OS Centos 9, Java

1. Langkah pertama siapan OS Linux Centos 9
![image](https://github.com/user-attachments/assets/d42aea10-25e6-47dc-b498-90dfd86c0935)
2. Pastikan sudah terinstall Java, disini saya pakai Java Version 11
![image](https://github.com/user-attachments/assets/2ed1b9e2-2c6e-4838-9901-925e522e81ce)
Setelah Java terinstall jangan lupa untuk menambahkan `PATH` Java pada file `.bashrc` seperti gamabar berikut
![image](https://github.com/user-attachments/assets/0baa3a61-1af3-4a27-8be1-39408ee77ac8)
3. Download AMQ Artemis dengan command berikut :
   `wget https://archive.apache.org/dist/activemq/activemq-artemis/2.38.0/apache-artemis-2.38.0-bin.tar.gz`
   ![image](https://github.com/user-attachments/assets/0393c4e4-2246-4fe2-aa3f-5f08b61bc89a)
3.1. Setelah download selesai, Ekstrak file yang sudah di download :
   ![image](https://github.com/user-attachments/assets/8dd5298c-a76c-486e-b803-2274bd1b5d68)
3.2. Ganti Nama Folder, lalu masuk kedalam direktori apache-artemis
   ![image](https://github.com/user-attachments/assets/21343d69-096e-4124-b00e-2619fee79c6f)
4. Create Broker dengan command berikut :
   `./bin/artemis create broker1`
   ![image](https://github.com/user-attachments/assets/410781db-64dc-449d-8cea-47aa1aa8b741)
5. Setelah Create Broker, masuk kedalam direktori broker1 lalu running broker dengan command berikut :
   `./bin/artemis run`
   ![image](https://github.com/user-attachments/assets/9fb15ac6-2e89-4427-8dcc-9004e5aa8036)
   ![image](https://github.com/user-attachments/assets/deb74d48-347b-44cf-9fd8-f55242f9775d)
6. Setelah Broker running, akses Dashboard Apache Active MQ dengan masuk browser dan akses link berikut :
   `http://localhost:8161/console` dan login dengan akses yang sudah dibuat pada langkah 4.
   ![image](https://github.com/user-attachments/assets/0e2c8e47-e6c7-4ad3-9925-abccfd110ac9)
   ![image](https://github.com/user-attachments/assets/0a52deb6-8cb1-4d8b-b77e-ec5e44ca5ff2)



