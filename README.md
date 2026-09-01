# Birokrasi PT Indonesia

Panduan lapangan menembus birokrasi **PT Perorangan** di Indonesia —
dari belum punya apa-apa sampai perusahaan benar-benar bisa beroperasi
dan patuh pajak.

Dikemas sebagai *skill* yang bisa dipakai Claude Code, Claude.ai, atau
asisten AI lain. Ditulis dari **satu pendirian yang benar-benar
dijalankan**, biaya resmi total **Rp 50.000**.

## Yang bisa dikerjakan dengan skill ini

| Urusan | Hasil |
|---|---|
| **Mendirikan PT Perorangan** di AHU Online | SK Pengesahan Kemenkumham + NPWP Badan terbit otomatis |
| **Mengurus izin berusaha** di OSS RBA | Kegiatan usaha, KBLI 2025, KKPR, Sertifikat Standar, **NIB** |
| **Penapisan lingkungan** di Amdalnet | SPPL — syarat tersembunyi yang menahan NIB |
| **Mengaktifkan akun Coretax DJP** | akses akun badan & pribadi, passphrase sertifikat elektronik |
| **Memperbaiki KLU** yang tercatat salah | Surat Pemberitahuan Perubahan Data |
| **Mengajukan Suket PPh Final 0,5%** | layanan AS.06-01 (PP 55/2022) |
| **Memahami kewajiban lapor & pembukuan** | SPT Tahunan, PPh masa, pembukuan badan |
| **Setoran modal 25%** | lapor ke AHU sebelum tenggat 60 hari |
| **Membuka rekening bank atas nama PT** | dokumen, urutan, jebakan setoran awal |
| **Mendaftar nomor D-U-N-S** | Dun & Bradstreet, termasuk jalur gratis |

Setiap tahap punya berkas rujukannya sendiri. Asisten membaca `SKILL.md`
dulu, lalu membuka berkas yang relevan dengan tahap penggunanya — bukan
memuat semuanya sekaligus.

## Isi

```
birokrasi-pt-indonesia/
├── SKILL.md                      alur besar, tenggat, prinsip kerja
└── references/
    ├── 1-pendirian-ahu.md        SK Pengesahan + NPWP Badan
    ├── 2-perizinan-oss.md        NIB, KBLI, Amdalnet, SPPL
    ├── 3-coretax.md              akun pajak, KLU, peran Wakil
    ├── 4-kewajiban-pajak.md      SPT, pembukuan, PPh Final 0,5%
    ├── 5-rekening-bank.md        rekening PT + setoran modal 25%
    ├── 6-duns.md                 nomor D-U-N-S untuk pasar global
    └── jebakan.md                gejala → penyebab
```

## Cara pakai

**Claude Code**

```bash
git clone https://github.com/MKWcorp/birokrasi-pt-indonesia.git
mkdir -p ~/.claude/skills
cp -r birokrasi-pt-indonesia/birokrasi-pt-indonesia ~/.claude/skills/birokrasi-pt-indonesia
```

Lalu bertanya seperti biasa — *"bantu saya mendirikan PT Perorangan"*,
*"NIB saya masih draft kenapa ya"*, *"cara aktivasi Coretax"*, *"daftar
DUNS number"* — skill akan terpanggil sendiri.

**Claude.ai / ChatGPT / asisten lain**

Unggah `birokrasi-pt-indonesia/SKILL.md` beserta berkas di `references/`
sebagai lampiran, atau tempel isinya ke percakapan.

## Yang membedakan dari panduan resmi

Urutan langkah sudah ada di situs pemerintah. Yang tidak ada di mana pun
adalah **hal yang menghentikan proses di tengah jalan** — dan itu isi
`references/jebakan.md`: gejala yang terlihat di layar, dipetakan ke
penyebab sebenarnya.

Contohnya, NIB yang berstatus *Draft* tanpa penjelasan ternyata tertahan
penapisan lingkungan, bukan antrean petugas. Ada belasan pola serupa,
semuanya ditemukan dengan cara tersangkut lebih dulu.

## Tiga tenggat yang menimbulkan denda

| Kewajiban | Tenggat | Sanksi |
|---|---|---|
| Lapor setoran modal 25% ke AHU | 60 hari sejak SK terbit | sanksi administratif PP 8/2021 |
| **SPT Tahunan Badan** | **30 April tiap tahun** | **denda Rp 1.000.000, walau nihil** |
| Setor PPh Final bulanan | tgl 15 bulan berikutnya | bunga keterlambatan |

## Batasan

Panduan ini **bukan nasihat hukum atau perpajakan profesional.** Isinya
pengalaman lapangan satu perusahaan, dan aturan bisa berubah.

Untuk hal yang ada dendanya, konfirmasi ke sumbernya: **Kring Pajak
1500200**, KPP terdaftar, atau konsultan pajak. Bagian yang tidak
sepenuhnya pasti sudah ditandai di dalam berkasnya.

Menemukan yang sudah tidak berlaku? Kirim *issue* atau *pull request* —
skill ini memang dimaksudkan untuk terus diperbarui.

## Pagar untuk asisten AI

Ditulis tegas di dalam skill: jangan mengarang data untuk formulir negara,
jangan membuatkan bukti fisik, jangan mencentang pernyataan mandiri atau
menekan tombol kirim tanpa izin tegas, dan jangan mengetik kata sandi, OTP,
CAPTCHA, membuat akun, atau melakukan pembayaran.

Semua itu tanggung jawab pemilik perusahaan, bukan asistennya.

## Lisensi

MIT — pakai, ubah, sebarkan.
