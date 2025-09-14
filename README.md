# Predictive Analysis of World Bank Program Budgets with AI Assistance

## Project Overview

Proyek ini merupakan *capstone project* yang bertujuan untuk menganalisis dataset publik "World Bank Program Budget and All Funds". Tujuan utamanya adalah untuk menggali wawasan mengenai pola alokasi dana, membangun model machine learning untuk memprediksi jumlah anggaran, dan memanfaatkan AI Generatif (IBM Granite) untuk mempercepat analisis serta menghasilkan rekomendasi strategis.

Permasalahan yang diangkat adalah bagaimana manajemen strategis dapat memahami faktor-faktor utama di balik distribusi dana dan menggunakan data historis untuk membuat keputusan yang lebih baik di masa depan.

---

## Raw Dataset Link 

Dataset yang digunakan dalam analisis ini bersifat publik dan dapat diakses melalui portal data resmi Bank Dunia.

* **Nama Dataset:** World Bank Program Budget and All Funds
* **Sumber:** [World Bank Program Budget and All Funds](https://financesone.worldbank.org/world-bank-program-budget-and-all-funds/DS00032)
* **Format:** CSV

---

## Insight & Findings

Analisis data dan pemodelan machine learning menghasilkan beberapa temuan kunci:

1.  **Konsentrasi Dana pada *Client Engagement***
    * Ditemukan bahwa alokasi dana tidak merata, dengan konsentrasi yang signifikan pada grup program kerja **'Client Engagement'**, yang secara konsisten menerima porsi pendanaan terbesar. Hal ini mengindikasikan adanya area prioritas utama dalam pendanaan Bank Dunia.

2.  **Prediktabilitas Anggaran yang Sangat Tinggi**
    * Model regresi **Random Forest** yang dikembangkan berhasil memprediksi jumlah alokasi dana (`All_Funds_Millions`) dengan tingkat keandalan yang sangat tinggi, dibuktikan dengan skor **R-squared sebesar 0.97**. Ini berarti sekitar **97%** variasi dalam alokasi dana dapat dijelaskan oleh fitur-fitur yang ada di dalam model.

3.  **Unit dengan Dana Teratas**
    * Analisis lebih lanjut menunjukkan bahwa unit kerja seperti **'Africa'** dan **'East Asia & Pacific'** merupakan beberapa di antara penerima alokasi dana terbesar, yang memperkuat fokus pada area-area geografis tertentu.

---

## AI Support Explanation

Dalam proyek ini, model AI Generatif **IBM Granite** (`ibm-granite/granite-3.3-8b-instruct`) digunakan melalui platform Replicate untuk mendukung tiga aspek analisis krusial, sesuai dengan pedoman proyek:

1.  **Automated Summarization**
    * **Bagaimana** AI diberi *prompt* yang berisi nama-nama kolom dari dataset.
    * **mengapa?** karena untuk mendapatkan ringkasan eksekutif tentang tujuan utama dataset dan potensi wawasan yang bisa digali. Hal ini mempercepat pemahaman awal tanpa perlu analisis manual yang mendalam.

2.  **Insight Generation**
    * **Bagaimana** AI diberi *prompt* yang menjelaskan temuan dari grafik visualisasi, yaitu bahwa grup 'Client Engagement' menerima dana tertinggi.
    * **Mengapa?** karena untuk membantu menerjemahkan data visual menjadi wawasan bisnis. AI bertindak sebagai "analis strategis" untuk memberikan tiga kemungkinan alasan di balik konsentrasi pendanaan tersebut beserta satu potensi risikonya.

3.  **Recommendation Generation**
    * **Bagaimana** AI diberi *prompt* yang merangkum semua temuan utama dari analisis (skor model yang tinggi dan konsentrasi dana pada 'Client Engagement').
    * **Mengapa?** karena Ini adalah langkah akhir untuk memenuhi output proyek. AI diminta untuk bertindak sebagai "konsultan" dan menghasilkan tiga rekomendasi yang konkret dan bisa ditindaklanjuti (*actionable*) untuk tim manajemen strategis Bank Dunia.
      
---

## Google Colab
 **link:** [Capstone Project IBM SKillsBuild](https://colab.research.google.com/drive/1UeUdKurtd0LP-TEeHiISS86n23DIaAGM?usp=sharing)

