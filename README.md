# 🌦️ AtmosPredict: Hourly Weather Forecasting with XGBoost

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![XGBoost](https://img.shields.io/badge/ML-XGBoost-orange.svg)

## 📌 Deskripsi Proyek
Membangun model Machine Learning untuk memprediksi suhu udara per jam menggunakan **Time Series Analysis**. Model menggunakan **XGBoost Regressor** untuk menangkap pola musiman harian dan tren tahunan.

## 📂 Struktur File
- `data/weatherproject.csv` : Dataset mentah.
- `images/` : Hasil visualisasi & evaluasi.
- `notebooks/Weather_Forecasting.ipynb` : Kode lengkap.

## 📊 Exploratory Data Analysis (EDA)
Menemukan pola siklus 24 jam dan fluktuasi musiman yang stabil sepanjang tahun.

| Tren Suhu | Rata-rata Harian |
| :---: | :---: |
| ![Tren](images/grafik%20suhu%20perjam.png) | ![Daily](images/rata%20rata%20suhu%20harian.png) |

| Distribusi Jam | Heatmap Korelasi |
| :---: | :---: |
| ![Boxplot](images/distribusi%20suhu.png) | ![Heatmap](images/korelasi%20antar%20cuaca.png) |

---

## 🤖 Hasil Pemodelan
Model dilatih dengan fitur *Lag* dan *Rolling Window* untuk akurasi maksimal.

- **MAE:** `0.78 °C`
- **RMSE:** `1.00 °C`

### Evaluasi Akurasi
| Perbandingan Tren | Scatter Plot |
| :---: | :---: |
| ![Akurasi](images/perbandingan%20suhu.png) | ![Scatter](images/analisis%20akurasi.png) |

---

## 🔮 Forecasting & Importance
Model memprediksi 24 jam ke depan dan sangat bergantung pada suhu jam sebelumnya (**Lag_1h**).

| Future Forecast (24h) | Feature Importance |
| :---: | :---: |
| ![Forecast](images/forecasting%20suhu%2024jam.png) | ![Importance](images/feature%20importance.png) |

## 🚀 Cara Jalankan
1. `pip install pandas numpy matplotlib seaborn xgboost scikit-learn statsmodels`
2. Jalankan file di folder `notebooks/`.

---
