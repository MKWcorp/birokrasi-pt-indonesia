# Jebakan — baca ini kalau prosesnya macet

Kumpulan hal yang menghentikan proses, disusun dari satu pendirian nyata.
Cari gejalanya.

## Gejala → penyebab

| Yang terlihat | Sebenarnya |
|---|---|
| NIB "Draft", *Menunggu Verifikasi Persyaratan Dasar* | **Penapisan lingkungan Amdalnet belum dikerjakan.** Bukan menunggu petugas. → `2-perizinan-oss.md` |
| KBLI dicari, "No data available" | Memakai kode **KBLI 2020**. Cari lewat **judul**, bukan kode. |
| AHU minta bayar Rp 50.000 lagi setelah sesi putus | Cek **Riwayat Pembelian Voucher** — mungkin sudah "Sudah Bayar". |
| Coretax: *"Wajib Pajak Sudah Memiliki Akun"* | Akun memang sudah dibuat otomatis. Pakai **Lupa Kata Sandi**, bukan Aktivasi. |
| Coretax login: *"Nama pengguna tidak ditemukan"* | Salah format ID. Badan = NPWP 16 digit; pribadi = **NIK**. NPWP lama 15 digit sudah pensiun. |
| Setiap menu Coretax dilempar ke "Tetapkan Kata Sandi" | Wizard onboarding **memblokir semua**. Selesaikan **dua tahap**: kata sandi **dan passphrase**. |
| Permohonan layanan Coretax tidak bisa dikirim | **Passphrase sertifikat elektronik** belum ditetapkan. Galatnya tidak pernah menyebut ini. |
| *"wajib memilih peran permintaan sebagai Wakil"* | Beralih ke **Akun Perwakilan** lewat pemilih akun kanan atas. |
| *"only available for Active Taxpayers"* | Sedang memakai akun pribadi yang Non-Efektif. Kerjakan lewat peran Wakil atas nama PT. |
| KLU tercatat sebagai bidang yang salah | Sistem mengambil **KBLI bernomor terkecil**. Perbaiki lewat Perubahan Data. |
| Bank/D&B minta "Akta Pendirian" | PT Perorangan tidak punya akta notaris. Yang ada **Surat Pernyataan Pendirian**. Tanyakan apakah diterima. |
| Dropdown "cuma punya 7 pilihan" | **Panelnya bisa digulir.** Gulir dulu sebelum menyimpulkan. |
| Jalur DUNS gratis "mustahil, minta laporan 3 tahun" | D&B memberi keringanan bila ditanya: laporan keuangan → **NIB**, AR data → **kosong**. |

## Pola perilaku situs pemerintah

Ini berulang di AHU, OSS, Coretax, dan D&B. Kenali polanya.

**Klik tombol kirim sering tidak memicu apa-apa lewat otomasi.** Formulir
berbasis React kadang tidak menanggapi klik terprogram, padahal klik manusia
berhasil. Setelah 2 kali gagal tanpa pesan apa pun, **serahkan tombolnya ke
pengguna** — jangan diklik berulang, risikonya permohonan ganda.

**Dropdown sering tidak benar-benar berpindah** meski terlihat terpilih.
Cara yang andal: kosongkan kolom → ketik kata kunci → tunggu daftar menyusut
→ klik satu-satunya hasil. **Lalu verifikasi kolomnya benar-benar berubah.**

**Formulir bisa ter-reset diam-diam.** Terutama setelah aksi berat seperti
mengambil foto. **Selalu gulir ke atas dan periksa seluruh isian sebelum
menyimpan.**

**Sesi cepat kedaluwarsa.** OSS dan Coretax berkali-kali melempar ke login.
Data yang sudah tersimpan aman; siapkan diri untuk login berulang.

**Halaman lambat, bukan mati.** Situs D&B kerap butuh 30 detik lebih per
klik. Tunggu, jangan mengulang klik.

**Nama berkas unduhan sering acak** (`d3b8e972-….pdf`). Segera ganti namanya
supaya tidak tertukar — dalam satu kasus, sertifikat kursus sempat disangka
dokumen AHU semata-mata karena namanya acak.

## Batas yang tidak boleh dilewati

Ini bukan preferensi gaya; ini soal siapa yang bertanggung jawab.

**Jangan mengarang data apa pun** yang masuk ke formulir negara — luas
bangunan, omzet, jumlah karyawan, tanggal. Tanya penggunanya.

**Jangan membuatkan bukti fisik.** Foto bangunan harus foto sungguhan.

**Jangan mencentang pernyataan mandiri atau menekan kirim** tanpa izin
eksplisit. Isinya mengikat pengguna berikut sanksi pidana/administratif.

**Jangan mengetik kata sandi, OTP, CAPTCHA, membuat akun, atau membayar.**

**Jangan mengisi data keuangan yang tidak ada.** Kalau perusahaan belum punya
riwayat piutang dagang, templat AR diunggah **kosong** — bukan diisi angka
karangan. Mengarang data pembayaran ke biro kredit itu jauh lebih serius
daripada sekadar salah isi formulir.
