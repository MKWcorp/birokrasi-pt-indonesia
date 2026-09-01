# 4 — Kewajiban pajak rutin & pembukuan

> ⚠️ Aturan PPh final dan tenggat masa pernah berubah. Isi berkas ini adalah
> kerangka, bukan pengganti konfirmasi. Untuk hal yang ada dendanya, suruh
> pengguna menelepon **Kring Pajak 1500200** dan menanyakan **kewajiban pajak
> apa saja yang terdaftar untuk NPWP mereka**.

## ⚠️ Badan wajib PEMBUKUAN, bukan pencatatan

Ini beda mendasar yang sering terlewat.

Orang pribadi tertentu boleh sekadar **mencatat** peredaran usaha. **Badan
tidak.** UU KUP mewajibkan badan menyelenggarakan **pembukuan** lengkap —
minimal **neraca** dan **laporan laba rugi**, dalam bahasa Indonesia dan
rupiah, disimpan **10 tahun**.

**Tarif final 0,5% tidak menghapus kewajiban ini.** Tarif finalnya
menyederhanakan cara menghitung pajak, bukan cara membukukan. SPT Tahunan
Badan tetap meminta neraca dan laba rugi.

## Kewajiban rutin

| Jenis | Frekuensi | Tenggat | Kapan berlaku |
|---|---|---|---|
| **SPT Tahunan Badan** | tahunan | **30 April** | **selalu, walau nihil** |
| PPh Final 0,5% | bulanan | tgl 15 bulan berikutnya | kalau ada omzet |
| PPh 21 | bulanan | tgl 10 / 20 | kalau menggaji orang |
| PPh 23 | bulanan | tgl 10 / 20 | kalau membayar jasa ke pihak lain |
| PPN | bulanan | — | hanya kalau sudah PKP |

**Denda telat SPT Tahunan Badan: Rp 1.000.000.** Berlaku walau perusahaan
belum berjalan. Ini denda yang paling sering menimpa PT baru.

**Setoran PPh final = pelaporannya.** Setoran yang tervalidasi (ada NTPN)
sudah dianggap SPT Masa; tidak ada formulir terpisah. Bulan tanpa omzet
berarti tidak ada yang disetor dan tidak ada yang dilapor.

## PKP: jangan diajukan terlalu dini

Pengukuhan PKP baru wajib saat omzet melewati **Rp 4,8 miliar setahun**.
Menjadi PKP berarti wajib memungut, menyetor, dan melaporkan PPN tiap bulan.
Jangan mengajukannya "biar terlihat profesional".

## Suket PPh Final 0,5% (PP 55/2022)

Layanan **AS.06-01** di Coretax:
*Layanan WP → Layanan Administrasi → Buat Permohonan Layanan Administrasi*

⚠️ **Jangan tertukar dengan AS.06-02** — itu justru pernyataan **memilih
tarif umum**, alias melepaskan fasilitas 0,5%.

**Kenapa Suket ini penting secara nyata:** tanpa Suket, klien korporat
memotong **PPh 23 sebesar 2% dari bruto** tiap kali membayar. Dengan Suket,
pemotongnya cukup **0,5% final**. Selisih empat kali lipat, langsung terasa
di arus kas tiap invoice.

**Batasan:** untuk badan berbentuk PT, fasilitas 0,5% berlaku **maksimal 3
tahun pajak** (orang pribadi 7 tahun). Jam-nya berjalan sejak tahun pertama.

⚠️ Permohonan ini menuntut **peran Wakil** dan **passphrase sertifikat
elektronik** — lihat `3-coretax.md`. Kalau kasus terbentuk tapi statusnya
diam di **"Dibuat"** dan tidak muncul di *Permohonan Dalam Proses* maupun
*Permohonan Telah Selesai*, kemungkinan formulirnya tidak pernah benar-benar
tersimpan. Suruh cek ke Kring Pajak dengan nomor kasusnya sebelum mengajukan
ulang — jangan sampai ada dua permohonan kembar.

## Bisa diotomatiskan?

**Pelaporannya tidak.** Coretax tidak punya penjadwalan otomatis dan tidak
ada yang melapor mewakili pengguna. Yang bisa diotomatiskan hanya
**pencatatannya**.

Tiga tingkat yang realistis:

| Cara | Cocok untuk | Kisaran biaya |
|---|---|---|
| Spreadsheet disiplin | PT satu orang, transaksi sedikit | Rp 0 |
| Software akuntansi (Kledo, Mekari Jurnal, Accurate, Zahir) | transaksi puluhan/bulan | ratusan ribu/bulan |
| Jasa pembukuan / konsultan pajak | ingin aman & tidak mau pusing | Rp 500rb–2jt/bulan |

## Aturan yang menyelamatkan pembukuan

**Pisahkan uang PT dari uang pribadi sejak rekening dibuka.** Begitu
tercampur, pembukuan tidak bisa diselamatkan tanpa kerja berlipat — dan
kalau diperiksa, seluruh pemasukan di rekening itu berpotensi dianggap
penghasilan PT.

Setoran modal wajib justru transaksi pertama yang bagus: uang masuk dari
pemilik, tercatat sebagai setoran modal.
