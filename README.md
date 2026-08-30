# Kebijakan Privasi TaxPilot - Coretax Assistant

**Tanggal berlaku: 30 Agustus 2026**  
**Terakhir diperbarui: 30 Agustus 2026**

TaxPilot - Coretax Assistant (selanjutnya disebut **“TaxPilot”**) adalah ekstensi Chrome yang membantu pengguna menjalankan otomasi Credit/Uncredit E-Faktur serta mengunduh dan memberi nama file Faktur Pajak dan Bukti Potong pada situs Coretax DJP. Kebijakan ini menjelaskan data yang diproses, tujuan pemrosesan, penyimpanan, pembagian data, dan pilihan pengguna.

## 1. Pengelola dan kontak

TaxPilot dikelola oleh **I Kadek Dharma Putra**. Untuk pertanyaan privasi, permintaan akses, koreksi, atau penghapusan akun, hubungi:

**Email: dharmaputra7777@gmail.com**

Placeholder di atas harus diganti dengan alamat email yang aktif sebelum ekstensi dipublikasikan.

## 2. Data yang diproses

### A. Data akun dan autentikasi

Saat pengguna mendaftar atau login, TaxPilot memproses:

- alamat email;
- password yang dimasukkan langsung ke layanan autentikasi Supabase;
- ID pengguna, nama tampilan jika tersedia, status akses, paket, dan tanggal berakhir akses;
- token akses dan token penyegaran sesi;
- kode promo/trial dan status penukarannya; serta
- versi ekstensi dan hasil pemeriksaan hak akses.

TaxPilot tidak menyimpan password di penyimpanan ekstensi atau basis data aplikasi. Password diproses oleh Supabase Auth. Token sesi disimpan sementara melalui `chrome.storage.session` dan dibersihkan saat logout atau ketika sesi browser berakhir sesuai perilaku Chrome.

### B. Data dokumen pajak dan konten Coretax

Ketika pengguna secara sadar menjalankan modul, TaxPilot dapat membaca dan memproses secara lokal:

- nomor Faktur Pajak atau Bukti Potong;
- nama lawan transaksi, masa dan tahun pajak, serta informasi yang tampil pada dokumen;
- pilihan status Credit/Uncredit;
- data Excel/CSV yang diimpor, nama file dan lembar kerja, serta kesalahan validasi;
- konten dan metadata PDF, nama file tujuan, serta status unduhan;
- URL tab Coretax yang sedang dipilih; dan
- progres operasi dan log teknis, yang dapat memuat nomor dokumen dan hasil proses.

Data impor, isi PDF, dan konten dokumen pajak tersebut diproses di perangkat pengguna untuk menjalankan fungsi yang diminta. Data tersebut tidak dikirim ke TaxPilot, Supabase, Resend, atau Cloudflare.

TaxPilot tidak meminta, membaca, atau menyimpan username, password, maupun OTP Coretax. Pengguna harus login sendiri pada situs resmi Coretax dan TaxPilot hanya bekerja dalam sesi Coretax yang sudah aktif.

### C. Data teknis halaman web

Saat halaman konfirmasi email atau kebijakan privasi dibuka, penyedia hosting Cloudflare dapat memproses data permintaan web standar seperti alamat IP, jenis browser, waktu akses, dan informasi keamanan jaringan sesuai kebijakan layanannya. Tautan konfirmasi menggunakan fragmen URL agar token tidak disertakan dalam permintaan HTTP awal ke Cloudflare. Halaman konfirmasi menghapus fragmen tersebut dari bilah alamat dan tidak menyimpannya dalam basis data aplikasi.

## 3. Tujuan penggunaan data

Data hanya digunakan untuk:

- membuat, mengautentikasi, dan menjaga keamanan akun;
- memeriksa paket, trial, dan hak akses pengguna;
- menjalankan otomasi Coretax yang dipilih pengguna;
- mengunduh dan memberi nama dokumen sesuai pilihan pengguna;
- menyimpan preferensi, data impor, progres, dan log lokal agar alur dapat dilanjutkan;
- mengirim email konfirmasi akun dan email layanan penting;
- mencegah penyalahgunaan, menyelesaikan masalah, dan menjaga keamanan layanan; serta
- memenuhi kewajiban hukum yang berlaku apabila diwajibkan.

TaxPilot tidak menjual data pengguna, tidak menayangkan iklan berbasis minat, tidak menggunakan data untuk penilaian kredit, dan tidak menggunakan data untuk tujuan yang tidak berkaitan dengan fungsi TaxPilot.

## 4. Penyimpanan dan masa retensi

- **Di perangkat:** pengaturan, data impor, progres, dan log disimpan melalui `chrome.storage.local` sampai ditimpa, dihapus oleh pengguna, data browser dibersihkan, atau ekstensi dihapus.
- **Sesi:** token autentikasi dan metadata sementara unduhan disimpan melalui `chrome.storage.session` dan dibersihkan saat logout atau ketika sesi browser berakhir sesuai perilaku Chrome.
- **Server:** data akun dan hak akses disimpan selama akun atau layanan masih aktif dan selama diperlukan untuk tujuan administrasi, keamanan, atau hukum. Catatan pemeriksaan akses dihapus otomatis setelah **180 hari**.
- **Penghapusan akun:** pengguna dapat meminta penghapusan melalui email dukungan. Data yang wajib dipertahankan karena kewajiban hukum atau keamanan dapat disimpan sebatas masa yang diperlukan.

## 5. Penyedia layanan dan pembagian data

TaxPilot menggunakan penyedia berikut hanya untuk mendukung fungsi layanan:

- **Supabase:** autentikasi, sesi akun, basis data hak akses, trial/promo, dan catatan pemeriksaan akses;
- **Resend:** pengiriman email konfirmasi dan email layanan, termasuk alamat penerima serta metadata pengiriman;
- **Cloudflare:** hosting halaman konfirmasi dan kebijakan privasi serta keamanan jaringan; dan
- **Coretax DJP:** situs tujuan yang berinteraksi dengan TaxPilot atas perintah pengguna dalam sesi Coretax pengguna sendiri.

Data tidak dibagikan kepada pihak lain kecuali kepada penyedia layanan yang diperlukan, atas persetujuan pengguna, untuk keamanan dan pencegahan penyalahgunaan, atau jika diwajibkan hukum. Akses manusia terhadap data dibatasi pada kebutuhan dukungan yang disetujui pengguna, penyelidikan keamanan/penyalahgunaan, pemenuhan kewajiban hukum, atau data yang telah diagregasi/dianonimkan untuk operasional internal.

## 6. Keamanan

Komunikasi jaringan TaxPilot menggunakan HTTPS. Izin ekstensi dibatasi pada fungsi yang diperlukan dan dua host yang digunakan: situs Coretax DJP serta proyek Supabase TaxPilot. Semua kode yang dijalankan oleh ekstensi disertakan dalam paket ekstensi; TaxPilot tidak mengunduh atau menjalankan kode jarak jauh.

Tidak ada sistem yang sepenuhnya bebas risiko. Pengguna tetap bertanggung jawab menjaga keamanan akun Google Chrome, email, Coretax, perangkat, dan passwordnya.

## 7. Pilihan dan hak pengguna

Pengguna dapat:

- tidak memberikan data dengan tidak membuat akun atau tidak menjalankan modul;
- menghapus data lokal melalui fitur bersihkan/reset bila tersedia, menghapus data situs/ekstensi di Chrome, atau menghapus ekstensi;
- logout untuk mengakhiri sesi TaxPilot;
- meminta akses, koreksi, atau penghapusan data akun melalui email dukungan; dan
- mencabut penggunaan dengan berhenti memakai TaxPilot.

Menghapus ekstensi tidak secara otomatis menghapus akun server. Hubungi email dukungan untuk permintaan penghapusan akun server.

## 8. Anak-anak

TaxPilot ditujukan untuk pengguna yang berwenang mengelola administrasi pajak, bukan untuk anak-anak. TaxPilot tidak dengan sengaja mengumpulkan data anak-anak.

## 9. Kepatuhan Penggunaan Terbatas Chrome Web Store

Penggunaan informasi yang diterima dari API Chrome dan izin ekstensi mematuhi **Kebijakan Data Pengguna Chrome Web Store**, termasuk persyaratan **Penggunaan Terbatas (Limited Use)**. Data tersebut hanya digunakan untuk menyediakan atau meningkatkan fungsi TaxPilot yang terlihat dan diminta pengguna. Data tidak digunakan untuk iklan yang dipersonalisasi, tidak dijual, tidak dipindahkan untuk penilaian kredit, dan tidak dibaca manusia kecuali dalam pengecualian dukungan, keamanan, hukum, atau agregasi/anonymisasi yang diizinkan kebijakan.

## 10. Perubahan kebijakan

Kebijakan ini dapat diperbarui apabila fungsi, penyedia layanan, atau persyaratan hukum berubah. Tanggal pembaruan akan dicantumkan di bagian atas. Jika perubahan bersifat material, pemberitahuan akan diberikan melalui halaman ini, ekstensi, atau email layanan bila sesuai.

## 11. Pernyataan independensi

TaxPilot bukan produk resmi dan tidak berafiliasi dengan Direktorat Jenderal Pajak atau Kementerian Keuangan Republik Indonesia. Pengguna wajib memakai TaxPilot hanya pada akun dan dokumen pajak yang berhak diakses.
