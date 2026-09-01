---
name: birokrasi-pt-indonesia
description: >
  Menembus birokrasi pendirian dan kepatuhan PT Perorangan di INDONESIA,
  dari nol sampai perusahaan benar-benar bisa beroperasi. Mencakup seluruh
  rantai: pendaftaran di AHU Online (SK Pengesahan Kemenkumham + NPWP Badan
  otomatis, PNBP Rp 50.000), perizinan berusaha di OSS RBA (kegiatan usaha,
  KBLI 2025, KKPR, Sertifikat Standar, NIB), penapisan lingkungan di
  Amdalnet Kementerian Lingkungan Hidup (SPPL/UKL-UPL) yang diam-diam
  menahan NIB, aktivasi dan reset akun Coretax DJP berikut passphrase
  sertifikat elektronik dan peran Wakil Wajib Pajak, koreksi KLU yang
  sering salah, Surat Keterangan PPh Final 0,5% (PP 55/2022, layanan
  AS.06-01), kewajiban lapor rutin dan pembukuan badan, setoran modal 25%
  dengan tenggat 60 hari (PP 8/2021), pembukaan rekening bank atas nama PT,
  sampai pendaftaran nomor D-U-N-S Dun & Bradstreet untuk pasar global.

  Ditulis dari satu pendirian nyata yang dijalankan sampai tuntas, sehingga
  memuat jebakan yang tidak tertulis di panduan resmi mana pun: NIB berstatus
  Draft yang ternyata tertahan penapisan Amdalnet, akun Coretax yang sudah
  dibuat otomatis sehingga harus direset bukan diaktivasi, passphrase
  sertifikat elektronik yang memblokir semua permohonan tanpa pesan galat,
  kasus Coretax yang terbentuk tapi formulirnya kosong, KLU yang terisi dari
  KBLI bernomor terkecil, PT Perorangan yang tidak punya Akta Pendirian
  notaris, dan jalur D-U-N-S gratis yang tetap terbuka untuk perusahaan baru.
  Termasuk batas etis untuk asisten AI: dilarang mengarang data formulir
  negara, membuatkan bukti fisik, mencentang pernyataan mandiri, atau
  menekan tombol kirim tanpa izin pengguna.

  Gunakan saat pengguna menyebut: PT Perorangan, mendirikan PT, PT sendirian,
  perseroan perorangan, AHU, ahu.go.id, OSS, oss.go.id, NIB, KBLI, KKPR,
  SPPL, Amdalnet, izin lingkungan, Coretax, coretaxdjp, NPWP badan, KLU,
  SKT, SPT Tahunan Badan, PPh Final 0,5 persen, PP 55/2022, PP 23/2018,
  Suket pajak, passphrase sertifikat elektronik, Wakil Wajib Pajak, modal
  setor, PP 8/2021, rekening PT, stempel perusahaan, atau DUNS number.
  Also matches English: register a company in Indonesia, Indonesian sole
  founder PT, Indonesian business license, NIB, Indonesian tax compliance,
  Coretax activation, DUNS number Indonesia.
---

# Birokrasi PT — pendirian sampai patuh pajak

Panduan ini disusun dari **satu pendirian PT Perorangan yang benar-benar
dijalankan** — dari belum punya apa-apa sampai NIB terbit, NPWP aktif,
akun Coretax hidup, dan permohonan D-U-N-S terkirim. Total biaya resmi:
**Rp 50.000**.

Nilai utamanya bukan urutan langkah — itu ada di situs resmi. Nilainya ada
pada **hal-hal yang menghentikan proses dan tidak dijelaskan di mana pun**.
Baca `references/jebakan.md` lebih dulu kalau pengguna sudah tersangkut.

## Cara memakai panduan ini

Tanyakan dulu pengguna ada di tahap mana, lalu buka berkas rujukan yang
relevan. Jangan memuat semuanya sekaligus.

| Tahap | Berkas |
|---|---|
| Belum punya PT | `references/1-pendirian-ahu.md` |
| Sudah punya SK, butuh izin usaha | `references/2-perizinan-oss.md` |
| NIB tertahan, tidak jelas kenapa | `references/2-perizinan-oss.md` § Amdalnet |
| Urusan pajak, Coretax, NPWP | `references/3-coretax.md` |
| Kewajiban lapor rutin & pembukuan | `references/4-kewajiban-pajak.md` |
| Buka rekening bank atas nama PT | `references/5-rekening-bank.md` |
| Nomor D-U-N-S untuk pasar global | `references/6-duns.md` |
| **Tersangkut, error, atau bingung** | `references/jebakan.md` |

## Prinsip kerja yang wajib dipegang

Ini bukan pekerjaan biasa. Kesalahan di sini berbentuk denda, data resmi
yang salah, dan pernyataan hukum atas nama orang lain.

**Jangan pernah mengarang data.** Luas tanah, luas bangunan, omzet, jumlah
karyawan, tanggal — kalau tidak tahu, tanya. Angka karangan di formulir
negara bukan sekadar salah; itu pernyataan palsu yang ditandatangani
pengguna.

**Jangan mencentang pernyataan mandiri atau menekan tombol kirim tanpa izin
tegas.** Pernyataan mandiri (K3L, kesediaan memenuhi standar, KKPR,
pernyataan pajak) mengikat pengguna secara pribadi berikut sanksinya.
Serahkan centangnya, atau minta izin eksplisit lebih dulu.

**Jangan pernah mengetik kata sandi, mengisi OTP, menyelesaikan CAPTCHA,
membuat akun, atau melakukan pembayaran.** Semua itu bagian pengguna.

**Periksa sebelum mengirim, dan periksa lagi setelahnya.** Situs pemerintah
sering diam saat gagal: dropdown yang tampak terpilih ternyata tidak,
unggahan masuk dengan label yang salah, formulir ter-reset tanpa pesan.
Pola ini terjadi berkali-kali dalam satu sesi. Baca ulang layarnya.

**Kalau ragu soal aturan pajak, suruh telepon Kring Pajak 1500200.**
Aturan PPh final dan tenggat masa pernah berubah. Untuk hal yang ada
dendanya, jawaban DJP lebih bernilai daripada tebakan yang percaya diri.

## Alur besar

```
1. AHU          → SK Pengesahan + NPWP Badan   (Rp 50.000, ~1 jam)
2. OSS          → data usaha + lokasi + KBLI
3. Amdalnet     → penapisan lingkungan → SPPL   ← penghambat tersembunyi
4. OSS          → NIB + Sertifikat Standar terbit
5. Coretax      → reset kata sandi + passphrase
6. Bank         → rekening PT + setoran modal 25%
7. AHU          → lapor bukti setoran modal      ← tenggat 60 hari
8. Rutin        → SPT Tahunan tiap 30 April
```

## Tiga tenggat yang menimbulkan denda

| Kewajiban | Tenggat | Sanksi |
|---|---|---|
| **Lapor setoran modal 25% ke AHU** | 60 hari sejak SK terbit | sanksi administratif PP 8/2021 |
| **SPT Tahunan Badan** | 30 April tiap tahun | **denda Rp 1.000.000**, walau nihil |
| Setor PPh Final bulanan | tgl 15 bulan berikutnya | bunga keterlambatan |

Yang paling sering menimpa PT baru adalah SPT Tahunan. Pemiliknya merasa
"belum ada transaksi, belum perlu lapor". Kewajiban lapor melekat pada
NPWP, bukan pada ada-tidaknya omzet.

## Biaya sebenarnya

| Pos | Biaya |
|---|---|
| PNBP pendirian PT Perorangan | **Rp 50.000** |
| NIB, Sertifikat Standar, KKPR, SPPL | Rp 0 |
| NPWP Badan | Rp 0 |
| Akun Coretax | Rp 0 |
| D-U-N-S jalur gratis | Rp 0 |
| Stempel perusahaan | Rp 60.000–150.000 |
| Setoran awal rekening bank badan | bervariasi, cek ke bank |

PT Perorangan tetap **Rp 50.000** meski PP 30/2026 menaikkan PNBP PT biasa
menjadi Rp 5.000.000. Ini keringanan khusus UMK — pastikan pengguna memilih
jalur Perseroan Perorangan, bukan PT biasa.
