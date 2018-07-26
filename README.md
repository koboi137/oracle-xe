# Oracle Database Expree Edition
Ini adalah installer Oracle Database Express Edition yang di buat untuk memudahkan installasi di dalam system operasi yang berbasis ubuntu.
File setup ini sengaja saya buat karena dalam installasi Oracle XE sendiri harus melewati step yang lumayan panjang.
Di sini saya buat menjadi se simple mungkin agar para pengguna/developer yang ingin mencoba Oracle XE tidak lagi melewati step yang panjang dalam melakukan installasi di system ubuntu.

# Cara installasi
1. ```$ git clone https://github.com/koboi137/oracle-xe```
2. ```$ cd OracleXE```
3. ```$ bash setup.sh```

Secara default service oracle-xe belum otomatis berjalan saat system operasi di restart.
Untuk membuat agar service oracle-xe berjalan saat di restart, kita bisa menambahkan perintah "bash /usr/sbin/startup.sh" ke dalam file /etc/rc.local yang ada pada system.

# Konfigurasi APEX
```
# http://localhost:8080/apex/apex_admin
username: ADMIN
password: admin
```

# Konfigurasi User Database
```
hostname: localhost
port: 1521
sid: xe
username: system
password: oracle
```
