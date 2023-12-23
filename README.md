#   Web Server #
Tugas yang di buat pada final project kali ini adalah menginstall apache2
![Picsart_23-11-30_18-42-27-335](https://kitaadmin.com/wp-content/uploads/2018/08/pengertian-apache2-dan-konfigurasi.png)

***

## Apa Itu Web Server? ##
Web server adalah perangkat lunak atau perangkat keras yang menyediakan layanan untuk mengakses halaman web atau konten web melalui internet. Fungsi utama dari web server adalah melayani permintaan dari klien (biasanya browser web) dengan menyediakan halaman web yang diminta. Ketika seseorang mengakses situs web melalui browser mereka, permintaan dikirim ke web server, dan web server ini kemudian mengirimkan halaman web tersebut kembali ke browser pengguna. Untuk contoh dari penggunaannya adalah sebagai berikut :

![image](https://github.com/alvingg666/FP/assets/148695999/d5a862af-9476-4a12-9e43-39a75f67b225)


## OS Server ##
Ubuntu 22.04
***


## Service Yang Digunakan ##
1. SSH 
2. Apache2
3. Ngrok
***
## Step Pengerjaan #
** Install Apache2 **
sudo apt install apache2
** Cek status **
sudo systemctl status apache2
** Cek hostname **
hostname -I
**  Ubah pemilik folder **
sudo chown -R www-data:www-data /var/www/html
** Beri ijin anggota grup untuk merubah folder **
sudo chmod -R g+rw /var/www/html
** Tambahkan user name kita **
sudo usermod -a -G www-data
** Restart ubuntu **
** Tambahkan rule untuk apache difirewall **
sudo ufw allow 'Apache'
** Cek status firewall **
sudo ufw status
** Install ssh **
sudo apt install openssh-server
** Install ngrok **
snap install ngrok
** Masukkan token authtoken **
ngrok config add-authtoken 2ZlR0DFXPuzK2a1nMQY6ONP1FLn_4oDZYTuGDNHW3jJPJHT5R
** Masuk cmd ketikkan **
ssh "username"@"ip ubuntu"
** http 80 untuk mendapatkan url ***
ngrok http 80
** Untuk mengedit index.html **
masuk folder /var/www/html open menggunakan texteditor 



