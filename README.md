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



<title>Jawaban Proyek Ujian - UMKM, Koperasi, dan Bank Sampah</title> <style> body { font-family: Arial, sans-serif; padding: 30px; background-color: #ffffff; } h1, h2, h3 { color: #333; } pre { background-color: #eee; padding: 10px; border-left: 4px solid #008080; overflow-x: auto; } code { font-family: "Courier New", Courier, monospace; } .output { background: #000; color: #0f0; padding: 10px; margin-top: 10px; white-space: pre-wrap; } .section { margin-bottom: 40px; } </style>
Jawaban Proyek Ujian - UMKM, Koperasi, dan Bank Sampah
Nama Peserta: Farhan Fadillah

Batch: ETL Batch 9

No. Absen: 9.008.DB2025

Judul Proyek: Sistem Pengelolaan UMKM, Koperasi, dan Bank Sampah

<div class="section">
    <h2>📘 Pendahuluan</h2>
    <p>Proyek ini bertujuan membangun sistem manajemen sederhana menggunakan Python untuk membantu UMKM, koperasi desa, dan bank sampah agar lebih efisien dan berkelanjutan. Kami menggunakan konsep OOP, dictionary, list, loops, dan berbagai tools dari Chapter 1–15.</p>
</div>

<div class="section">
    <h2>Langkah-Langkah Penyelesaian</h2>

    <h3>Query 1: Class UMKMSystem</h3>
    <pre><code>class UMKMSystem:
def __init__(self, nama_umkm):
    self.nama_umkm = nama_umkm
    self.anggota = []
    self.dana_pinjaman = 50000000</code></pre>
    <p><strong>Penjelasan:</strong> Class ini adalah dasar dari sistem, menyimpan nama UMKM, daftar anggota, dan total dana pinjaman awal sebesar 50 juta rupiah.</p>

    <h3>Query 2: Method tambah_anggota</h3>
    <pre><code>def tambah_anggota(self, nama_anggota, jumlah_pinjaman):
self.anggota.append({
    "nama": nama_anggota,
    "pinjaman": jumlah_pinjaman
})</code></pre>
<p><strong>Penjelasan:</strong> Method ini menambahkan anggota baru ke dalam daftar, lengkap dengan nama dan jumlah pinjaman yang diajukan.</p>

    <h3>Query 3: Method Menghitung Pengembalian Pinjaman</h3>
    <pre><code>def hitung_pengembalian(self, nama_anggota, tahun):
for anggota in self.anggota:
    if anggota["nama"] == nama_anggota:
        bunga = 0.05 * tahun * anggota["pinjaman"]
        return anggota["pinjaman"] + bunga
return "Anggota tidak ditemukan."</code></pre>
<p><strong>Penjelasan:</strong> Fungsi ini menghitung jumlah pengembalian pinjaman setelah periode tertentu, termasuk bunga 5% per tahun.</p>

    <h3>Query 4: Class Koperasi</h3>
    <pre><code>class Koperasi(UMKMSystem):
def __init__(self, nama_umkm):
    super().__init__(nama_umkm)
    self.transaksi = []</code></pre>
    <p><strong>Penjelasan:</strong> Kelas ini mewarisi UMKMSystem dan menambahkan fitur pencatatan transaksi jual dan beli untuk koperasi.</p>

    <h3>Query 5: Method catat_transaksi</h3>
    <pre><code>def catat_transaksi(self, nama_anggota, jenis, jumlah):
self.transaksi.append({
    "nama": nama_anggota,
    "jenis": jenis,
    "jumlah": jumlah
})</code></pre>
<p><strong>Penjelasan:</strong> Method ini menyimpan data transaksi anggota berdasarkan nama, jenis (jual/beli), dan jumlahnya.</p>

    <h3>Query 6: Method hitung_keuntungan</h3>
    <pre><code>def hitung_keuntungan(self):
total_jual = sum(t["jumlah"] for t in self.transaksi if t["jenis"] == "jual")
total_beli = sum(t["jumlah"] for t in self.transaksi if t["jenis"] == "beli")
return total_jual - total_beli</code></pre>
<p><strong>Penjelasan:</strong> Fungsi ini menghitung total keuntungan koperasi dari selisih penjualan dan pembelian seluruh transaksi.</p>

    <h3>Query 7: Class BankSampah</h3>
    <pre><code>class BankSampah(UMKMSystem):
def __init__(self, nama_umkm):
    super().__init__(nama_umkm)
    self.data_sampah = {}</code></pre>
    <p><strong>Penjelasan:</strong> Kelas ini memperluas UMKMSystem dengan kemampuan menyimpan data jenis dan jumlah sampah dari tiap anggota.</p>

    <h3>Query 8: Method catat_sampah</h3>
    <pre><code>def catat_sampah(self, nama_anggota, jenis_sampah, jumlah_kg):
if nama_anggota not in self.data_sampah:
    self.data_sampah[nama_anggota] = []
self.data_sampah[nama_anggota].append({
    "jenis": jenis_sampah,
    "jumlah": jumlah_kg
})</code></pre>
<p><strong>Penjelasan:</strong> Fungsi ini mencatat jenis dan berat sampah (dalam kg) yang disetorkan oleh setiap anggota.</p>

    <h3>Query 9: Method hitung_nilai_tukar</h3>
    <pre><code>def hitung_nilai_tukar(self, nama_anggota):
harga = {"plastik": 5000, "kertas": 2000, "logam": 8000}
total = 0
for item in self.data_sampah.get(nama_anggota, []):
    total += item["jumlah"] * harga.get(item["jenis"], 0)
return total</code></pre>
<p><strong>Penjelasan:</strong> Fungsi ini mengubah jumlah sampah menjadi nilai uang berdasarkan jenisnya (misalnya plastik = 5.000/kg).</p>

    <h3>Query 10: Method pesan_edukasi</h3>
    <pre><code>def pesan_edukasi(self, nama_anggota):
total = sum(item["jumlah"] for item in self.data_sampah.get(nama_anggota, []))
if total > 100:
    return "Luar biasa! Anda adalah pahlawan lingkungan desa!"
elif total > 50:
    return "Kerja bagus! Terus tingkatkan kontribusi Anda!"
elif total > 0:
    return "Terima kasih telah berkontribusi, mari kumpulkan lebih banyak!"
else:
    return "Ayo mulai kumpulkan sampah dan jaga lingkungan kita!"</code></pre>
 <p><strong>Penjelasan:</strong> Memberikan pesan motivasi berdasarkan jumlah sampah yang dikumpulkan. Semakin banyak, semakin positif pesannya.</p>

    <h3>Query 11: Program Utama</h3>
    <pre><code>if __name__ == "__main__":
nama_umkm = input("Masukkan nama UMKM: ")
koperasi = Koperasi(nama_umkm)
bank_sampah = BankSampah(nama_umkm)

# Tambah anggota
while True:
    nama = input("Nama anggota (atau 'selesai'): ")
    if nama.lower() == 'selesai':
        break
    pinjaman = int(input(f"Jumlah pinjaman untuk {nama}: "))
    koperasi.tambah_anggota(nama, pinjaman)
    bank_sampah.tambah_anggota(nama, pinjaman)

# Tambah transaksi
while True:
    nama = input("Nama anggota transaksi (atau 'selesai'): ")
    if nama.lower() == 'selesai':
        break
    jenis = input("Jenis transaksi (beli/jual): ")
    jumlah = int(input("Jumlah transaksi (Rp): "))
    koperasi.catat_transaksi(nama, jenis, jumlah)

# Catat sampah
while True:
    nama = input("Nama anggota sampah (atau 'selesai'): ")
    if nama.lower() == 'selesai':
        break
    jenis_sampah = input("Jenis sampah: ")
    jumlah_kg = float(input("Jumlah (kg): "))
    bank_sampah.catat_sampah(nama, jenis_sampah, jumlah_kg)

# Output
for anggota in koperasi.anggota:
    nama = anggota["nama"]
    pinjaman = anggota["pinjaman"]
    pengembalian = koperasi.hitung_pengembalian(nama, 1)
    nilai_sampah = bank_sampah.hitung_nilai_tukar(nama)
    pesan = bank_sampah.pesan_edukasi(nama)

    print(f"\nNama: {nama}")
    print(f"Pinjaman: Rp{pinjaman}")
    print(f"Pengembalian: Rp{int(pengembalian)}")
    print(f"Nilai Tukar Sampah: Rp{nilai_sampah}")
    print(f"Pesan Edukasi: {pesan}")

print(f"\nTotal Keuntungan Koperasi: Rp{koperasi.hitung_keuntungan()}")</code></pre>
<p><strong>Penjelasan:</strong> Program utama akan menjalankan seluruh alur — input data, simpan, dan menampilkan output. Semua kelas dan method sebelumnya digunakan di sini.</p>
</div>

<div class="section">
    <h2>🖥️ Contoh Output Terminal</h2>
    <div class="output">
UMKM: Tani Maju Anggota: Budi Pinjaman: 1000000 Pengembalian (1 tahun): Rp1050000 Nilai Tukar Sampah: Rp30000 Pesan Edukasi: Terima kasih telah berkontribusi, mari kumpulkan lebih banyak!

Total Keuntungan Koperasi: Rp250000

<div class="section">
    <h2>📌 Catatan & Pembelajaran</h2>
    <p>Saya belajar bagaimana mengintegrasikan banyak konsep Python menjadi satu sistem terstruktur. Tantangan utama adalah menjaga agar data antar class tetap sinkron. Dengan sistem ini, saya merasa lebih siap membangun solusi nyata untuk masyarakat.</p>
</div>

<div class="section">
    <h2>🚫 Do’s & Don’ts</h2>
    <ul>
        <li>✅ Gunakan inheritance untuk menghindari duplikasi kode.</li>
        <li>✅ Gunakan dictionary untuk fleksibilitas penyimpanan data.</li>
        <li>❌ Jangan lupa konversi input dari `str` ke `int/float` sebelum perhitungan.</li>
        <li>❌ Jangan hardcode data — selalu gunakan input atau variable.</li>
    </ul>
</div>
<div class="section" style="margin-top: 40px;">
<button onclick="window.open('https://etl-task-bank-sampah-farhan.streamlit.app/', '_blank')" 
    style="padding: 10px 20px; background-color: #008080; color: white; border: none; border-radius: 5px; cursor: pointer;">
    Buka Aplikasi
</button>
</div>
