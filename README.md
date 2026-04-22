# 📦 Topik Proyek: Sistem Inventaris UKM
## 👥 Anggota Kelompok 9
| **Nama** | **NPM** |
| ------------- | ------------- |
| Dheka Airlangga | 4524210027 |
| Naila Putri Fahel | 4524210053 |
| Maghfiroh Lisabiliana | 4524210040 |
| Az-Zahra Putri| 4524210018 |
| Ghifari Ezra Ramadhan | 4524210041 |

# 🚨 Masalah
Pengelolaan inventaris saat ini terkendala oleh sistem yang terfragmentasi dan minim standarisasi. Ketergantungan pada pencatatan manual dan database yang tidak menyeluruh hanya mencakup aset besar sering kali menyebabkan selisih data atau missing link antara catatan dan fisik barang. Masalah ini diperparah dengan absennya sistem kodifikasi unik, sehingga pelacakan barang secara spesifik menjadi sangat sulit dilakukan.

Selain itu, terdapat risiko administratif yang tinggi karena ketiadaan dokumen serah terima formal dan durasi pinjam yang tidak diatur secara baku oleh organisasi. Minimnya jadwal stock opname rutin serta ketiadaan prosedur pemutihan aset yang jelas mengakibatkan database tetap dipenuhi data barang rusak atau hilang, yang pada akhirnya mengaburkan akuntabilitas laporan pertanggungjawaban UKM.

# 🔍 Analisis
**1. Aktor**
[Tuliskan ...] 

## 📋 Bagian 2: Analisis Perbandingan SOP
Klik pada masing-masing aspek di bawah ini untuk melihat detail perbandingan alur kerja sebelum dan sesudah implementasi sistem:

<details>
<summary><b>1. Pencatatan & Data Masuk (Input Barang Baru)</b></summary><br>

* **❌ SOP Manual:** Pencatatan bergantung pada struk fisik. Tidak ada kodifikasi/nomor seri terpusat, dan *database* (Excel) hanya digunakan untuk mendata aset berukuran besar.
* **✅ SOP Sistem:** Semua barang langsung diinput ke *database*. Sistem otomatis membuatkan kode unik (ID/Barcode) dan struk pembelian dapat diunggah langsung ke sistem secara *real-time*.
</details>

<details>
<summary><b>2. Peminjaman (Alur Keluar Barang)</b></summary><br>

* **❌ SOP Manual:** Peminjam mengirim surat fisik/PDF. Tidak ada standar batas waktu peminjaman, dan bukti serah terima hanya mengandalkan kiriman foto via *chat* WhatsApp.
* **✅ SOP Sistem:** Pengajuan melalui *E-Form*. Sistem menolak otomatis jika barang berstatus "Dipinjam" atau "Rusak", membatasi durasi maksimal peminjaman, dan tervalidasi melalui *Digital Handover* di sistem.
</details>

<details>
<summary><b>3. Pengembalian & Pelacakan (Tracking)</b></summary><br>

* **❌ SOP Manual:** Konfirmasi pengembalian via grup *chat* rentan tertumpuk. Tidak ada pelacakan terpusat siapa yang memegang barang.
* **✅ SOP Sistem:** Terdapat *Dashboard Tracking* interaktif. Sistem mengirim notifikasi *reminder* keterlambatan, dan mewajibkan admin memverifikasi kondisi barang (Baik/Rusak) sebelum transaksi selesai.
</details>

<details>
<summary><b>4. Perawatan & Pengecekan Rutin (Stock Opname)</b></summary><br>

* **❌ SOP Manual:** Pengecekan bersifat reaktif (menunggu barang habis/rusak), sering menyebabkan selisih data antara catatan dan fisik ruangan.
* **✅ SOP Sistem:** Dilengkapi fitur Audit Cepat (*Stock Opname* berkala) dan *Minimum Stock Alert* untuk memberi peringatan jika barang habis pakai (seperti ATK/tinta) perlu di-restock.
</details>

<details>
<summary><b>5. Penghapusan/Pemutihan Barang Keluar</b></summary><br>

* **❌ SOP Manual:** Barang hilang/rusak dilaporkan secara lisan. Data hanya diubah menjadi "dalam servis", membuat daftar barang aktif rancu.
* **✅ SOP Sistem:** Menggunakan *Approval Workflow* dari akun Ketua untuk status "Write-off". Data yang dihapus dipindahkan ke tabel *Archive* sehingga tidak mengganggu jumlah aset aktif namun tetap tercatat untuk LPJ.
</details>

**3. Use Case**
[Tuliskan ...] 

# 💡 Solusi
[Tuliskan rancangan solusi yang ditawarkan. Sebutkan fitur-fitur unggulan dari Sistem Inventaris UKM yang akan dibuat dan bagaimana sistem tersebut dapat menyelesaikan masalah yang ada...]
