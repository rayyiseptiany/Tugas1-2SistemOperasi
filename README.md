# Panduan Instalasi Linux di VirtualBox

Oleh: Rayyi Septiany T.Z.M (NIM: 09011282328108)  
Mata Kuliah: Sistem Operasi

## Daftar Isi
- [Langkah-langkah Instalasi](#langkah-langkah-instalasi)
- [Analisis Mount Point "/"](#analisis-mount-point-)
- [Penjelasan Sistem File](#penjelasan-sistem-file)

## Langkah-langkah Instalasi

### 1. Membuat Mesin Virtual Baru
- Buka Aplikasi VirtualBox
- Klik menu "New"
- Isi nama dan pilih ISO yang telah ditentukan
- Klik "Next"

![Langkah 1](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/1.jpg)

### 2. Konfigurasi Memori dan Prosesor
- Atur Base Memory dan Processors sesuai ukuran yang disarankan
- Klik "Next"

![Langkah 2](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/2.jpg)

### 3. Pengaturan Disk
- Buat Disk Size menjadi 25,00 GB
- Klik "Next"

![Langkah 3](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/3.jpg)

### 4. Tinjauan Pengaturan
- Periksa kembali Machine Name dan OS Type yang telah dibuat

![Langkah 4](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/4.jpg)

### 5. Konfigurasi Display
- Klik menu "Settings" dan pilih "Display"
- Atur Video Memory menjadi 128 MB
- Set Monitor Count ke 1 dan Scale Factor 100%
- Klik "OK"

![Langkah 5](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/5.jpg)

### 6. Memulai Instalasi
- Klik "Start" untuk memulai mesin virtual
- Pilih opsi "Install Linux Mint"

![Langkah 6](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/6.jpg)

### 7. Menerima Persyaratan
- Centang kotak persetujuan
- Klik "Lanjutkan"

![Langkah 7](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/7.jpg)

### 8. Partisi Disk
- Pilih opsi "Hapus disk dan pasang Linux"
- Klik "Lanjutkan"

![Langkah 8](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/8.jpg)

### 9. Pengaturan Lokasi
- Pilih lokasi Anda untuk mengatur zona waktu

![Langkah 9](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/9.jpg)

### 10. Konfigurasi Pengguna
- Isi Nama Anda, Nama Komputer, Nama Pengguna, dan Sandi
- Klik "Lanjutkan"

![Langkah 10](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/10.jpg)

### 11. Proses Instalasi
- Tunggu hingga proses instalasi selesai

![Langkah 11](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/11.jpg)

### 12. Instalasi Selesai
- Instalasi Linux Mint telah berhasil

![Langkah 12](https://github.com/rayyiseptiany/Tugas1-2SistemOperasi/blob/main/12.jpg)

## Analisis Mount Point "/"

Pemilihan "/" (root) sebagai Mount Point saat instalasi Linux sangat penting karena:

1. **Root Directory**: "/" adalah direktori utama dalam sistem file Linux. Semua direktori dan file lainnya berada di bawah "/".

2. **Struktur FHS**: Filesystem Hierarchy Standard (FHS) menetapkan "/" sebagai titik pemasangan dasar yang harus ada di setiap sistem Linux.

3. **Isolasi Direktori**: Memungkinkan isolasi direktori seperti /var, /tmp, dan /home ke partisi terpisah, mencegah partisi utama menjadi penuh.

4. **Instalasi dan Konfigurasi**: Sistem operasi memerlukan titik pemasangan dasar untuk menempatkan file sistem dan konfigurasi.

## Penjelasan Sistem File

### 1. ext4
- Sistem file jurnal untuk Linux
- Fitur: jurnal, extent, kapasitas besar (hingga 1 yobibyte), kompatibel dengan ext3 dan ext2

### 2. ext3
- Sistem file jurnal, pendahulu ext4
- Fitur: jurnal, kapasitas hingga 16 terabyte, kompatibel dengan ext2

### 3. Swap
- Area penyimpanan sementara untuk data yang tidak aktif di RAM
- Meningkatkan kemampuan sistem menangani kebutuhan memori besar

### 4. NTFS
- New Technology File System oleh Microsoft
- Fitur: jurnal, kapasitas hingga 256 terabyte, kompatibilitas terbatas dengan sistem non-Windows

### 5. FAT32
- File Allocation Table 32 oleh Microsoft
- Kapasitas: volume hingga 2 terabyte, file maksimal 4 gigabyte
- Kompatibel dengan berbagai sistem operasi

### 6. Btrfs
- B-Tree File System untuk Linux
- Fitur: jurnal, kapasitas hingga 16 exabyte, masih dalam pengembangan

Setiap sistem file memiliki kelebihan dan kekurangan. Pilihan tergantung pada kebutuhan spesifik penggunaan.
