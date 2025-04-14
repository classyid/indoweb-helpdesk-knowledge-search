# Solusi Pencarian Indoweb

![Logo Indoweb](https://indoweb.id/wp-content/uploads/2022/12/logo-idw-fix.png)

## Deskripsi

Solusi Pencarian Indoweb adalah sistem pencarian terpadu untuk helpdesk yang memungkinkan pengguna mencari solusi dari berbagai sumber termasuk tiket support, knowledge base, dan FAQ. Sistem ini dirancang untuk memudahkan staf support dan pengguna dalam menemukan informasi yang diperlukan dengan cepat dan efisien.

## Fitur Utama

- 🔍 **Pencarian Terpadu**: Mencari di semua sumber data (tiket, knowledge base, FAQ) sekaligus
- 🎯 **Filter Berdasarkan Kategori**: Memfokuskan pencarian pada tipe konten tertentu
- 🧩 **Tampilan Detail yang Komprehensif**: Melihat seluruh informasi tiket, artikel, dan FAQ
- 📱 **Responsive Design**: Tampilan yang menyesuaikan dengan berbagai ukuran layar
- 📤 **Berbagi Konten**: Membagikan artikel dan FAQ ke media sosial
- 👍 **Feedback Pengguna**: Menilai kegunaan artikel knowledge base

## Teknologi

- **Backend**: PHP 7.4+, MySQL 5.7+
- **Frontend**: HTML5, CSS3, JavaScript, Tailwind CSS
- **Icons**: Font Awesome
- **Fonts**: Inter (Google Fonts)

## Struktur Sistem

Sistem terdiri dari beberapa komponen utama:

1. **Halaman Utama (index.php)**: Form pencarian dan tampilan hasil
2. **API Pencarian (cari.php)**: Endpoint untuk pencarian yang mengembalikan hasil dalam format JSON
3. **Halaman Detail**:
   - **ticket_detail.php**: Menampilkan detail tiket support
   - **faq_detail.php**: Menampilkan detail FAQ
   - **knowledge_detail.php**: Menampilkan detail artikel knowledge base

## Instalasi

1. Clone repository ini:
   ```
   git clone https://github.com/classyid/indoweb-helpdesk-knowledge-search.git
   ```

2. Import struktur database dari file `database.sql` ke MySQL/MariaDB Anda:
   ```
   mysql -u username -p database_name < database.sql
   ```

3. Konfigurasi koneksi database di setiap file PHP (`cari.php`, `ticket_detail.php`, `faq_detail.php`, `knowledge_detail.php`).

4. Salin file ke server web Anda atau jalankan server lokal:
   ```
   php -S localhost:8000
   ```

5. Akses aplikasi melalui browser (misalnya http://localhost:8000).

## Konfigurasi

Beberapa parameter yang dapat dikonfigurasi:

- Koneksi database (host, username, password, nama database)
- Jumlah hasil pencarian per halaman
- Path upload untuk file lampiran

## Penggunaan

1. Pada halaman utama, masukkan kata kunci di kotak pencarian
2. Secara opsional, pilih kategori untuk memfilter hasil (Tiket Support, Knowledge Base, FAQ)
3. Klik tombol "Cari" atau tekan Enter
4. Lihat hasil pencarian yang ditampilkan
5. Klik pada hasil untuk melihat detail lengkap

## Keamanan

**Penting:** Sebelum men-deploy ke produksi:

1. Ubah kredensial database default
2. Pastikan direktori upload file memiliki izin yang tepat
3. Pertimbangkan untuk menerapkan HTTPS
4. Tambahkan validasi input dan sanitasi untuk semua data yang diterima dari pengguna

## Kontribusi

Kontribusi sangat diterima! Jika Anda ingin berkontribusi pada proyek ini:

1. Fork repository
2. Buat branch fitur (`git checkout -b feature/fitur-baru`)
3. Commit perubahan Anda (`git commit -m 'Menambahkan fitur X'`)
4. Push ke branch (`git push origin feature/fitur-baru`)
5. Buat Pull Request

## Lisensi

[MIT License](LICENSE)

## Kontak

Untuk pertanyaan atau dukungan, hubungi [info@indoweb.id](mailto:info@indoweb.id)
