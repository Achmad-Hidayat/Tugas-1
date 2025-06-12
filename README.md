# Tugas-1

####ETL-WEEKDATE-TASK
WEEKDATE TASK BUSINESS INSIGHT CONCEPT RELATED ENVIRONMENTAL ENERGI TERBARUKAN

Soal Ujian Proyek: Sistem Pengelolaan UMKM, Koperasi, dan Bank Sampah 🌟 Halo peserta ujian! Selamat datang di proyek ujian Sistem Pengelolaan UMKM, Koperasi, dan Bank Sampah yang disusun oleh Arry Hutomo, Founder Komunitas Nawala Integra Nusantara, bersama tim PT Engineering Career Centre (ECC). Proyek ini adalah bagian dari pelatihan ETL Batch 9 & 10 untuk menguji kemampuan kalian dalam menerapkan konsep Python dari Chapter 1 hingga Chapter 15 yang sudah kita pelajari bersama. Yuk, kita wujudkan solusi yang bermanfaat untuk masyarakat dengan pendekatan yang asik dan elegan! 🚀

Narasi Kasus: Nawala Integra Nusantara dan PT ECC untuk UMKM dan Lingkungan Komunitas Nawala Integra Nusantara, yang dipimpin oleh Arry Hutomo, bekerja sama dengan PT Engineering Career Centre (ECC), sedang menjalankan program pemberdayaan masyarakat melalui pengembangan UMKM (Usaha Mikro, Kecil, dan Menengah), koperasi, dan bank sampah di desa-desa. Program ini bertujuan untuk:

Mendukung UMKM: Membantu UMKM lokal dengan sistem manajemen yang efisien untuk melacak data anggota, pinjaman, dan pengembalian dana. Mengelola Koperasi: Mempermudah pengelolaan koperasi desa dengan mencatat transaksi dan menghitung keuntungan anggota. Bank Sampah: Mendorong kesadaran lingkungan dengan sistem bank sampah yang mencatat data sampah, menghitung nilai tukar, dan memberikan edukasi kepada masyarakat.

Arry Hutomo, sebagai penderma utama, menyediakan dana pinjaman awal sebesar Rp50 juta untuk setiap UMKM dan koperasi yang bergabung, dengan syarat mereka juga aktif dalam program bank sampah. Sistem ini akan membantu mengelola data anggota, pinjaman, transaksi, dan aktivitas bank sampah, sekaligus memberikan laporan edukasi untuk meningkatkan kesadaran masyarakat tentang pentingnya keberlanjutan lingkungan.

Latar Belakang Kasus Kenapa kita pilih tema UMKM, Pengelolaan Koperasi, dan Bank Sampah? Di Indonesia, UMKM adalah tulang punggung ekonomi, menyumbang lebih dari 60% PDB nasional dan menyerap 97% tenaga kerja. Namun, banyak UMKM di desa kesulitan mengelola keuangan dan mengakses dana. Koperasi desa sering kali kurang terorganisir dalam mencatat transaksi, sehingga sulit menghitung keuntungan anggota secara adil. Sementara itu, masalah sampah di desa semakin parah—sampah plastik sering mencemari sungai dan pesisir, mengancam ekosistem seperti mangrove. Program ini dirancang untuk memberdayakan masyarakat desa dengan solusi teknologi sederhana namun berdampak besar. Dengan sistem Python, kita bisa membantu UMKM dan koperasi mengelola data mereka secara efisien, sekaligus mendorong kesadaran lingkungan melalui bank sampah. Arry Hutomo dan tim PT ECC percaya bahwa teknologi bisa menjadi jembatan untuk keberlanjutan ekonomi dan lingkungan, dan kalian, sebagai peserta ujian, akan menjadi bagian dari misi ini! 🌍

Daftar Pertanyaan Query untuk Proyek Proyek ini akan dibangun langkah demi langkah melalui serangkaian query. Setiap query memiliki narasi yang menjelaskan apa yang harus dilakukan. Gunakan konsep dari Chapter 1 hingga Chapter 15 untuk menyelesaikan proyek ini. Query 1: Membuat Class untuk Sistem UMKM Kita mulai dengan membuat class UMKMSystem yang akan menjadi inti dari sistem ini. Class ini akan menyimpan data dasar seperti nama UMKM, data anggota, dan dana pinjaman awal dari Arry Hutomo.

Tugas: Buat class UMKMSystem dengan atribut nama_umkm, anggota (list kosong untuk menyimpan data anggota), dan dana_pinjaman (set sebagai Rp50 juta). Gunakan konsep OOP (Chapter 15) dan variables (Chapter 1).

Query 2: Method untuk Menambah Anggota UMKM Setiap UMKM punya anggota yang akan menerima pinjaman. Kita perlu method untuk menambah anggota ke dalam sistem.

Tugas: Tambahkan method tambah_anggota ke class UMKMSystem. Method ini akan menerima input nama anggota dan jumlah pinjaman (dalam rupiah), lalu menyimpannya sebagai dictionary dalam list anggota. Gunakan konsep list (Chapter 8) dan dictionary (Chapter 11).

Query 3: Method untuk Menghitung Pengembalian Pinjaman Setiap anggota harus mengembalikan pinjaman dengan bunga sederhana 5% per tahun. Kita perlu method untuk menghitung total pengembalian.

Tugas: Tambahkan method hitung_pengembalian ke class UMKMSystem. Method ini menerima nama anggota dan tahun pengembalian, lalu menghitung total pengembalian (pinjaman + bunga). Gunakan konsep operators (Chapter 3).

Query 4: Membuat Class untuk Koperasi Selain UMKM, kita perlu class untuk mengelola koperasi desa yang akan mencatat transaksi anggota.

Tugas: Buat class Koperasi yang mewarisi class UMKMSystem. Class ini akan memiliki atribut tambahan transaksi (list kosong untuk menyimpan transaksi). Gunakan konsep inheritance (Chapter 15).

Query 5: Method untuk Mencatat Transaksi Koperasi Koperasi akan mencatat transaksi setiap anggota, seperti pembelian barang atau pembayaran pinjaman.

Tugas: Tambahkan method catat_transaksi ke class Koperasi. Method ini menerima nama anggota, jenis transaksi (beli/jual), dan jumlah (dalam rupiah), lalu menyimpannya sebagai dictionary dalam list transaksi. Gunakan konsep dictionary (Chapter 11) dan list (Chapter 8).

Query 6: Method untuk Menghitung Keuntungan Koperasi Koperasi akan menghitung keuntungan berdasarkan transaksi anggota.

Tugas: Tambahkan method hitung_keuntungan ke class Koperasi. Method ini menghitung total keuntungan dari transaksi (jual - beli). Gunakan konsep for loops (Chapter 6) dan operators (Chapter 3).

Query 7: Membuat Class untuk Bank Sampah Bank sampah akan mencatat data sampah yang dikumpulkan oleh anggota dan memberikan nilai tukar dalam rupiah.

Tugas: Buat class BankSampah yang mewarisi class UMKMSystem. Class ini memiliki atribut tambahan data_sampah (dictionary untuk menyimpan data sampah dan nilai tukar per kg). Gunakan konsep inheritance (Chapter 15) dan dictionary (Chapter 11).

Query 8: Method untuk Mencatat Data Sampah Bank sampah akan mencatat jenis sampah dan jumlah yang dikumpulkan oleh anggota.

Tugas: Tambahkan method catat_sampah ke class BankSampah. Method ini menerima nama anggota, jenis sampah, dan jumlah (dalam kg), lalu menyimpannya ke dalam dictionary data_sampah. Gunakan konsep dictionary (Chapter 11).

Query 9: Method untuk Menghitung Nilai Tukar Sampah Bank sampah akan menghitung nilai tukar sampah dalam rupiah berdasarkan jumlah yang dikumpulkan.

Tugas: Tambahkan method hitung_nilai_tukar ke class BankSampah. Method ini menghitung nilai tukar berdasarkan data sampah (misalnya, plastik Rp5000/kg, kertas Rp2000/kg). Gunakan konsep operators (Chapter 3) dan dictionary (Chapter 11).

Query 10: Method untuk Pesan Edukasi Lingkungan Sistem ini juga akan memberikan pesan edukasi kepada masyarakat tentang pentingnya daur ulang.

Tugas: Tambahkan method pesan_edukasi ke class BankSampah. Method ini memberikan pesan berbeda berdasarkan total sampah yang dikumpulkan (gunakan kondisi if-elif-else). Gunakan konsep if...elif...else (Chapter 5) dan strings (Chapter 4).

Query 11: Mengintegrasikan Semua Komponen Terakhir, kita integrasikan semua class ke dalam sistem utama dengan input dari user untuk menjalankan simulasi.

Tugas: Buat program utama yang: Membuat objek dari class Koperasi dan BankSampah. Meminta input user untuk nama UMKM, data anggota, transaksi koperasi, dan data sampah. Menampilkan laporan lengkap (pinjaman, transaksi, keuntungan, nilai tukar sampah, dan pesan edukasi).Gunakan konsep input (Chapter 4), loops (Chapter 6), dan OOP (Chapter 15).

Petunjuk Pengerjaan Kalian memiliki waktu 1 minggu untuk menyelesaikan proyek ini, mulai dari 26 Mei 2025 hingga 5 June 2025. Berikut adalah langkah-langkah pengerjaan:

Persiapan Alat

Gunakan VS Code sebagai text editor. Download di code.visualstudio.com jika belum punya. Pastikan Python 3.9.13 terinstall di laptop kalian. Download dari python.org dan pastikan sudah ditambahkan ke PATH (cek dengan python --version di command prompt).

Pengerjaan Proyek

Buat file Python bernama umkm_koperasi_banksampah.py di VS Code. Salin kode dari jawaban kalian (yang akan kalian buat di jawaban.html) ke file tersebut. Jalankan kode di VS Code menggunakan terminal (tekan Ctrl+, lalu ketik python umkm_koperasi_banksampah.py`). Pastikan hasil output di command prompt sesuai dengan yang diminta di soal.

Format Jawaban

Buat file HTML bernama jawaban.html yang berisi kode lengkap kalian, penjelasan langkah demi langkah, dan contoh output (mirip seperti format proyek sebelumnya). Sertakan narasi untuk setiap query yang kalian kerjakan, termasuk do and don'ts. Tambahkan contoh output di command prompt untuk setiap langkah.

Pengumpulan

Simpan proyek kalian di repository GitHub bernama umkm-koperasi-banksampah-exam. Aktifkan GitHub Pages untuk repository kalian (Settings > Pages > Pilih branch main dan folder /(root)). Kirimkan link GitHub Pages ke email ETL.BATCH9@ecc.co.id (jika kalian Batch 9) atau ETL.BATCH10@ecc.co.id (jika kalian Batch 10) sebelum tenggat waktu 05 JUNE 2025, pukul 23:59 WIB. Subjek email: [ETL Batch 9/10] Ujian Proyek - Nama Lengkap - Nomor Peserta. Contoh: [ETL Batch 9] Ujian Proyek - Budi Santoso - 009.

Motivasi dan Doa "Setiap baris kode yang kalian tulis adalah langkah menuju perubahan besar untuk UMKM dan lingkungan. Bersyukurlah kepada Tuhan atas kemampuan untuk berkarya dan memberi manfaat! 🌟" "Ya Tuhan, kuatkan hati kami dalam menyelesaikan proyek ini. Berikan kami ketekunan dan keikhlasan untuk terus belajar demi masa depan yang lebih baik. Aamiin." Selamat mengerjakan, dan semoga sukses! 🚀Dibuat oleh Arry Hutomo - Nawala Integra Nusantara & PT ECC.
