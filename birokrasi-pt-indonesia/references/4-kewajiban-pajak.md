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
elektronik** — lihat `3-coretax.md`.

### ⚠️ Jebakan: kasus terbentuk tapi isinya kosong

Terjadi dalam kasus nyata dan sulit dikenali. Setelah memilih AS.06-01 dan
menekan **Lanjut**, sistem langsung membuat nomor kasus dan melompat ke
halaman ringkasan — **tanpa pernah menampilkan formulir permohonannya**.

Terlihat seperti berhasil: ada nomor kasus, ada prioritas "Tinggi", ada
"Penyelesaian yang diharapkan". Padahal tidak ada apa pun yang diisi,
diunggah, atau ditandatangani.

**Ciri kasus kosong** (periksa di *Portal Saya → Kasus Saya → Case Overview*):

| Kolom | Kasus kosong | Permohonan yang sehat |
|---|---|---|
| Status / Portal Status | diam di **"Dibuat"** berhari-hari | berubah, lalu selesai |
| **Tanggal Akhir** | **kosong** | terisi saat selesai |
| **Tindakan Terakhir** | **kosong** | ada jejak |
| Keterangan | hanya *"Kasus Created for … Form …"* | lebih spesifik |
| Muncul di *Permohonan Dalam Proses* / *Telah Selesai* | **tidak** | ya |

Pembanding yang berguna: permohonan **perubahan KLU** melewati formulir
lengkap, unggahan dokumen, pernyataan, dan tombol Simpan — lalu terbit
**keesokan harinya** berikut surat resmi. Kalau sebuah permohonan tidak
pernah meminta satu pun dari itu, curigai.

**Jangan langsung mengajukan ulang.** Kalau yang lama masih hidup di sistem
internal, hasilnya dua permohonan kembar yang justru memperlambat. Telepon
**Kring Pajak 1500200** dengan nomor kasusnya dan tanyakan: apakah
permohonan lengkap, dan bagaimana membatalkannya bila tidak.

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
