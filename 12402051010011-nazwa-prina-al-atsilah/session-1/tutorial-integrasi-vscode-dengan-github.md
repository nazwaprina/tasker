# Tutorial Mengintegrasikan VS Code dengan GitHub
## Step 1: Install VS Code Terlebih Dahulu
### Buka Website Resmi VS Code untuk Melihat Instruksinya
Klik link ini: http://code.visualstudio.com/docs/setup/linux
 <img width="778" height="299" alt="image" src="https://github.com/user-attachments/assets/a1a72daa-66a0-49f6-b6d6-1dfdb84a00f3" />

### Update Sistem 
```
sudo apt update
```
<img width="577" height="211" alt="image" src="https://github.com/user-attachments/assets/fe95c581-d5c8-4acf-a45c-c2abea57ed78" />

### Install Paket Prasyarat
```
sudo apt install software-properties-common apt-transport-https wget -y

```
<img width="973" height="372" alt="image" src="https://github.com/user-attachments/assets/a11d01cf-0d81-4244-a3b3-249b0bd2b2b3" />

### Unduh dan Tambahkan Kunci GPG Microsoft
```
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -

```
<img width="1034" height="52" alt="image" src="https://github.com/user-attachments/assets/749af8e6-3c68-4005-8318-4cbb08d62d92" />

### Tambahkan Repository VS Code
```
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
```
<img width="1178" height="36" alt="image" src="https://github.com/user-attachments/assets/8648c420-82de-4537-97cb-246412f7ee10" />

### Perbarui indeks paket lagi setelah menambahkan repositori baru:
```
sudo apt update
```
<img width="675" height="239" alt="image" src="https://github.com/user-attachments/assets/550ea3a8-d708-4816-895e-0c6fb1184f57" />

### Install VS Code
```
sudo apt install code
```
<img width="853" height="379" alt="image" src="https://github.com/user-attachments/assets/e6e927f8-d0d9-419d-b0c5-201ddc8d854d" />

Setelah instalasi selesai, VS Code bisa diluncurkan dari menu aplikasi.

## Step 2: Meng-install Git
```
sudo apt-get install git
```
<img width="839" height="510" alt="image" src="https://github.com/user-attachments/assets/9305d767-f38a-409e-8838-b97a1e549e12" />

### Pastikan Git Sudah Ter-Install
```
git --version
```
<img width="496" height="35" alt="image" src="https://github.com/user-attachments/assets/fb5d3b47-7ee4-4029-9c3b-dff313a037e5" />

Jika Git sudah terinstal dengan benar, akan muncul informasi versi Git yang terpasang di komputer.
## Step 3: Konfigurasi Git Awal
Sebelum mulai, beri tahu Git Nama dan Email yang akan digunakan. Hal ini cuma perlu dilakukan sekali saja.
Buka Terminal/Git Bash, lalu ketik perintah berikut, ganti Nama dan email@example.com dengan nama dan email GitHub yang akan digunakan.
```
git config --global user.name "Nama"
git config --global user.email "emailexample.com"
```
<img width="657" height="73" alt="image" src="https://github.com/user-attachments/assets/7a489a52-efc0-4300-a37c-416000c506e9" />

## Step 4: Mengambil Proyek dari GitHub
* Buka GitHub: Pergi ke halaman repositori yang sudah dibuat.
* Salin URL: Klik tombol hijau < > Code, lalu salin URL HTTPS-nya.
* Buka Terminal/Git Bash: Buka terminal di folder tempat yang akandigunakan untuk menyimpan proyek.
* Jalankan Perintah clone: Ketik git clone diikuti dengan URL yang sudah sudah disalin tadi.
```
git clone https://github.com/nama-kamu/nama-proyek.git
```
<img width="653" height="194" alt="image" src="https://github.com/user-attachments/assets/9083fbc5-6b9c-45ae-a7bc-0f54f14e4225" />

## Step 5: Buka Proyek di VS Code dan Mulai Mengerjakan
Setelah proyek di-clone, kita bisa mulai mengerjakan tugas dokumentasi di VS Code.
 * Buka VS Code.
 * Pilih File > Open Folder... dan navigasi ke folder proyek yang baru saja di-clone.
 * Di dalam VS Code, buat file-file dokumentasinya (misalnya, README.md) dan mulai tulis isinya.
   
<img width="393" height="293" alt="image" src="https://github.com/user-attachments/assets/4c43f59c-87db-4038-b57c-292fa5a9954e" />
<img width="732" height="449" alt="image" src="https://github.com/user-attachments/assets/76fb0554-d9c7-4f7c-af31-38484b525c1c" />

Kita bisa menulis kode, dokumentasi, dan nanti mengunggahnya ke GitHub, semuanya bisa dilakukan dari dalam VS Code.
