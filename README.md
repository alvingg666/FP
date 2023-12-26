#   Web Server #
Tugas yang di buat pada final project kali ini adalah menginstall apache2
![Picsart_23-11-30_18-42-27-335](https://kitaadmin.com/wp-content/uploads/2018/08/pengertian-apache2-dan-konfigurasi.png)

***

## Apa Itu Web Server? ##
Web server adalah perangkat lunak atau perangkat keras yang menyediakan layanan untuk mengakses halaman web atau konten web melalui internet. Fungsi utama dari web server adalah melayani permintaan dari klien (biasanya browser web) dengan menyediakan halaman web yang diminta. Ketika seseorang mengakses situs web melalui browser mereka, permintaan dikirim ke web server, dan web server ini kemudian mengirimkan halaman web tersebut kembali ke browser pengguna. Untuk contoh dari penggunaannya adalah sebagai berikut :

![Screenshot 2023-12-23 110152](https://github.com/alvingg666/FP/assets/148695999/d803f33a-00af-4490-b01b-b1623b169034)





## OS Server ##
Ubuntu 22.04
***


## Service Yang Digunakan ##
1. SSH 
2. Apache2
3. Ngrok
***
## Step Pengerjaan #
1.** Install Apache2 **
sudo apt install apache2

2.** Cek status **
sudo systemctl status apache2

3.** Cek hostname **
hostname -I

4.**  Ubah pemilik folder **
sudo chown -R www-data:www-data /var/www/html

5.** Beri ijin anggota grup untuk merubah folder **
sudo chmod -R g+rw /var/www/html

6.** Tambahkan user name kita **
sudo usermod -a -G www-data

7.** Restart ubuntu **

8.** Tambahkan rule untuk apache difirewall **
sudo ufw allow 'Apache'

9.** Cek status firewall **
sudo ufw status

10.** Install ssh **
sudo apt install openssh-server

11.** Install ngrok **
snap install ngrok

12.** Masukkan token authtoken **
ngrok config add-authtoken 2ZlR0DFXPuzK2a1nMQY6ONP1FLn_4oDZYTuGDNHW3jJPJHT5R

13.** Masuk cmd ketikkan **
ssh "username"@"ip ubuntu"

14.** http 80 untuk mendapatkan url ***
ngrok http 80

15.** Untuk mengedit index.html **
masuk folder /var/www/html open menggunakan texteditor 



