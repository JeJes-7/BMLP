# BMLP
BMLP (Belajar Machine Learning untuk Pemula)

🚀 Deteksi Penipuan Finansial & Analisis Pola Transaksi (Machine Learning)

Projek ini dikembangkan sebagai bagian dari Belajar Machine Learning untuk Pemula (BMLP). Repository ini berfokus pada eksplorasi perilaku transaksi dan pola aktivitas keuangan untuk mendeteksi penipuan (fraud detection) dan identifikasi anomali menggunakan teknik Unsupervised Learning (Clustering) dan Supervised Learning (Classification).

📊 Tentang Dataset

Dataset yang digunakan berisi 2.512 sampel data transaksi yang mencakup berbagai atribut transaksi, demografi nasabah, dan pola penggunaan. Dataset ini ideal untuk keamanan finansial dan pengembangan model prediktif.

🛠️ Tahapan Projek (Workflow)

Projek ini dikerjakan melalui 5 tahapan utama sesuai kriteria yang ditentukan:

1. Exploratory Data Analysis (EDA)

Menampilkan struktur dataset menggunakan head(), info(), dan ringkasan statistik deskriptif menggunakan describe().

2. Pembersihan & Pra-Pemrosesan Data (Data Preprocessing)
   
- Pengecekan missing values (isnull().sum()) dan data duplikat (duplicated().sum()).
- Penanganan data hilang menggunakan dropna() dan penghapusan duplikat dengan drop_duplicates().
- Penghapusan kolom yang tidak relevan (ID, Address, dan Date).
- Penerapan Feature Encoding menggunakan LabelEncoder() (serta opsi One Hot Encoding untuk tahap lanjutan).

3. Membangun Model Clustering (Unsupervised Learning)
- Menentukan jumlah cluster terbaik menggunakan visualisasi Elbow Method (KElbowVisualizer).
- Melatih model pengelompokan menggunakan algoritma K-Means Clustering.
- Menyimpan model clustering menggunakan joblib.dump().
  
4. Interpretasi Hasil Clustering
- Menganalisis karakteristik tiap cluster berdasarkan nilai mean, min, dan max dari fitur numerik.
- Mengekspor data hasil preprocessing dan clustering dengan menambahkan kolom baru bernama Target sebagai label untuk tahap klasifikasi.
  
5. Membangun Model Klasifikasi (Supervised Learning)
- Membagi dataset menjadi data latih dan data uji menggunakan train_test_split() dengan parameter stratify=y.
- Membangun dan melatih model klasifikasi menggunakan Decision Tree Classifier.
- Melakukan eksperimen lanjutan (Skilled/Advanced) menggunakan Random Forest Classifier dan Hyperparameter Tuning (GridSearchCV).
- Evaluasi performa model menggunakan Accuracy, Precision, Recall, dan F1-Score (classification_report).
- Menyimpan model terbaik menggunakan joblib.dump().


Author
Jesika Yudiani Putri

Peserta Belajar Machine Learning untuk Pemula (BMLP)

Disubmit pada Jumat, 23 Oktober 2026
