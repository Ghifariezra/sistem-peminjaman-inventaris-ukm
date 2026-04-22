# 📦 Topik Proyek: Sistem Inventaris UKM
## 👥 Anggota Kelompok 9
| **Nama** | **NPM** |
| ------------- | ------------- |
| Dheka Airlangga | 4524210027 |
| Naila Putri Fahel | 4524210053 |
| Maghfiroh | 4524210040 |
| Az-Zahra Putri| 4524210018 |
| Ghifari Ezra Ramadhan | 4524210041 |

# 🚨 Masalah
[Deskripsikan kendala atau masalah utama yang saat ini dihadapi oleh UKM dalam mengelola pencatatan dan pelacakan barang inventaris mereka di sini...]

# 🔍 Analisis
**1. Aktor**
[Tuliskan ...] 

## Bagian 2: Analisis Perbandingan SOP (Sebelum dan Sesudah Implementasi Sistem)
Bagian ini menguraikan transformasi prosedur operasional (SOP) pengelolaan inventaris UKM dari sistem pencatatan manual menjadi sistem informasi berbasis aplikasi. Perubahan ini bertujuan untuk menyelesaikan masalah pendataan dan meningkatkan efisiensi, transparansi, serta akurasi data.

### 1. Pencatatan & Data Masuk (Input Barang Baru)
* **SOP Saat Ini (Manual):** Pencatatan barang masih bergantung pada pengumpulan struk fisik yang diserahkan ke Bendahara. Tidak ada sistem kodifikasi/nomor seri pada barang, dan *database* (Microsoft Excel) hanya digunakan untuk mendata aset-aset berukuran besar, sementara barang kecil tidak terdata secara digital.
* **SOP Usulan (Sistem Aplikasi):**
  * **Digitalisasi Data:** Semua barang (besar maupun kecil) langsung diinput ke dalam *database* sistem.
  * **Auto-Generate ID:** Sistem akan otomatis membuatkan kode unik (ID Barang/Barcode) untuk setiap entri baru sehingga pelabelan lebih terstandar.
  * **Integrasi Berkas:** Struk pembelian dapat difoto dan diunggah langsung ke sistem, sehingga Bendahara dapat mengaksesnya secara *real-time* tanpa perlu serah terima kertas fisik.

### 2. Peminjaman (Alur Keluar Barang)
* **SOP Saat Ini (Manual):** Peminjam (eksternal) harus mengirim surat fisik/PDF, lalu pengurus mengecek ketersediaan barang secara manual. Batas waktu peminjaman tidak memiliki standar baku, dan bukti serah terima hanya berupa kiriman foto barang via *chat* WhatsApp.
* **SOP Usulan (Sistem Aplikasi):**
  * **E-Form Peminjaman:** Peminjam mengisi form pengajuan langsung melalui sistem. Sistem akan otomatis menolak pengajuan jika status barang sedang "Dipinjam" atau "Rusak".
  * **Standarisasi Durasi:** Sistem akan membatasi rentang waktu maksimal peminjaman (misalnya maksimal 7 hari).
  * **Digital Handover:** Serah terima divalidasi melalui sistem (klik tombol "Terima Barang" oleh peminjam dan admin) sebagai pengganti Berita Acara Serah Terima (BAST), yang tersimpan otomatis di log *database*.

### 3. Pengembalian & Pelacakan (*Tracking*)
* **SOP Saat Ini (Manual):** Konfirmasi pengembalian hanya via foto di grup *chat*. Tidak ada pelacakan terpusat siapa yang sedang memegang barang, sehingga rentan terjadi kehilangan atau kerusakan yang tidak bisa dipertanggungjawabkan akibat pesan *chat* yang tertumpuk.
* **SOP Usulan (Sistem Aplikasi):**
  * **Notifikasi Otomatis:** Sistem akan mengirimkan *reminder* (peringatan) otomatis jika masa pinjam barang hampir habis atau sudah *overdue* (terlambat).
  * **Dashboard Tracking:** Admin dapat melihat dasbor interaktif yang menampilkan daftar barang yang sedang keluar, siapa peminjamnya, dan kapan tenggat waktu pengembaliannya.
  * **Verifikasi Kondisi:** Saat pengembalian, admin harus memperbarui status kondisi barang di sistem (Baik/Rusak) sebelum transaksi peminjaman dianggap "Selesai".

### 4. Perawatan & Pengecekan Rutin (*Stock Opname*)
* **SOP Saat Ini (Manual):** Pengecekan bersifat reaktif (menunggu barang habis/rusak baru melapor). Pencatatan kondisi barang sangat terbatas, sering menyebabkan selisih data antara catatan Excel dengan fisik barang di ruangan.
* **SOP Usulan (Sistem Aplikasi):**
  * **Fitur Audit Cepat:** Dilengkapi fitur *Stock Opname* berkala di mana admin tinggal mencocokkan barang fisik dengan daftar di sistem.
  * **Minimum Stock Alert:** Untuk barang habis pakai (seperti tinta/ATK), sistem akan memberikan peringatan jika stok sudah mencapai batas minimum, sehingga pengadaan bisa dilakukan sebelum barang benar-benar habis.

### 5. Penghapusan/Pemutihan Barang Keluar
* **SOP Saat Ini (Manual):** Belum ada alur pemutihan aset yang jelas. Barang yang hilang/rusak total hanya dilaporkan secara lisan ke Ketua/Bendahara, dan datanya hanya diubah keterangannya menjadi "dalam servis/diganti", membuat daftar barang aktif menjadi rancu.
* **SOP Usulan (Sistem Aplikasi):**
  * **Status Barang Dinamis:** Sistem menyediakan opsi status "Write-off" atau "Dihapus/Pemutihan".
  * **Approval Workflow:** Penghapusan barang dari daftar aktif harus melalui klik persetujuan (*digital approval*) dari akun Ketua.
  * **Arsip Terpisah:** Data barang yang sudah dihapus tidak akan hilang, melainkan dipindahkan ke tabel *History/Archive* agar tidak mengganggu jumlah aset aktif namun tetap bisa dilacak riwayatnya untuk keperluan Laporan Pertanggungjawaban (LPJ).

**3. Use Case**

# 💡 Solusi
[Tuliskan rancangan solusi yang ditawarkan. Sebutkan fitur-fitur unggulan dari Sistem Inventaris UKM yang akan dibuat dan bagaimana sistem tersebut dapat menyelesaikan masalah yang ada...]
