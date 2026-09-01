# 6 — Nomor D-U-N-S (Dun & Bradstreet)

Pengenal 9 digit yang dipakai di 200+ negara. Diminta oleh banyak korporasi
global untuk menjadi pemasok, dan oleh sebagian program pengembang
(Apple, Google).

## ⚠️ Di Indonesia lewat mitra lokal, bukan dnb.com

Alur global melempar ke **PT D&B Indonesia**:
`dnb.co.id` (informasi) dan **`dis.dnb.co.id`** (portal pendaftaran).

⚠️ **Peringatan resmi dari D&B Indonesia sendiri:** pendaftaran hanya lewat
situs resmi mereka. Mereka **tidak pernah** mengarahkan pembayaran ke
rekening perorangan — hanya ke Virtual Account atas nama perusahaan pemohon
atau rekening PT D&B Indonesia. Jangan beli jasa DUNS lewat marketplace.

## Tiga paket

| | Dapat | Waktu | Biaya |
|---|---|---|---|
| **Gold** | Digital Seal + sertifikat | 2 hari kerja | berbayar |
| **Silver** | sertifikat softcopy | 10 hari kerja | berbayar |
| **Bronze** | **hanya nomor DUNS** | 30 hari kerja | **gratis** |

Harga Gold/Silver tidak ditampilkan sampai paket dipilih.

## Syarat dokumen

| # | Gold | Silver | Bronze |
|---|---|---|---|
| 1 | NIB/SIUP/TDP | Profil Perusahaan | Profil Perusahaan |
| 2 | Tax ID (NPWP) | NIB/SIUP/TDP | NIB/SIUP/TDP |
| 3 | SK Kehakiman | Tax ID (NPWP) | Tax ID (NPWP) |
| 4 | Form DRS | Akta Pendirian | Akta Pendirian |
| 5 | | SK Kehakiman | SK Kehakiman |
| 6 | | Form DRS | Form DRS |
| 7 | | | Laporan Keuangan / Pajak |
| 8 | | | AR Data / Trade data paydex |

⚠️ **Gold tidak meminta Akta Pendirian** — kebetulan yang menguntungkan
PT Perorangan, yang memang tidak punya akta notaris.

## ⚠️ Perusahaan baru tetap bisa lewat jalur gratis

Syarat Bronze mencantumkan laporan keuangan 3 tahun dan AR data — mustahil
bagi perusahaan berumur hari. **Tapi D&B Indonesia memberi keringanan bila
ditanya:**

- **Laporan keuangan → diganti NIB**
- **AR data → tetap diunggah, tapi templatenya dibiarkan kosong**

Jadi jangan langsung menyimpulkan jalur gratis tertutup. **Tanya dulu lewat
widget WhatsApp di dashboard mereka.**

## Form DRS

Formulir milik D&B, wajib untuk ketiga paket, dan **tidak ada tombol
unduhnya di portal**. Minta lewat WhatsApp — mereka mengirimkan berkasnya.
Isi halaman 1 saja, tanda tangani, unggah.

Kolomnya: nama perusahaan, alamat, telepon, fax, email, website, tanggal
berdiri, jumlah karyawan, line of business, nama direktur, centang
**New**, dan tanda tangan.

## ⚠️ Dropdown Document Type bisa digulir

Daftar jenis dokumen tampak berisi 7 pilihan dan berhenti di *Financial
Reports*. **Panelnya punya bilah gulir.** Di bawahnya masih ada
**AR Data/Trade data paydex** dan **Other** — total 9.

Ini pernah menyebabkan kesimpulan keliru bahwa AR Data tidak punya slot.
**Gulir dulu sebelum menyimpulkan sesuatu tidak ada.**

## ⚠️ Pastikan label unggahan benar

Jenis dokumen **harus benar-benar terpilih sebelum berkas dikirim**. Kalau
dropdown belum berpindah, berkas terunggah dengan label salah dan
**menimpa** entri sebelumnya yang berlabel sama.

Dropdown-nya juga tidak mau menerima ketikan kalau kolomnya sudah berisi:
**kosongkan dulu**, baru ketik kata kunci, baru klik hasilnya. Setelah tiap
unggahan, **baca tabel dokumen** dan pastikan nama berkas dan labelnya
berpasangan benar.

## Website perusahaan sangat membantu

Verifikator memeriksa keberadaan perusahaan. Situs dengan **nama badan
hukum, alamat terdaftar, telepon, dan NIB di footer setiap halaman** plus
JSON-LD `Organization` mengubah klaim menjadi sesuatu yang bisa dicek.

Email berdomain sendiri (`hello@domain.id`) jauh lebih kuat daripada Gmail
saat tahap validasi.
