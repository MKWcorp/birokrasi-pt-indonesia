# 2 — Perizinan berusaha di OSS (NIB)

**Portal:** `oss.go.id` → login → `beranda.oss.go.id` (dashboard) dan
`perizinan.oss.go.id` (proses perizinan).
**Biaya:** Rp 0.
**Hasil:** NIB, Sertifikat Standar, KKPR, SPPL.

Sesi OSS **sering putus**. Data tersimpan di server, jadi kerja yang sudah
lewat tidak hilang — tapi siapkan diri untuk login berulang kali.

## Alur

```
Data pelaku usaha → lokasi usaha → kegiatan usaha (KBLI)
   → data usaha (investasi, tenaga kerja, produk)
   → validasi risiko → PERIZINAN LINGKUNGAN ← penghambatnya di sini
   → pernyataan mandiri → NIB terbit
```

## ⚠️ Satu kegiatan usaha = satu KBLI

Ini mengejutkan orang yang mendaftarkan banyak KBLI di AHU. Di OSS, **tiap
kegiatan usaha hanya menampung satu KBLI dan satu Nama Usaha**. Setelah satu
KBLI ditambahkan, formulirnya terkunci.

KBLI lain perlu dibuat sebagai **kegiatan usaha baru** — masing-masing dengan
KKPR, penapisan lingkungan, dan perizinannya sendiri.

**Saran praktis:** selesaikan satu KBLI utama sampai NIB terbit lebih dulu.
NIB itu sudah sah dan cukup untuk membuka rekening bank serta ikut tender.
KBLI lain ditambahkan belakangan saat memang dibutuhkan.

## ⚠️ Penapisan lingkungan Amdalnet — penghambat tersembunyi

**Ini penyebab paling umum NIB berstatus "Draft" tanpa penjelasan.**

Gejalanya: Perizinan Berusaha berbunyi *"Menunggu Verifikasi Persyaratan
Dasar"*, NIB tetap **Draft**, dan tidak ada yang menjelaskan apa yang kurang.
Terlihat seperti sedang menunggu petugas. **Bukan.**

Buka **Detail Kegiatan → Persyaratan Dasar → Lingkungan**. Kalau ada baris
*Persetujuan Lingkungan* berstatus **"Penapisan Izin Lingkungan"** dengan
tombol **Proses Penapisan**, itulah penghambatnya — dan itu pekerjaan
pengguna, bukan pemerintah.

Klik tombol itu → sistem melempar ke **Amdalnet** (`amdalnet.kemenlh.go.id`),
milik Kementerian Lingkungan Hidup.

### Mengisi penapisan Amdalnet

Yang diminta:

- **Sektor** dan **Jenis Kegiatan** — pilihannya dipetakan dari KBLI,
  sering hanya ada satu opsi; sistem memakai padanan **KBLI 2020**
  (mis. 62199 muncul sebagai 62019)
- **Nama Usaha**
- **Nilai/Besaran Parameter** — biasanya *luas bangunan terbangun* dalam m²
- **Kawasan PIPPIB / kawasan lindung** — umumnya "Tidak"
- **Lokasi** — daratan, satu kabupaten/kota

⚠️ **Luas bangunan terbangun harus angka nyata.** Tooltip Amdalnet
mendefinisikannya sebagai luas lantai fisik seluruhnya; bangunan bertingkat
dijumlahkan. **Tanya penggunanya. Jangan mengarang.**

Untuk usaha mikro di bangunan biasa, hasilnya hampir selalu **SPPL** —
terbit otomatis, gratis, tanpa antre verifikator. Ambang yang memicu
UKL-UPL ada di kisaran ribuan meter persegi.

⚠️ **Hasil penapisan tidak dapat diubah setelah disimpan.** Sistem
memperingatkan hal ini. Pastikan angkanya benar sebelum menyimpan.

Setelah SPPL terbit, kembali ke OSS. Status Persetujuan Lingkungan berubah
jadi **"Izin Terbit/SS Terverifikasi"**, Perizinan Berusaha berubah jadi
**"Proses Perizinan Berusaha"**, dan tombol **Lanjut** aktif.

### Kalau Amdalnet minta login

Token SSO dari OSS bisa kedaluwarsa. Amdalnet lalu meminta username dan
kata sandi OSS. **Itu bagian pengguna.** Menutup tab dan mengulang dari
tombol Proses Penapisan kadang membuat token baru yang berhasil.

## Data usaha — hal yang perlu dijaga

**Tanggal mulai operasional** memakai pemilih bulan/tahun yang sering
menolak input otomatis. Kalau tiga cara sudah gagal, serahkan ke pengguna.

**Nilai investasi dan penjualan tahunan tidak boleh 0.** Sistem menolaknya.
Angka ini adalah proyeksi yang dideklarasikan, bukan realisasi — tapi tetap
pernyataan. Tanyakan ke pengguna; jangan mengisi sendiri.

⚠️ **Jangan mengulang nilai investasi penuh di tiap KBLI.** Kalau modal
perusahaan Rp 2 juta lalu tiap kegiatan usaha diisi Rp 2 juta, total
investasi perusahaan menggelembung jadi kelipatannya. Bagilah.

**Jumlah tenaga kerja** — orang yang sama tidak dihitung ulang di tiap
kegiatan usaha.

**Alamat** — perhatikan petunjuk di bawah kolom. Beberapa kolom alamat
meminta ditulis **tanpa RT/RW dan kode pos**, karena keduanya sudah ada
kolom sendiri.

## Dokumen lokasi

Sebagian tahap meminta unggahan PDF:

- **Dokumen Lokasi Administratif** — keterangan tertulis soal lokasi,
  ditandatangani pemilik usaha
- **Foto Tampak Depan** — foto bangunan sungguhan

⚠️ **Jangan pernah membuatkan gambar bangunan.** Kalau pengguna tidak punya
fotonya, minta mereka memotret. Mengarang bukti fisik untuk sistem perizinan
pemerintah adalah pemalsuan.

## Pernyataan mandiri

Menjelang akhir ada beberapa pernyataan mandiri: KKPR skala mikro,
kesanggupan K3L, dan kesediaan memenuhi standar usaha. Isinya mengikat
pengguna berikut sanksinya.

Untuk KBLI risiko **Menengah Rendah** ke atas, pernyataan kesediaan memenuhi
standar usaha memuat kewajiban nyata — misalnya laporan Data Industri tiap
6 bulan, sertifikat kompetensi SDM, SOP keamanan data. **Bacakan isinya ke
pengguna**, jangan biarkan mereka mencentang buta.

## Setelah NIB terbit

Empat dokumen terbit sekaligus dan semuanya bisa diunduh:

1. **Nomor Induk Berusaha**
2. **Sertifikat Standar**
3. Pernyataan Mandiri K3L
4. Pernyataan Mandiri Kesediaan Memenuhi Standar Usaha

Unduh NIB dan simpan dengan nama yang jelas — akan dipakai untuk bank,
D-U-N-S, dan pengganti laporan keuangan bagi perusahaan baru.
