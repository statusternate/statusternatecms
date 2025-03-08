// README.md placeholder for Statuters CMS

✅ Persyaratan Awal
Pastikan environment berikut sudah tersedia di komputer/server Anda:

PHP (minimal versi 8.1)
Composer
MySQL atau MariaDB
Git (opsional)
🚀 Langkah Instalasi
1. Unduh Statuters CMS
Jika tersedia di GitHub, jalankan perintah berikut:


git clone https://github.com/statuterscms/statuterscms.git
cd statuterscms
Jika tersedia dalam bentuk ZIP:

Download file ZIP dan ekstrak di direktori kerja Anda.
Buka folder hasil ekstrak tersebut.
2. Instalasi Dependensi
Gunakan Composer untuk menginstal dependensi PHP:


composer install
3. Konfigurasi Database
Buat database baru di MySQL/MariaDB, misalnya dengan nama statuterscms.

sql

CREATE DATABASE statuterscms;
Salin file .env.example menjadi .env:


cp .env.example .env
Ubah konfigurasi database di file .env tersebut:

dotenv

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=statuterscms
DB_USERNAME=root
DB_PASSWORD=password_anda
4. Generate App Key
Generate kunci aplikasi untuk keamanan:

bash
t
php artisan key:generate
5. Migrasi Database & Seed (Opsional)
Jalankan migrasi database:


php artisan migrate
Opsional, jika tersedia seeder:



php artisan db:seed
6. Konfigurasi Storage & Cache
Atur permission direktori:

t
chmod -R 775 storage bootstrap/cache
7. Menjalankan Aplikasi
Jalankan Statuters CMS dengan command berikut:



php artisan serve
Buka browser Anda, akses URL:


http://127.0.0.1:8000
🛠️ Informasi Default (jika ada)
Username default: admin
Password default: password (Ubah setelah login)

✅ Selesai!
Statuters CMS berhasil terinstal, Anda dapat mulai mengelola konten blog Anda.

Jika menemukan kesulitan, beri tahu agar bisa saya bantu lebih lanjut. 🚀

se you salam satu ternate
