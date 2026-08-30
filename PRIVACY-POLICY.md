# Kebijakan Privasi TaxPilot - Faktur & BuPot Downloader

**Tanggal berlaku: 30 Agustus 2026**

**Developer:** I Kadek Dharma Putra

**Contact:** dharmaputra7777@gmail.com

Kebijakan Privasi ini menjelaskan cara ekstensi Chrome **TaxPilot - Faktur & BuPot Downloader** (selanjutnya disebut “TaxPilot”) memproses data ketika digunakan untuk mengunduh dan mengganti nama PDF Faktur Pajak atau Bukti Potong dari Coretax Direktorat Jenderal Pajak.

## 1. Ringkasan

TaxPilot bekerja secara lokal di browser pengguna. TaxPilot tidak mengirimkan isi PDF, data perpajakan, kredensial, riwayat penggunaan, atau data pribadi pengguna kepada pengembang maupun server eksternal milik TaxPilot.

TaxPilot tidak menjual data, tidak menggunakan data untuk iklan, tidak melakukan pelacakan pengguna, dan tidak memakai layanan analitik pihak ketiga.

## 2. Data yang diproses

Untuk menjalankan fungsi unduh dan penamaan otomatis, TaxPilot dapat memproses data berikut:

- isi PDF Faktur Pajak dan Bukti Potong yang dipilih untuk diunduh;
- nomor faktur, nomor bukti potong, masa pajak, serta nama pihak yang tercantum di dalam PDF;
- alamat atau URL PDF sementara yang dibuat oleh halaman Coretax;
- nama berkas, identitas unduhan, dan status penyelesaian unduhan;
- jenis dokumen yang dipilih pengguna;
- ringkasan proses, seperti jumlah berhasil, jumlah gagal, durasi, dan rata-rata waktu per PDF; dan
- pesan status teknis yang diperlukan untuk menampilkan hasil proses.

Dokumen perpajakan dapat memuat data pribadi atau data usaha. TaxPilot hanya memproses bagian yang diperlukan untuk mengunduh, membaca, dan menentukan nama berkas.

## 3. Tujuan pemrosesan

Data tersebut hanya digunakan untuk:

- membuka modul Coretax sesuai jenis dokumen yang dipilih;
- menjalankan unduhan PDF dari tab Coretax yang aktif;
- membaca teks PDF secara lokal menggunakan PDF.js yang disertakan bersama ekstensi;
- membuat nama berkas berdasarkan nomor dokumen, masa pajak, dan nama pihak terkait;
- mencegah nama berkas yang tidak sesuai atau unduhan ganda selama proses berjalan;
- menampilkan progres, hasil, kegagalan, waktu, dan rata-rata pemrosesan; serta
- menghentikan proses ketika pengguna menekan tombol **Stop**.

## 4. Cara dan lokasi pemrosesan

Pemrosesan berlangsung di perangkat pengguna melalui Chrome atau browser berbasis Chromium yang kompatibel. Pembacaan PDF dan pembuatan nama berkas dilakukan di dalam tab Coretax serta komponen lokal ekstensi.

Komunikasi jaringan yang diperlukan untuk mengambil PDF tetap ditujukan ke sumber PDF pada Coretax atau URL sementara yang dibuat oleh halaman Coretax. TaxPilot tidak mengunggah salinan PDF ke server pengembang.

## 5. Penyimpanan dan masa retensi

TaxPilot menggunakan penyimpanan lokal atau sesi milik Chrome untuk menyimpan:

- pilihan jenis dokumen;
- status dan ringkasan proses; serta
- metadata nama berkas sementara yang diperlukan selama unduhan berjalan.

Data sementara di memori, termasuk Blob atau byte PDF, hanya digunakan selama proses pembacaan dan unduhan. Berkas PDF yang selesai diunduh disimpan di lokasi unduhan normal browser dan tetap berada di perangkat pengguna sampai pengguna menghapusnya.

Pengguna dapat menghapus data ekstensi melalui pengaturan browser, menghapus ekstensi, atau menghapus berkas unduhan secara manual.

## 6. Pembagian data kepada pihak lain

TaxPilot tidak mengirim, menjual, menyewakan, atau membagikan data yang diproses kepada pengembang, pengiklan, broker data, maupun pihak ketiga lainnya.

Penggunaan situs dan layanan Coretax tetap tunduk pada kebijakan serta ketentuan yang ditetapkan oleh Direktorat Jenderal Pajak. TaxPilot tidak mengendalikan penyimpanan atau pemrosesan data yang dilakukan oleh Coretax itu sendiri.

## 7. Kredensial dan autentikasi

TaxPilot tidak meminta, membaca, atau menyimpan nama pengguna, kata sandi, token autentikasi, maupun kredensial Coretax. Ekstensi berjalan pada tab Coretax yang telah dibuka dan diautentikasi sendiri oleh pengguna.

## 8. Izin browser

TaxPilot menggunakan izin berikut:

- **activeTab**: mengakses tab aktif setelah pengguna menjalankan TaxPilot;
- **scripting**: menjalankan fungsi pengunduhan dan pembacaan PDF pada tab Coretax yang dipilih pengguna;
- **downloads**: mengelola nama berkas serta memantau keberhasilan atau kegagalan unduhan; dan
- **storage**: menyimpan pilihan pengguna, status proses, dan ringkasan hasil secara lokal.

Izin tersebut hanya digunakan untuk fungsi utama TaxPilot dan bukan untuk pelacakan aktivitas penelusuran.

## 9. Keamanan dan tanggung jawab pengguna

TaxPilot dirancang agar pemrosesan data tetap berada di perangkat pengguna. Namun, tidak ada perangkat lunak yang dapat menjamin keamanan mutlak. Pengguna bertanggung jawab untuk:

- menggunakan TaxPilot hanya pada akun dan dokumen yang berhak diakses;
- menjaga keamanan perangkat serta akun Coretax;
- memeriksa nama dan isi berkas hasil unduhan; dan
- melindungi PDF perpajakan yang tersimpan di perangkat.

## 10. Hak dan kontrol pengguna

Pengguna dapat kapan saja:

- menghentikan proses melalui tombol **Stop**;
- menutup atau menonaktifkan TaxPilot;
- menghapus data lokal ekstensi melalui pengaturan browser;
- menghapus berkas PDF dari folder unduhan; atau
- menghapus instalasi TaxPilot untuk menghentikan seluruh pemrosesan oleh ekstensi.

## 11. Perubahan kebijakan

Kebijakan Privasi ini dapat diperbarui apabila fungsi, izin, atau cara pemrosesan data TaxPilot berubah. Tanggal berlaku di bagian atas dokumen akan diperbarui ketika terdapat perubahan material.

## 12. Kontak

Untuk pertanyaan mengenai privasi atau penggunaan TaxPilot, hubungi pengembang melalui alamat dukungan atau kanal kontak yang tercantum pada halaman distribusi resmi ekstensi.

