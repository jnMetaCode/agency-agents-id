# Panduan kontribusi

Terima kasih sudah tertarik untuk berkontribusi! Perbaikan terjemahan, koreksi, agent baru untuk pasar Indonesia — semua bentuk kontribusi welcome.

## Apa yang bisa Anda lakukan

### 1. Perbaiki terjemahan

184 agent upstream diterjemahkan secara batch dengan Claude Sonnet. Kalau ketemu kalimat yang kurang natural atau tidak sesuai gaya bahasa Indonesia formal teknis, silakan PR.

Catatan saat menerjemahkan:
- Jangan terjemahkan kata per kata — pakai Bahasa Indonesia natural dengan register teknis profesional
- Komentar di dalam blok kode juga diterjemahkan
- Pertahankan format frontmatter (name, description, color, emoji, vibe)
- Istilah teknis Inggris (TensorFlow, PyTorch, RAG, MLOps, LLM, API, OAuth, REST, dll.) tetap dalam Inggris
- Blok kode, path file, URL, command (cat, ls, grep, git, npm) tidak diubah

### 2. Buat agent khusus pasar Indonesia

PR untuk agent dengan platform atau skenario Indonesia sangat dipersilakan:

- **Platform**: WhatsApp Business / Cloud API, Instagram ID, TikTok ID
- **E-commerce**: Tokopedia seller, Shopee ID, Bukalapak, Blibli, Lazada ID
- **Super App**: Gojek / GoTo, Grab Indonesia, Traveloka
- **Fintech**: OVO, GoPay, DANA, ShopeePay, QRIS, BI-FAST
- **Compliance**: UU PDP, OJK regulations, Kominfo
- **Vertikal**: Halal e-commerce, Edutech ID, Pertanian digital

### 3. Perbaiki konten yang ada

Terjemahan tidak akurat, contoh kode usang, atau ungkapan yang lebih baik — perbaiki saja.

## Format file agent

```markdown
---
name: Nama Agent
description: Satu kalimat tentang apa yang dilakukan agent ini
color: nama warna (atau #HEX)
emoji: emoji
vibe: satu baris karakter agent
---

# Nama Agent

Anda adalah **Nama Agent**, [positioning satu kalimat].

## Identitas dan ingatan
- **Peran**: peran spesifik
- **Karakter**: ciri kepribadian
- **Ingatan**: apa yang diingat
- **Pengalaman**: apa yang dikuasai

## Misi utama
...

## Aturan kritis
...

## Deliverable teknis
Contoh kode, template, framework

## Workflow
Langkah-langkah kerja

## Gaya komunikasi
Contoh nada dan kalimat

## Metrik sukses
Kriteria terukur
```

## Garis merah konten

PR yang melanggar di bawah ini akan langsung di-close.

### 1. Tanpa terikat ke employer / brand tertentu

Agent adalah "peran dan metodologi", bukan identitas karyawan. Berikut tidak diterima:

```
Anda adalah Engineer XX dari Group XX — pemimpin global solusi XX...
- Peran: Engineer XX, anggota Group XX
```

Yang benar (netral):

```
Anda adalah Engineer XX, praktisi berpengalaman di bidang XX. Dalam berbagai proyek XX...
- Peran: Engineer XX — metodologi dan eksekusi di XX
```

**Pengecualian**: nama model peralatan, software, atau protokol standar industri (misal "Bullmer S90 PRO", "Adobe Premiere Pro", "PCI DSS") adalah referensi teknis, bukan brand placement; boleh dipertahankan.

### 2. Tanpa menyisipkan API / plugin alat tertentu di body prompt

Prompt agent harus jalan di LLM mana pun, alat mana pun. Menyisipkan nama API, cara panggil, atau link eksternal alat tertentu di body prompt menjadi sampah konten dan berpotensi jadi iklan vendor.

### 3. Tanpa "soft marketing" berkedok terjemahan/penambahan

PR dengan judul "docs: pelengkapan" tapi isinya link eksternal, sebutan produk sendiri, anchor SEO — akan dinilai dari isi, bukan judul.

## Kirim PR

1. Fork repo ini
2. Buat branch: `git checkout -b add-xxx-agent`
3. Tulis kontennya, cek format secara lokal
4. Buka PR dengan deskripsi singkat

## Konvensi

- File pakai line ending LF (bukan CRLF)
- Satu PR satu hal (jangan campur terjemahan dengan penambahan)
- Commit message boleh Bahasa Indonesia atau Inggris
