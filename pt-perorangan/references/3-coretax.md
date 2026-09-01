# 3 — Coretax DJP

**Portal:** `coretaxdjp.pajak.go.id`
**Biaya:** Rp 0.

NPWP Badan sudah terbit otomatis lewat AHU. Yang belum ada adalah **akses**
ke akunnya.

## ⚠️ Akunnya sudah ada — jangan pilih "Aktivasi"

Ini menghabiskan waktu banyak orang.

Saat NPWP Badan terbit lewat AHU, **Coretax otomatis membuatkan akun wajib
pajaknya**. Pemiliknya hanya tidak pernah diberi kata sandi.

Kalau memilih menu **Aktivasi Akun Wajib Pajak**, sistem akan menolak:

> *"Wajib Pajak Sudah Memiliki Akun Wajib Pajak, Silakan Login Kembali atau
> Lakukan Lupa Kata Sandi"*

**Jalur yang benar: "Lupa Kata Sandi?" di halaman login.**

| ID Pengguna | Untuk |
|---|---|
| NPWP 16 digit | akun badan |
| NIK | akun orang pribadi |

Hal yang sama berlaku untuk akun **pribadi** pemiliknya — sering juga sudah
ada tanpa disadari.

## ⚠️ NPWP lama 15 digit sudah pensiun

Kalau pengguna punya NPWP orang pribadi lama (format `xx.xxx.xxx.x-xxx.xxx`),
kemungkinan besar sudah dilebur ke NIK. Gejalanya: pencarian NPWP lama
berbunyi "Wajib Pajak Tidak Ditemukan", sementara **pencarian dengan NIK
berhasil**.

Pakai NIK. NPWP lama tidak lagi berlaku sebagai identitas maupun ID login.

## Formulir mencocokkan data, bukan menerima data

Formulir aktivasi dan reset **membandingkan** email dan nomor HP yang
diketik dengan yang tersimpan di DJP. Salah sedikit → ditolak.

Kalau tidak tahu email yang terdaftar untuk badan, **cek di dashboard AHU**
pada bagian *Informasi Perseroan* — itulah yang mengalir ke DJP. Sering
berbeda dari email akun AHU milik pemiliknya.

⚠️ Validasi baru berjalan **setelah fokus pindah dari kolom**. Mengetik lalu
langsung membaca layar akan menampilkan galat lama yang menyesatkan. Klik
kolom lain dulu, baru periksa.

## Onboarding pertama: kata sandi DAN passphrase

Setelah berhasil masuk, Coretax memaksa wizard yang **memblokir seluruh
menu** sampai selesai. Setiap navigasi dilempar balik ke halaman ini.

Dua tahap:

1. **Kata Sandi** — untuk login
2. **Passphrase** — untuk **Sertifikat Elektronik** (tanda tangan digital)

⚠️ **Passphrase bukan kata sandi kedua.** Itu kunci tanda tangan digital,
dan **inilah yang sebenarnya memblokir semua permohonan layanan**. Tanpa
passphrase, formulir permohonan tidak bisa dikirim — dan pesan galatnya
tidak pernah menyebut passphrase.

⚠️ **Passphrase yang hilang tidak bisa direset lewat email.** Perlu
mengajukan sertifikat elektronik baru ke KPP. Suruh pengguna menyimpannya di
pengelola kata sandi dengan label jelas.

Akun **orang pribadi** juga menuntut **verifikasi wajah** (foto langsung
dicocokkan dengan data kependudukan). Ini jelas pekerjaan pengguna.

⚠️ Aksi ambil foto pernah me-**reset seluruh formulir**. Urutan yang aman:
**foto dulu, kolom kontak belakangan**, lalu periksa lagi seluruh isian
sebelum menyimpan.

## ⚠️ Periksa KLU — sering salah

Buka **Portal Saya → Profil Saya → Ikhtisar Profil Wajib Pajak** dan lihat
**Kegiatan Utama / KLU**.

Sistem tampaknya mengambil **KBLI dengan nomor terkecil** dari daftar di
AHU, bukan yang ditetapkan sebagai kegiatan utama. Perusahaan perangkat
lunak dengan KBLI 46511 di daftarnya akan tercatat sebagai **pedagang grosir
komputer**.

Ini bukan kosmetik. DJP memakai KLU untuk membandingkan SPT dengan wajib
pajak sejenis. Profil keuangan software house sangat berbeda dari pedagang
grosir, dan ketidakcocokan itu mengundang pertanyaan.

**Perbaiki lewat:** *Portal Saya → Perubahan Data → Identitas Wajib Pajak*

- Centang **Perbarui Kode Ekonomi Utama** untuk membuka kolomnya
- Cari kode lewat **deskripsi**, bukan angka
- Perbarui juga **Deskripsi Kegiatan** agar cocok
- ⚠️ **Tanggal Mulai diisi tanggal PT berdiri**, bukan tanggal hari ini —
  supaya tercatat sebagai koreksi data, bukan perubahan bidang usaha
- **Matikan** bagian Rekening Bank kalau PT belum punya rekening; kotaknya
  kadang tercentang sendiri dan memunculkan kolom wajib yang mustahil diisi
- Lampirkan **NIB** sebagai dokumen pendukung

Prosesnya cepat — dalam pengalaman nyata, terbit **keesokan harinya** berupa
*Surat Pemberitahuan Perubahan Data*.

## Peran Wakil untuk mengurus badan

Sebagian layanan menolak permohonan yang diajukan "sebagai badan" dan
menuntut peran **Wakil**:

> *"Untuk jenis layanan ini, Wajib Pajak Badan wajib memilih peran
> permintaan sebagai Wakil"*

Caranya: login dengan **akun pribadi**, lalu lewat pemilih akun di kanan
atas pilih **Akun Perwakilan → nama PT**. Header berubah menjadi
**IMPERSONATE**.

⚠️ **Peran Wakil biasanya sudah terdaftar otomatis** untuk direktur —
tidak perlu didaftarkan. Formulir akan meminta **Nomor Penunjukan**
(format `DA…`) yang tinggal dipilih dari daftar.

⚠️ Layanan tertentu juga menuntut status wajib pajak **Aktif**. Akun pribadi
yang berstatus Non-Efektif (lazim untuk karyawan yang pajaknya dipotong
kantor) akan ditolak — makanya harus lewat peran Wakil atas nama PT.

## Dokumen yang bisa diunduh dari Coretax

- **Kartu NPWP** (TIN Card)
- **SKT** (Surat Keterangan Terdaftar)
- Surat penerbitan akun, bukti penerimaan surat

⚠️ **Surat penerbitan akun memuat kata sandi dalam bentuk terbaca.** Setelah
kata sandi diganti, suruh pengguna menghapus atau mengamankan berkas itu.
