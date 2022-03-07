# rediswp

Redis objek Cache WordPress ##Gaang

#Ubuntu 18

sudo apt update
sudo apt install redis-server

sudo nano /etc/redis/redis.conf

#tambahkan 

supervised ke supervised systemd

sudo systemctl restart redis.service

#Centos 7

sudo yum install epel-release

sudo yum update

sudo yum install redis

sudo systemctl start redis

sudo systemctl enable redis

#cek redis sudah berjalan atau tidak

redis-cli ping

#Jika sudah berjalan maka akan muncul 

PONG

#default, Redis berjalan pada port 127.0.0.1:6379

git clone https://github.com/FosterG4/rediswp.git

#Pasang pada wordpress

letakan object-cache.php didalam wp-content

#cek redis sudah bekerja atau tidak

redis-cli KEYS *

#kemudian refresh wordpress yang di jalankan
