# Dokumentasi Proyek

## Setup dan Penggunaan

### Persiapan Proyek

1. **Instalasi Dependensi**

   Pastikan semua dependensi proyek telah diinstal dengan menjalankan:

   ```bash
   npm install
   ```

1. **Migrasi**
   Untuk menerapkan migrasi dan membuat tabel di database, gunakan perintah berikut:

```bash
npx sequelize-cli db:migrate --config src/config/config.js --migrations-path src/migrations
```

Seeder
Untuk memasukkan data awal ke dalam tabel (seeding), jalankan perintah berikut:

```bash
npx sequelize-cli db:seed:all --config src/config/config.js --seeders-path src/seeders
```

Rollback Semua Migrasi
Untuk membatalkan semua migrasi yang diterapkan, jalankan:

```bash
npx sequelize-cli db:migrate:undo:all --config src/config/config.js --migrations-path src/migrations
```

Hapus Seeder
Jika Anda perlu menghapus data yang telah di-seed, gunakan perintah ini:

```bash
npx sequelize-cli db:seed:undo:all --config src/config/config.js --seeders-path src/seeders
```
