# GuardAMDAI
AI-Driven Predictive Acid Mine Drainage Management System for Kideco Innovation Hackathon (KIC) 2026.

# GuardAMD AI — Predictive Acid Mine Drainage Management

[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue.svg)](https://www.python.org)
[![Streamlit App](https://img.shields.io/badge/Framework-Streamlit-FF4B4B.svg)](https://streamlit.io)
[![Framework](https://img.shields.io/badge/ML-Scikit--Learn-F7931E.svg)](https://scikit-learn.org/)

**GuardAMD AI** adalah prototipe sistem cerdas berbasis *Machine Learning* yang dirancang untuk mengantisipasi dan memitigasi fenomena **Air Asam Tambang (Acid Mine Drainage / AMD)** secara preventif. Proyek ini dikembangkan sebagai bagian dari inovasi untuk **Kideco Innovation Hackathon (KIC) 2026** dengan pilar *AI-Driven Operational Excellence*.

---

## 📌 Fitur Utama

1. **Predictive Analytics (24-Hour pH Forecasting):** Memprediksi tingkat keasaman air (pH) untuk 24 jam ke depan menggunakan algoritma *Random Forest Regression* berdasarkan parameter multi-dimensi.
2. **Automated Risk Scoring:** Mengklasifikasikan tingkat risiko lingkungan ke dalam kategori **LOW**, **MEDIUM**, atau **HIGH** secara *real-time* berbasis regulasi ambang batas.
3. **Smart Lime Recommendation Engine:** Memberikan estimasi dosis kalkulasi kebutuhan Kalsium Oksida ($CaO$ / Kapur Tohor) yang presisi untuk menetralkan pH air kembali ke batas aman.
4. **Interactive Dashboard:** Antarmuka berbasis Streamlit yang intuitif untuk visualisasi *monitoring* bagi tim operasional di lapangan.

---

## ⚙️ Struktur Parameter & Alur Sistem

### Input Fitur (Data Sensor/Lapangan)
* **pH**: Tingkat keasaman air saat ini.
* **TSS (Total Suspended Solids)**: Kandungan padatan tersuspensi (mg/L).
* **Debit**: Laju aliran air masuk ($m^3$/jam).
* **Fe (Zat Besi) & Mn (Mangan)**: Konsentrasi kandungan logam berat (mg/L).
* **Curah Hujan**: Tingkat presipitasi (mm).

### Alur Kerja Protototipe

git clone [https://github.com/reakkszz/GuardAMDAI.git](https://github.com/reakkszz/GuardAMDAI.git)
cd GuardAMDAI

pip install pandas numpy scikit-learn joblib streamlit

python train_model.py

streamlit run app.py
