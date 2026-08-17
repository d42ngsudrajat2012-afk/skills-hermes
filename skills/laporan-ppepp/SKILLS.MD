---
name: laporan-ppepp-lam-infokom
description: Susun laporan PPEPP LAM INFOKOM berbasis bukti.
version: 0.1.0
author: Pengguna, Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [PPEPP, LAM INFOKOM, LED, akreditasi, assessment, bukti, grafik]
    related_skills: []
---

# Laporan PPEPP LAM INFOKOM

Skill ini digunakan untuk menyusun laporan Pelaksanaan, Evaluasi, Pengendalian, atau Peningkatan kegiatan terkait standar dan indikator kinerja pada instrumen LED LAM INFOKOM. Gunakan alur keterlacakan: **Standar → Indikator Kinerja → Kegiatan → Target → Realisasi → Persentase Capaian → Assessment → Nilai Akhir → RNA → Nilai LED → Bukti → Temuan → Tindakan**.

## When to Use

Gunakan ketika pengguna meminta laporan PPEPP yang:

- ditujukan kepada tim akreditasi Program Studi/UPPS, penjaminan mutu, pimpinan, auditor mutu internal, atau asesor LAM INFOKOM;
- membandingkan target dan realisasi kegiatan;
- menghitung persentase capaian, nilai akhir, RNA, dan selisih dengan nilai LED;
- memerlukan assessment berbobot, audit trail bukti, analisis temuan, grafik, dan tindak lanjut;
- meminta output Markdown, Word, PDF, atau format laporan terstruktur.

Jangan membuat dasar hukum, standar, kebijakan, SOP, SK, nama pejabat, nomor dokumen, hasil AMI, nilai, atau bukti yang tidak diberikan pengguna.

## Data and Evidence Rules

1. Prioritaskan data faktual dari pengguna.
2. Bedakan secara eksplisit **data faktual**, **simulasi**, **asumsi**, **hasil perhitungan**, dan **data yang perlu diverifikasi**.
3. Jika pengguna meminta contoh tetapi data faktual belum tersedia, gunakan data simulasi realistis dan beri label persis:
   **SIMULASI — WAJIB DIGANTI DENGAN DATA FAKTUAL INSTITUSI**.
4. Jangan menyajikan data simulasi sebagai fakta institusi.
5. Jangan menyatakan bukti tersedia, lengkap, atau terverifikasi apabila dokumen belum diberikan.
6. Jika akar penyebab belum terbukti, tulis: **Hipotesis — Perlu Verifikasi**.
7. Jika hasil AMI tidak tersedia, jangan membuat hasil AMI secara spekulatif.
8. Jangan menetapkan toleransi selisih secara sepihak.

## Mode PPEPP

Pilih tepat satu mode, kecuali pengguna meminta laporan terpadu:

| Mode | Fokus | Status default |
| --- | --- | --- |
| Pelaksanaan | Pelaksanaan standar dan kegiatan | Terlaksana / Cukup terlaksana / Belum optimal |
| Evaluasi | Evaluasi target, realisasi, temuan, dan bukti | Tercapai / Cukup tercapai / Belum optimal |
| Pengendalian | Pengendalian deviasi, tindakan korektif, dan RTL | Tercapai / Cukup tercapai / Belum optimal |
| Peningkatan | Perbaikan gap, tindakan peningkatan, dan efektivitas | Tercapai / Cukup tercapai / Belum optimal |

Rubrik status di atas adalah rubrik operasional. Nyatakan bahwa rubrik harus disesuaikan dengan kebijakan institusi apabila tersedia.

## Struktur Laporan

Gunakan urutan berikut:

1. Halaman Judul.
2. Lembar Identitas Dokumen.
3. Halaman Pengesahan.
4. Ringkasan Eksekutif 350–450 kata.
5. Kata Pengantar 350–450 kata.
6. Daftar Isi.
7. **BAB 1 PENDAHULUAN**.
8. **BAB 2 [MODE] KEGIATAN DAN ASSESSMENT**.
9. **BAB 3 KESIMPULAN**.
10. Daftar Lampiran.

## BAB 1 Pendahuluan

### 1.1 Latar Belakang

Untuk Pelaksanaan, jelaskan hubungan standar, indikator kinerja, pelaksanaan, bukti, dan pembuktian capaian LED dalam 350–450 kata. Untuk Evaluasi, jelaskan kebutuhan evaluasi, bukti capaian, dan verifikasi LED. Untuk Pengendalian, jelaskan deviasi, tindakan korektif, RTL, dan pembuktian LED. Untuk Peningkatan, jelaskan hasil evaluasi/pengendalian, gap capaian, tindakan peningkatan, dan pembuktian LED.

### 1.2 Dasar [Pelaksanaan/Evaluasi/Pengendalian/Peningkatan]

Gunakan hanya dasar yang tersedia, seperti standar, kebijakan, SOP, SK, dokumen mutu, hasil monitoring, hasil AMI, RTM, atau RTL sebelumnya. Jika dasar belum tersedia, gunakan placeholder `[DASAR BELUM TERSEDIA]`.

### 1.3 Tujuan

Jelaskan tujuan dokumentasi, pengukuran capaian, assessment, verifikasi nilai LED, identifikasi kesenjangan, tindakan korektif, dan perbaikan berkelanjutan sesuai mode.

### 1.4 Ruang Lingkup

Jelaskan standar, indikator, kegiatan, periode, unit, target, realisasi, bukti, assessment, temuan, tindakan, dan rekonsiliasi LED.

## BAB 2 Isi Standar, Indikator, dan Mekanisme

### 2.1 Pernyataan [Mode] Isi Standar

Tulis dalam paragraf penuh yang memuat isi standar, kondisi atau bentuk kegiatan, pihak terkait, periode, bukti, serta hubungan dengan indikator kinerja.

### 2.2 Indikator Kinerja

Gunakan tabel:

```markdown
| No. | Indikator Kinerja | Definisi Operasional | Target | Realisasi | Satuan | Sumber Data/Bukti |
| --- | --- | --- | ---: | ---: | --- | --- |
```

Tulis rumus dalam LaTeX:

$$
\text{Persentase Capaian} = \frac{\text{Realisasi}}{\text{Target}} \times 100\%
$$

Hindari pembagian dengan nol. Untuk target kualitatif, gunakan rubrik yang terdefinisi. Jika target tidak tersedia, jangan menghitung secara spekulatif. Tampilkan hasil maksimal dua angka desimal.

### 2.3 Mekanisme Kegiatan

Tulis mekanisme dalam paragraf penuh, bukan hanya daftar. Gunakan alur sesuai mode:

- Pelaksanaan: Perencanaan → Penetapan Target → Pelaksanaan → Pengumpulan Bukti → Monitoring → Evaluasi → Assessment → Tindak Lanjut → Dokumentasi.
- Evaluasi: Penetapan Standar → Penetapan Indikator → Pengumpulan Data → Verifikasi Bukti → Perbandingan Target–Realisasi → Evaluasi → Assessment → Analisis Temuan → AMI/Tindak Lanjut → Dokumentasi.
- Pengendalian: Penetapan Standar → Monitoring → Evaluasi Target–Realisasi → Identifikasi Deviasi → Analisis Akar Penyebab → Tindakan Korektif → Pengendalian → RTL → Monitoring RTL → Verifikasi Efektivitas → Dokumentasi.
- Peningkatan: Hasil Evaluasi/Pengendalian → Identifikasi Gap → Analisis Akar Penyebab → Sasaran Peningkatan → Perencanaan → Pelaksanaan → Monitoring → Assessment → Verifikasi Efektivitas → RTL → Dokumentasi.

## Tabel Kegiatan

Turunkan indikator menjadi jumlah kegiatan yang logis dan relevan. Gunakan kolom bentuk sesuai mode:

```markdown
| No. | Nama Kegiatan | Bentuk [Pelaksanaan/Evaluasi/Pengendalian/Peningkatan] | Target | Realisasi | Persentase Capaian | Status |
| --- | --- | --- | ---: | ---: | ---: | --- |
```

Gunakan klasifikasi operasional:

- Realisasi > Target: Terlaksana/Tercapai/Terkendali sesuai mode.
- Realisasi = Target: Cukup terlaksana/Cukup tercapai/Cukup terkendali.
- Realisasi < Target: Belum optimal.

## Data dan Grafik

Sediakan tabel data grafik:

```markdown
| Kegiatan | Target | Realisasi | Persentase Capaian |
| --- | ---: | ---: | ---: |
```

Rekomendasikan grafik batang berkelompok untuk target vs realisasi, grafik batang untuk persentase capaian, grafik garis untuk beberapa periode, atau grafik kombinasi untuk nilai absolut dan persentase.

Setiap grafik wajib memiliki judul, label sumbu X, label sumbu Y, legenda, label/data nilai, sumber data, dan interpretasi sekitar 150 kata. Jika platform mendukung gambar, buat grafik yang benar-benar konsisten dengan tabel. Jika tidak, berikan tabel siap grafik atau kode grafik dan jangan mengklaim gambar telah dibuat.

## Assessment Kegiatan

### 2.5.1 Komponen Penilaian

Buat tepat lima komponen, bukan lima kegiatan. Jika komponen resmi tidak diberikan, gunakan komponen sesuai mode:

- Pelaksanaan: Perencanaan; Keterlaksanaan; Kualitas Pendampingan; Dukungan Sumber Daya; Dokumentasi dan Tindak Lanjut.
- Evaluasi: Perencanaan Evaluasi; Pelaksanaan Evaluasi; Validitas Data; Analisis Temuan; Tindak Lanjut.
- Pengendalian: Monitoring; Analisis Deviasi; Tindakan Korektif; Efektivitas Pengendalian; RTL.
- Peningkatan: Ketercapaian Target Peningkatan; Relevansi Tindakan; Kelengkapan dan Validitas Bukti; Efektivitas Hasil; Keberlanjutan dan Integrasi.

```markdown
| No. | Komponen | Definisi Operasional | Indikator Bukti |
| --- | --- | --- | --- |
```

### 2.5.2 Bobot Penilaian

```markdown
| No. | Komponen | Bobot (%) | Bobot Desimal | Alasan Pembobotan |
| --- | --- | ---: | ---: | --- |
```

Verifikasi bahwa jumlah Bobot (%) = 100% dan jumlah Bobot Desimal = 1,00. Bobot Desimal = Bobot (%) ÷ 100.

### 2.5.3 Rubrik Skor

Jika rubrik resmi tidak tersedia, gunakan:

| Skor | Kriteria |
| ---: | --- |
| 80–100 | Sangat baik: seluruh persyaratan terpenuhi dan didukung bukti lengkap |
| 60–79 | Baik: sebagian besar persyaratan terpenuhi dan bukti memadai |
| 40–59 | Cukup: persyaratan terpenuhi sebagian dan bukti masih terbatas |
| 20–39 | Kurang: hanya sedikit persyaratan terpenuhi |
| 0–19 | Tidak tersedia/tidak terlaksana/tidak ada bukti |

Semua skor komponen harus berupa bilangan bulat 0–100.

### 2.5.4 Assessment Penilaian

B1–B5 adalah lima komponen penilaian. Isi penilaian untuk seluruh kegiatan:

```markdown
| No. | Nama Kegiatan | B1 | B2 | B3 | B4 | B5 | Nilai Akhir |
| --- | --- | ---: | ---: | ---: | ---: | ---: | ---: |
```

Gunakan rumus:

$$
NA_i = (w_1 \times Nilai_{i1}) + (w_2 \times Nilai_{i2}) + (w_3 \times Nilai_{i3}) + (w_4 \times Nilai_{i4}) + (w_5 \times Nilai_{i5})
$$

$$
\sum_{j=1}^{5} w_j = 1{,}00
$$

$$
RNA = \frac{NA_1 + NA_2 + \cdots + NA_n}{n}
$$

Bulatkan Nilai Akhir dan RNA menjadi dua angka di belakang koma. Tampilkan minimal satu contoh perhitungan lengkap. Jangan merekayasa skor agar RNA sama dengan nilai LED; jika berbeda, laporkan perbedaannya.

### 2.5.5 Dasar Pemberian Skor

Gunakan audit trail:

```markdown
| Kegiatan | Komponen | Skor | Bukti/Data | Alasan Pemberian Skor | Status Bukti |
| --- | --- | ---: | --- | --- | --- |
```

Status bukti: Tersedia, Sebagian tersedia, Belum tersedia, atau Perlu Verifikasi. Setiap skor harus dapat ditelusuri ke data atau bukti.

### 2.5.6 Rekonsiliasi Nilai LED

```markdown
| Komponen | Nilai |
| --- | ---: |
| Target Indikator |  |
| Realisasi Indikator |  |
| Hasil Perhitungan Capaian |  |
| Hasil Assessment/RNA |  |
| Nilai Capaian dalam LED |  |
| Selisih Assessment dengan LED |  |
| Status Kesesuaian |  |
```

$$
\text{Selisih} = \text{Hasil Assessment} - \text{Nilai Capaian LED}
$$

Gunakan status **Sesuai** jika selisih = 0, **Perlu Verifikasi** jika ada selisih tetapi penyebab belum dapat dipastikan, dan **Tidak Sesuai** jika perhitungan serta bukti menunjukkan nilai berbeda. Pastikan semua nilai berada pada skala yang sebanding.

### 2.5.7 Grafik Hasil Assessment

Sediakan tabel:

```markdown
| Kegiatan | Nilai Assessment | Nilai LED/Target |
| --- | ---: | ---: |
```

Grafik wajib memiliki judul, label sumbu, legenda, label/data nilai, dan sumber data. Interpretasikan kegiatan dengan nilai tertinggi dan terendah, komponen paling berpengaruh, gap terhadap target, serta implikasi terhadap indikator. Rekomendasikan grafik batang assessment per kegiatan, radar B1–B5, atau kombinasi assessment vs LED.

### 2.5.8 Analisis

Gunakan tabel sesuai mode:

```markdown
| No. | Temuan/Kendala | Akar Penyebab | Dampak terhadap Indikator | Tindakan Korektif | RTL/Tindakan Peningkatan |
| --- | --- | --- | --- | --- | --- |
```

Tindakan korektif harus menjawab temuan, RTL harus menjawab akar penyebab, dan tindakan peningkatan harus membawa kondisi menuju capaian yang lebih baik. Jika tersedia, sertakan PIC, target waktu, indikator keberhasilan, dan bukti penyelesaian.

## BAB 3 Kesimpulan

Tulis kesimpulan dalam paragraf penuh. Jelaskan tingkat pelaksanaan/evaluasi/pengendalian/peningkatan, ketercapaian target, hasil assessment, RNA, hubungan RNA dengan LED, bukti pendukung, temuan utama, serta tindakan yang diperlukan. Jika assessment sama dengan LED, jelaskan alur pembuktiannya. Jika berbeda, jangan memaksakan kesimpulan “Sesuai”.

## Daftar Lampiran

Susun daftar bukti yang relevan, misalnya standar, indikator, rekap target–realisasi, bukti kegiatan, instrumen assessment, audit trail, hasil AMI jika tersedia, notulen, dokumentasi, tindakan korektif, RTL, monitoring RTL, dan rekap nilai. Jangan mengklaim lampiran tersedia jika belum diberikan.

## Procedure

1. Pilih satu mode PPEPP dan catat konteks institusi, unit, periode, standar, indikator, target, dan LED. **Selesai jika mode dan data inti jelas.**
2. Pisahkan data faktual, simulasi, asumsi, dan data yang perlu diverifikasi. **Selesai jika setiap angka memiliki label sumber.**
3. Susun BAB 1, pernyataan standar, indikator, dan mekanisme dalam paragraf penuh. **Selesai jika alur mode lengkap.**
4. Turunkan indikator menjadi kegiatan dan hitung capaian tanpa pembagian dengan nol. **Selesai jika nama kegiatan konsisten di seluruh tabel.**
5. Buat tabel data grafik dan grafik berlabel. **Selesai jika grafik cocok dengan data dan memiliki sumber.**
6. Buat lima komponen, bobot 100%/1,00, rubrik, assessment, dan contoh perhitungan. **Selesai jika NA dan RNA dihitung ulang.**
7. Buat audit trail, rekonsiliasi LED, dan status kesesuaian. **Selesai jika setiap skor memiliki bukti atau status verifikasi.**
8. Analisis temuan, akar penyebab, tindakan korektif, RTL, dan tindakan peningkatan sesuai mode. **Selesai jika tindakan menjawab temuan.**
9. Tulis kesimpulan paragraf penuh dan daftar lampiran. **Selesai jika tidak ada klaim tanpa bukti.**
10. Jalankan checklist verifikasi sebelum menyerahkan laporan.

## Pitfalls

- Jangan mengubah simulasi menjadi fakta.
- Jangan membuat sumber, nomor dokumen, pejabat, hasil AMI, atau kebijakan fiktif.
- Jangan menghitung persentase dengan target nol atau target yang tidak tersedia.
- Jangan memberikan skor tanpa dasar bukti.
- Jangan membuat RNA sama dengan LED melalui manipulasi nilai.
- Jangan membandingkan skala penilaian yang tidak sebanding.
- Jangan menggunakan toleransi selisih yang tidak ditetapkan institusi.
- Jangan menyimpulkan akar masalah tanpa data.
- Jangan mengklaim grafik atau lampiran tersedia jika belum dibuat atau diberikan.

## Verification

- [ ] Mode PPEPP konsisten di seluruh laporan.
- [ ] Struktur halaman awal, BAB 1, BAB 2, BAB 3, dan lampiran lengkap.
- [ ] Data faktual dan simulasi diberi label.
- [ ] Target, realisasi, satuan, dan sumber data tersedia atau diberi placeholder.
- [ ] Tidak ada pembagian dengan nol.
- [ ] Persentase capaian benar dan maksimal dua desimal.
- [ ] Total bobot = 100% dan bobot desimal = 1,00.
- [ ] Semua skor komponen berada pada 0–100 dan berbentuk bilangan bulat.
- [ ] NA dan RNA telah dihitung ulang.
- [ ] Audit trail memuat bukti, alasan, dan status bukti.
- [ ] Rekonsiliasi LED memuat selisih dan status yang tidak dipaksakan.
- [ ] Grafik memiliki judul, label sumbu, legenda, label nilai, dan sumber data.
- [ ] Nama kegiatan konsisten di tabel, grafik, narasi, dan kesimpulan.
- [ ] Akar penyebab yang belum terbukti diberi label “Hipotesis — Perlu Verifikasi”.
- [ ] Tindakan korektif, RTL, dan tindakan peningkatan relevan dengan temuan.
- [ ] Tidak ada klaim lampiran, AMI, atau bukti yang belum diberikan.

## Source

Skill ini disusun dari file PDF `2b._UPLOAD_PROMPT_TULIS_LAPORAN_PELAKSANAAN_KEGIATAN.pdf` yang memuat prompt terstruktur C-O-S-T-A-R untuk laporan Pelaksanaan, Evaluasi, Pengendalian, dan Peningkatan terkait standar serta indikator kinerja LED LAM INFOKOM.

## Publishing from Hermes WebUI

Untuk meminta Hermes WebUI memublikasikan skill, gunakan instruksi:

> Validasi skill `/workspace/laporan-ppepp-lam-infokom`, periksa bahwa tidak ada rahasia, lalu jalankan `hermes skills publish /workspace/laporan-ppepp-lam-infokom`. Tampilkan hasil, ID, atau URL publikasinya. Jika CLI Hermes tidak tersedia, jangan mengklaim publikasi berhasil; berikan perintah yang harus saya jalankan di terminal.

Publikasi hanya berhasil jika executable `hermes` tersedia di environment yang menjalankan perintah dan layanan publikasi/akun yang diperlukan telah dikonfigurasi.

## Sharing without Publishing

Jika publikasi resmi tidak tersedia, bagikan file `SKILL.md` atau folder skill melalui ZIP, GitHub, atau penyimpanan cloud. Penerima dapat memasangnya pada:

```text
~/.hermes/skills/laporan-ppepp-lam-infokom/SKILL.md
```

Setelah pemasangan, mulai sesi Hermes baru agar skill dimuat.

## Source

Skill ini disusun dari PDF prompt laporan PPEPP LAM INFOKOM yang diunggah pengguna. Data institusi tidak ditambahkan ke dalam skill.

## Verification

Sebelum publikasi, pastikan file dimulai dengan frontmatter `---`, memiliki `name` dan `description`, berisi instruksi setelah frontmatter, tidak menyimpan rahasia, dan seluruh contoh data diberi label simulasi jika digunakan.

## Common Pitfalls

- `hermes skills publish` tidak sama dengan membagikan file ZIP.
- Jangan menyatakan publikasi berhasil tanpa ID atau URL hasil publikasi.
- Jika WebUI menampilkan `hermes: command not found`, jalankan publikasi dari terminal instalasi Hermes yang benar.
- Skill yang baru dibuat mungkin belum muncul pada sesi saat ini sampai sesi baru dimulai.

## Verification

Validasi akhir harus mencakup struktur frontmatter, isi Markdown, ukuran file, ketiadaan rahasia, dan ketersediaan folder skill sebelum publikasi.

## Source

Sumber: `2b._UPLOAD_PROMPT_TULIS_LAPORAN_PELAKSANAAN_KEGIATAN.pdf`.

## Notes

Jangan menampilkan proses berpikir internal. Tampilkan hanya laporan, data, rumus, perhitungan, grafik yang didukung platform, interpretasi, temuan, tindakan, dan catatan verifikasi yang relevan.

## End

Skill selesai.

## Verification Checklist

- [ ] Laporan dapat diaudit dari standar sampai bukti.
- [ ] Data simulasi tidak dianggap fakta.
- [ ] Semua perhitungan konsisten.
- [ ] Grafik berlabel dan konsisten dengan tabel.
- [ ] Kesimpulan berupa paragraf penuh.
- [ ] Publikasi dilaporkan hanya jika benar-benar menghasilkan ID atau URL.

## Source

Materi sumber adalah PDF yang diunggah pengguna pada sesi ini.

## Final Rule

Jika data belum cukup, gunakan placeholder dan minta data yang diperlukan; jangan mengarang.
