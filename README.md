# 📊 Analisis Kepuasan Pelanggan & Waktu Pengiriman  
### Business Intelligence Project

Proyek ini bertujuan untuk melakukan analisis mendalam terhadap **kepuasan pelanggan** berdasarkan **ketepatan waktu pengiriman** pada platform e-commerce. Studi kasus menggunakan dataset *Brazilian E-Commerce* dari Kaggle.

🎯 **Goal Utama:**
- Mengidentifikasi faktor yang mempengaruhi kepuasan pelanggan yaitu skor review
- Melihat pengaruh *delivery performance* terhadap tingkat kepuasan
- Memberikan insight untuk rekomendasi strategi peningkatan layanan

---

## 🔍 Latar Belakang
Dalam dunia e-commerce, kepuasan pelanggan menjadi indikator penting keberhasilan bisnis.  
Salah satu faktor utama yang memengaruhinya adalah **pengiriman produk**.

Jika pesanan datang terlambat → pelanggan cenderung memberikan rating rendah  
Jika pesanan cepat → loyalitas pelanggan meningkat

Oleh karena itu, **Business Intelligence** hadir untuk:
- Mengolah data operasional
- Menyajikan visualisasi kinerja logistik
- Memfasilitasi pengambilan keputusan berbasis data

---

## 🛠️ Tools & Teknologi
| Kategori | Teknologi |
|---------|-----------|
| ETL | Pentaho Data Integration (Kettle) |
| Data Warehouse | MySQL / PostgreSQL |
| Data Cleaning | Pentaho + Excel/CSV |
| Visualization | Metabase / Tableau / Power BI |
| Documentation | GitHub + Markdown |

---

## 🗂️ Sumber Data  
Menggunakan 4 tabel utama dari dataset Kaggle:
| Tabel | Deskripsi |
|-------|-----------|
| `orders.csv` | Informasi pemesanan & tanggal pengiriman |
| `order_items.csv` | Detail produk dalam transaksi |
| `products.csv` | Kategori & informasi barang |
| `customers.csv` | Data pelanggan |

📌 Dataset asli: *Brazilian E-Commerce Public Dataset*

---

## ⚙️ Alur Business Intelligence

```mermaid
flowchart LR
A[CSV Source Files] --> B[Extract - Pentaho]
B --> C[Transform - Cleaning & Join]
C --> D[Load to DWH - Dim & Fact Tables]
D --> E[Dashboard Visualization]
