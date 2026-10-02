# Practical Statistics for Data Scientists

Repository ini berisi **reproduksi kode Python** dan **penjelasan teori** dari buku
*Practical Statistics for Data Scientists: 50+ Essential Concepts Using R and Python* (2nd Edition)
karya **Peter Bruce, Andrew Bruce, dan Peter Gedeck** (O'Reilly, 2020).

Dibuat untuk memenuhi **Tugas 1 — Enrichment for Machine Learning Class (Individual Task)**.

| | |
|---|---|
| **Nama** | *Ahmad GHazali EL-Faruqi Hsb* |
| **NIM** | *101032330080* |
| **Mata Kuliah** | Machine Learning |

---

## 📁 Struktur Repository

```
Practical-Statistics-for-Data-Scientists/
├── README.md
├── requirements.txt
├── data/                 # Dataset dari repository resmi penulis buku
└── notebooks/
    ├── Chapter1_Exploratory_Data_Analysis.ipynb
    ├── Chapter2_Data_and_Sampling_Distributions.ipynb
    ├── Chapter3_Statistical_Experiments_and_Significance_Testing.ipynb
    └── Chapter4_Regression_and_Prediction.ipynb
```

Setiap notebook disusun dengan pola: **teori → kode → interpretasi output**, untuk setiap sub-bab, lalu ditutup dengan **ringkasan chapter**.

---

## 📚 Ringkasan Isi Setiap Chapter

### [Chapter 1 — Exploratory Data Analysis](notebooks/Chapter1_Exploratory_Data_Analysis.ipynb)
Membahas langkah pertama dalam setiap proyek data: **mengenal data**. Topiknya meliputi tipe data (numerik dan kategorikal) dan data rectangular, **estimasi lokasi** (mean, trimmed mean, weighted mean, median), **estimasi variabilitas** (variance, standard deviation, MAD, IQR), serta eksplorasi distribusi dengan **persentil, boxplot, frequency table, histogram, dan density plot**. Chapter ini juga membahas ringkasan data kategorikal (mode, bar chart, expected value), **korelasi** dan scatterplot, serta visualisasi dua variabel atau lebih (**hexbin, contour, contingency table, violin plot, conditioning**).
**Dataset:** `state.csv`, `dfw_airline.csv`, `sp500_*.csv`, `kc_tax.csv.gz`, `lc_loans.csv`, `airline_stats.csv`

### [Chapter 2 — Data and Sampling Distributions](notebooks/Chapter2_Data_and_Sampling_Distributions.ipynb)
Membahas hubungan **sampel dan populasi**: random sampling, sample bias, selection bias, dan regression to the mean. Inti chapter ini adalah **sampling distribution** dan **Central Limit Theorem**, **standard error**, serta **bootstrap** dan **confidence interval** untuk mengukur ketidakpastian estimasi tanpa asumsi distribusi. Chapter ini juga mengenalkan distribusi penting: **normal** (dan QQ-plot), **long-tailed**, **t**, **binomial**, **chi-square**, **F**, **Poisson**, **eksponensial**, dan **Weibull**.
**Dataset:** `loans_income.csv`, `sp500_data.csv.gz`

### [Chapter 3 — Statistical Experiments and Significance Testing](notebooks/Chapter3_Statistical_Experiments_and_Significance_Testing.ipynb)
Membahas cara merancang eksperimen (**A/B testing**) dan menentukan apakah perbedaan hasil **nyata atau hanya kebetulan**. Topiknya meliputi **hypothesis testing** (null vs alternative, one-way vs two-way), **permutation test**, **p-value**, alpha, error Type I dan II, **t-test**, **multiple testing**, **degrees of freedom**, **ANOVA** dan **F-statistic**, **chi-square test** dan Fisher's exact test, **multi-arm bandit**, serta **power and sample size**.
**Dataset:** `web_page_data.csv`, `four_sessions.csv`, `click_rates.csv`, `imanishi_data.csv`

### [Chapter 4 — Regression and Prediction](notebooks/Chapter4_Regression_and_Prediction.ipynb)
Membahas **regresi linear** untuk penjelasan dan prediksi: **simple dan multiple linear regression**, least squares, evaluasi model (**RMSE, R², t-stat, p-value**), model selection (**AIC, stepwise regression**), dan **weighted regression**. Topik lainnya meliputi prediction interval vs confidence interval, **dummy variables** untuk variabel kategorikal, interpretasi koefisien (**multicollinearity, confounding, interaction**), **regression diagnostics** (outlier, influential values, heteroskedasticity, partial residual plot), serta model non-linear (**polynomial, spline, GAM**). Sebagai materi tambahan, dibahas juga **Lasso regularization**.
**Dataset:** `LungDisease.csv`, `house_sales.csv`

---

## ⚙️ Cara Menjalankan

```bash
git clone https://github.com/<username>/Practical-Statistics-for-Data-Scientists.git
cd Practical-Statistics-for-Data-Scientists
pip install -r requirements.txt
jupyter notebook
```
Buka notebook di folder `notebooks/`, lalu jalankan **Run All**.

---

## 📖 Referensi
- Bruce, P., Bruce, A., & Gedeck, P. (2020). *Practical Statistics for Data Scientists* (2nd ed.). O'Reilly Media.
- Kode & dataset resmi: https://github.com/gedeck/practical-statistics-for-data-scientists
