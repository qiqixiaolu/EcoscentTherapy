# ECOSCENT THERAPY — Aromaterapi untuk Kesehatan Mental Mahasiswa

ECOSCENT THERAPY adalah sebuah platform web interaktif yang menjembatani pendekatan non-verbal dalam **Bimbingan dan Konseling (BK)** dengan kekuatan neurosains aromaterapi. Proyek ini dirancang khusus untuk membantu mahasiswa mengelola stres akademik, kecemasan (*anxiety*), *burnout*, hingga masalah prokrastinasi melalui ritual relaksasi yang dipetakan langsung ke 4 bidang layanan utama BK (Pribadi, Sosial, Belajar, dan Karier).



## ✦ Deskripsi Umum Sistem
Web ini telah bertransformasi dari halaman statis menjadi **aplikasi web dinamis berbasis penyimpanan lokal (`localStorage`)**. Sistem ini mengintegrasikan seluruh interaksi data secara *real-time* antara antarmuka pengguna utama (`index.html`), ruang curhat varian wewangian (`cinnamon.html`, `jasmine.html`, `coffee.html`), dan panel kendali administrator (`admin.html`) tanpa memerlukan konfigurasi database server eksternal yang rumit.

## 🕯️ Varian Mood & Bidang Layanan BK
Platform ini menyediakan tiga pilar aroma utama yang masing-masing merepresentasikan solusi psikologis mahasiswa:
1. **Cinnamon (Mood: Fokus)**: Diintegrasikan dengan **Layanan Belajar & Karier** untuk membantu konsentrasi, mengatasi *overthinking*, dan memicu keberanian mengambil tindakan di bawah tekanan *deadline*.
2. **Jasmine (Mood: Tenang)**: Diintegrasikan dengan **Layanan Pribadi & Sosial** untuk menurunkan tingkat kecemasan presentasi, menenangkan sistem saraf, dan membuka ruang kenyamanan saat bercerita.
3. **Coffee (Mood: Semangat Pagi)**: Diintegrasikan dengan **Layanan Belajar** untuk membangun regulasi energi positif, memicu motivasi, dan memberikan semangat untuk memulai kembali.

## 🚀 Fitur Utama & Pembaruan Dinamis

### 1. Rotasi Afirmasi Otomatis (Hero Section)
* Menampilkan kalimat afirmasi positif/energi hari ini secara dinamis pada halaman utama.
* Kalimat berganti secara halus setiap **7 detik**.
* Konten afirmasi ini dapat ditambah, diubah, atau dihapus langsung melalui Admin Dashboard.

### 2. Artikel Edukasi Dinamis & Pop-up Modal
* Artikel dimuat langsung dari database lokal admin secara dinamis.
* Halaman utama hanya menampilkan **judul dan cuplikan singkat (preview)** beberapa kalimat saja guna menjaga estetika tata letak (*clean layout*).
* Menyediakan tombol **"Baca Selengkapnya"** yang memicu *Pop-up Modal* interaktif untuk memunculkan artikel secara utuh tanpa perlu melakukan *reload* halaman.

### 3. Integrasi Sistem *Diary Wall* (Ruang Cerita Varian)
* Mahasiswa dapat mencurahkan isi hati dan *mood* mereka secara anonim maupun personal di halaman `cinnamon.html`, `jasmine.html`, dan `coffee.html`.
* Setiap curhatan langsung tersinkronisasi dan tersimpan rapi ke dalam database lokal.
* Halaman ruang cerita dilengkapi pemutar musik latar (*ambient piano*) otomatis via YouTube IFrame API untuk memperkuat efek terapi relaksasi.

### 4. Panel Kontrol Administrator (`admin.html`)
* Dilindungi oleh sistem otentikasi kunci akses.
* Manajer konten dapat melakukan operasi **CRUD Lengkap** (Buat, Baca, Ubah, Hapus) untuk data Afirmasi Utama dan Artikel Edukasi.
* Menyediakan fitur penapis (*filter*) varian untuk memantau dan menghapus kiriman curhatan mahasiswa yang tidak layak tayang pada *Diary Wall*.
* Fitur **Ekspor JSON** untuk menyalin seluruh *payload* database lokal dalam satu klik guna kebutuhan cadangan (*backup*).