# Pelacakan upstream

Catatan versi upstream [agency-agents](https://github.com/msitarzewski/agency-agents) yang menjadi basis proyek ini, untuk mempermudah sinkronisasi update.

## Baseline saat ini

- **Repo upstream**: https://github.com/msitarzewski/agency-agents
- **Commit referensi**: `783f6a7` (2026-04-12)
- **Total agent upstream**: 184 (tidak termasuk 16 dokumen operasional di `strategy/`)

## Cakupan terjemahan

| Kategori | Total upstream | Diterjemahkan | Cakupan |
|----------|--------------:|--------------:|--------:|
| academic | 5 | 5 | 100% |
| design | 8 | 8 | 100% |
| engineering | 29 | 29 | 100% |
| finance | 5 | 5 | 100% |
| game-development | 20 | 20 | 100% |
| marketing | 30 | 30 | 100% |
| paid-media | 7 | 7 | 100% |
| product | 5 | 5 | 100% |
| project-management | 6 | 6 | 100% |
| sales | 8 | 8 | 100% |
| spatial-computing | 6 | 6 | 100% |
| specialized | 41 | 41 | 100% |
| support | 6 | 6 | 100% |
| testing | 8 | 8 | 100% |
| **Total** | **184** | **184** | **100%** |

## Metode terjemahan

Inggris upstream → Bahasa Indonesia (batch via Claude Sonnet). Menjaga tone dan struktur asli dengan ungkapan yang natural bagi pembaca Indonesia.

- Istilah teknis Inggris (TensorFlow / PyTorch / RAG / MLOps / LLM / API / OAuth / REST dll.): tetap Inggris
- Blok kode, path, URL, command: tidak diubah
- Body / heading / tabel / list: diterjemahkan ke Bahasa Indonesia natural
- Frontmatter `name:`, `description:`, `vibe:`: diterjemahkan; `color:`, `emoji:`: dipertahankan

## Agent khusus pasar Indonesia

Selain 184 terjemahan, **PR agent khusus pasar Indonesia welcome**. Area yang masih kosong:

- Platform ID (WhatsApp Business, Instagram ID, TikTok ID)
- E-commerce / Marketplace (Tokopedia, Shopee, Bukalapak, Blibli, Lazada)
- Super App (Gojek/GoTo, Grab Indonesia, Traveloka)
- Fintech (OVO, GoPay, DANA, ShopeePay, QRIS, BI-FAST)
- Compliance (UU PDP, OJK, Kominfo)
- Vertikal (Halal e-commerce, Edutech ID, Pertanian digital)

Detail di [CONTRIBUTING.md](./CONTRIBUTING.md).

## Kebijakan sinkronisasi

- Mengikuti branch `main` upstream
- Agent baru di upstream akan diterjemahkan bertahap
- Perubahan struktural besar (rename direktori dll.) di-mirror dalam 1 minggu
- Versi upstream diperbarui di file ini setiap kali sinkronisasi
