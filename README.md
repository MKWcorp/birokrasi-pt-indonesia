# Birokrasi PT — pendirian sampai patuh pajak

Panduan lapangan untuk mendirikan **PT Perorangan** di Indonesia dan
mengurus kewajiban pajaknya, dikemas sebagai *skill* yang bisa dipakai
Claude Code, Claude.ai, atau asisten AI lain.

Ditulis dari **satu pendirian yang benar-benar dijalankan** — dari belum
punya apa-apa sampai NIB terbit, NPWP aktif, akun Coretax hidup, KLU
diperbaiki, dan permohonan D-U-N-S terkirim. Biaya resmi total:
**Rp 50.000**.

## Kenapa ini ada

Situs resmi sudah menjelaskan urutan langkahnya. Yang tidak dijelaskan
di mana pun adalah **hal-hal yang menghentikan proses di tengah jalan**:

- NIB berstatus *Draft* tanpa penjelasan — ternyata penghambatnya
  **penapisan lingkungan di Amdalnet**, bukan antrean petugas
- Coretax menolak aktivasi karena **akunnya sudah dibuat otomatis**;
  yang dibutuhkan reset kata sandi, bukan aktivasi
- Semua permohonan layanan pajak diam tanpa pesan galat karena
  **passphrase sertifikat elektronik** belum ditetapkan
- **KLU tercatat salah** karena sistem mengambil KBLI bernomor terkecil
- PT Perorangan **tidak punya Akta Pendirian notaris**, dan hampir semua
  formulir bank meminta dokumen itu
- Jalur **D-U-N-S gratis** tampak mustahil untuk perusahaan baru, padahal
  D&B memberi keringanan bila ditanya

Semuanya terdokumentasi di `birokrasi-pt/references/jebakan.md`.

## Isi

```
birokrasi-pt/
├── SKILL.md                      alur besar, tenggat, prinsip kerja
└── references/
    ├── 1-pendirian-ahu.md        SK Pengesahan + NPWP Badan
    ├── 2-perizinan-oss.md        NIB, KBLI, Amdalnet, SPPL
    ├── 3-coretax.md              akun pajak, KLU, peran Wakil
    ├── 4-kewajiban-pajak.md      SPT, pembukuan, PPh Final 0,5%
    ├── 5-rekening-bank.md        rekening PT + setoran modal 25%
    ├── 6-duns.md                 nomor D-U-N-S untuk pasar global
    └── jebakan.md                gejala → penyebab, batas yang tak boleh dilewati
```

## Cara pakai

**Claude Code**

```bash
git clone https://github.com/MKWcorp/birokrasi-pt.git
mkdir -p ~/.claude/skills
cp -r birokrasi-pt/birokrasi-pt ~/.claude/skills/birokrasi-pt
```

Lalu cukup bertanya seperti biasa — *"bantu saya mendirikan PT Perorangan"*,
*"NIB saya masih draft kenapa ya"*, *"cara aktivasi Coretax"* — skill akan
terpanggil sendiri.

**Claude.ai / ChatGPT / asisten lain**

Unggah `birokrasi-pt/SKILL.md` beserta berkas di `references/` sebagai
lampiran, atau tempel isinya ke dalam percakapan.

## Tiga tenggat yang menimbulkan denda

| Kewajiban | Tenggat | Sanksi |
|---|---|---|
| Lapor setoran modal 25% ke AHU | 60 hari sejak SK terbit | sanksi administratif PP 8/2021 |
| **SPT Tahunan Badan** | **30 April tiap tahun** | **denda Rp 1.000.000, walau nihil** |
| Setor PPh Final bulanan | tgl 15 bulan berikutnya | bunga keterlambatan |

## Batasan penting

Panduan ini **bukan nasihat hukum atau perpajakan profesional.** Isinya
pengalaman lapangan satu perusahaan, dan aturan bisa berubah.

Untuk hal yang ada dendanya, konfirmasi ke sumbernya:
**Kring Pajak 1500200**, KPP terdaftar, atau konsultan pajak.

Bagian yang tidak sepenuhnya pasti sudah ditandai di dalam berkasnya.
Kalau menemukan yang sudah tidak berlaku, kirim *issue* atau *pull request* —
skill ini memang dimaksudkan untuk terus diperbarui.

## Prinsip yang ditegakkan skill ini

Untuk asisten AI yang memakainya, ada batas yang ditulis tegas di dalam:
jangan mengarang data untuk formulir negara, jangan membuatkan bukti fisik,
jangan mencentang pernyataan mandiri atau menekan tombol kirim tanpa izin
tegas, dan jangan mengetik kata sandi, OTP, CAPTCHA, atau melakukan
pembayaran.

Semua itu tanggung jawab pemilik perusahaan, bukan asistennya.

## Lisensi

MIT — pakai, ubah, sebarkan.
