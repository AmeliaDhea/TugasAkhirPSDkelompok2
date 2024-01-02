# Penjelasan Tugas Akhir Kelompok 2 
## Mengelompokkan Class siswa berdasarkan nilai akhir siswa

### Capstone 1
#### Memilih dataset bidang edukasi
https://github.com/Western-OC2-Lab/Student-Performance-and-Engagement-Prediction-eLearning-datasets

### Capstone 2
#### Identifikasi Masalah & Pendekatan Analitik Identifikasi Masalah
A. Identifikasi Masalah
1. Menetapkan permasalahan yang akan diselesaikan
   Permasalahan yang akan diselesaikan adalah mengelompokkan class siswa berdasarkan nilai akhir siswa.
2. Menentukan tujuan sains data yang akan diselesaikan
   Tujuan sains data adalah menciptakan model klasifikasi yang dapat mengelompokkan Class siswa berdasarkan kumpulan nilai akhir siswa. Model-model ini akan memberikan pemahaman mendalam terhadap faktor-faktor yang menentukan Class siswa.
B. Pendekatan Analitik
1. Informasikan dan deskripsikan metode analitik apa yang akan diselesaikan dengan menggunakan dataset tersebut
   Pendekatan analitik akan melibatkan penggunaan metode pembelajaran mesin untuk mengembangkan model klasifikasi. Model yang dikembangkan menggunakan teknik klasifikasi ansambel untuk mengkategorikan siswa dan memprediksi kinerja akhir kelompok/kategori selama kursus dalam dua tahap — pada 20% dan 50% tugas kursus.
### Capstone 3
#### Data Requirements & Data Collections
A. Data Requirements
1. Fitur-fitur apa saja yang diperlukan untuk  menyelesaikan kasus sains data
a. Quiz01 	: Nilai dari Quiz 1.
b. Assign.01	: Nilai dari Tugas 1.
c. Midterm	: Nilai dari Ujian Tengah Semester.
d. Assign.02	: Nilai dari Tugas 2.
e. Assign.03	: Nilai dari Tugas 3.
f. Final Exam	: Nilai dari Ujian Akhir.
g. Final Grade	: Total nilai akhir mahasiswa.
h. Student Category: Kategori akhir dari kinerja mahasiswa. Fitur ini bersifat nominal dan memiliki nilai kategorikal, yaitu "G" (Good), "F" (Fair), atau "W" (Weak).  (sebagai variabel y)
2. Tidak semua fitur akan sesuai dengan kasus yang akan diselesaikan sesuai pada poin 1
a. Student Id : Nomor identitas tidak dibutuhkan untuk klasifikasi data
3. Berikan argumen pada data maupun fitur yang akan digunakan : 
a. Quiz01: Nilai dari Quiz 1 bisa menjadi indikator awal kinerja mahasiswa. Ini dapat memberikan wawasan awal tentang pemahaman materi oleh mahasiswa.
b. Assign.01, Assign.02, Assign.03: Nilai dari tugas-tugas dapat memberikan informasi tentang kemampuan mahasiswa dalam mengerjakan pekerjaan rumah dan proyek-proyek yang diberikan.
c. Midterm: Nilai dari Ujian Tengah Semester adalah indikator penting tentang pemahaman dan penguasaan materi setelah pertengahan periode kuliah.
d. Final Exam: Nilai dari Ujian Akhir adalah salah satu komponen paling penting untuk menentukan hasil akhir mahasiswa.
e. Final Grade : Nilai akhir mahasiswa dapat dijadikan target variabel untuk model prediksi. Ini adalah hasil akhir yang ingin diprediksi.
f. Student Category (sebagai variabel y): Kategori akhir kinerja mahasiswa ("G" (Good), "F" (Fair), atau "W" (Weak)) adalah variabel target kategori yang ingin diprediksi.
### Capstone 4
A. Data Understanding
**Dataset "Student Performance Prediction-Multi.csv" berisi data-data prediksi kinerja mahasiswa dalam bentuk multi-kelas. Berikut adalah deskripsi dari kolom-kolom yang ada dalam dataset tersebut:**
- "Student ID": ID unik yang mengidentifikasi setiap mahasiswa.
- "Quiz01 [10]": Skor yang diperoleh mahasiswa dalam kuis 1, dengan total skor maksimum 10.
- "Assignment01 [8]": Skor yang diperoleh mahasiswa dalam tugas 1, dengan total skor maksimum 8.
- "Midterm Exam [20]": Skor yang diperoleh mahasiswa dalam ujian paruh semester, dengan total skor maksimum 20.
- "Assignment02 [12]": Skor yang diperoleh mahasiswa dalam tugas 2, dengan total skor maksimum 12.
- "Assignment03 [25]": Skor yang diperoleh mahasiswa dalam tugas 3, dengan total skor maksimum 25.
- "Final Exam [35]": Skor yang diperoleh mahasiswa dalam ujian akhir, dengan total skor maksimum 35.
- "Course Grade": Kelas hasil prediksi kinerja mahasiswa dalam mata kuliah ini. Nilai ini merupakan prediksi yang didasarkan pada skor-skor yang diperoleh mahasiswa.
- "Total [100]": Total skor yang diperoleh mahasiswa dari semua komponen evaluasi dalam mata kuliah ini, dengan total skor maksimum 100.
- "Class": Kelas aktual dari mahasiswa, yaitu kelas yang seharusnya didapatkan berdasarkan kriteria penilaian.
**Buat data dictionary nya yang berisi penjelasan setiap fitur data yang digunakan secara lengkap**
- "Quiz01 [10]":
   - Deskripsi: Skor yang diperoleh mahasiswa dalam kuis 1.
   - Tipe data: Numerik (float)
   - Rentang nilai: 0 hingga 10
- "Assignment01 [8]":
   - Deskripsi: Skor yang diperoleh mahasiswa dalam tugas 1.
   - Tipe data: Numerik (float)
   - Rentang nilai: 0 hingga 8
- "Midterm Exam [20]":
   - Deskripsi: Skor yang diperoleh mahasiswa dalam ujian paruh semester.
   - Tipe data: Numerik (float)
   - Rentang nilai: 0 hingga 20
- "Assignment02 [12]":
   - Deskripsi: Skor yang diperoleh mahasiswa dalam tugas 2.
   - Tipe data: Numerik (float)
   - Rentang nilai: 0 hingga 12
- "Assignment03 [25]":
   - Deskripsi: Skor yang diperoleh mahasiswa dalam tugas 3.
   - Tipe data: Numerik (float)
   - Rentang nilai: 0 hingga 25
- "Final Exam [35]":
   - Deskripsi: Skor yang diperoleh mahasiswa dalam ujian akhir.
   - Tipe data: Numerik (float)
   - Rentang nilai: 0 hingga 35
- "Course Grade":
   - Deskripsi: Kelas hasil prediksi kinerja mahasiswa dalam mata kuliah ini.
   - Tipe data: String
   - Kelas yang mungkin: "G" (Good) atau "F" (Fail), atau “W” (Weak)
- "Total [100]":
   - Deskripsi: Total skor yang diperoleh mahasiswa dari semua komponen evaluasi dalam mata kuliah ini.
   - Tipe data: Numerik (float)
   - Rentang nilai: 0 hingga 100
- "Class":
    - Deskripsi: Kelas aktual dari mahasiswa, yaitu kelas yang seharusnya didapatkan berdasarkan kriteria penilaian.
   - Tipe data: String 
    - Kelas yang mungkin: "G" (Good) atau "F" (Fail), atau “W” (Weak)
**Exploratory Data Analysis (EDA)**
```
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```
Penjelasan : import pandas as pd untuk import library Pandas, yang merupakan library untuk manipulasi dan analisis data.
import matplotlib.pyplot as plt untuk import library Matplotlib, yang merupakan library untuk visualisasi data.
import seaborn as sns untuk import library Seaborn, yang merupakan library untuk visualisasi data yang lebih kompleks.
```
dataset = pd.read_excel('grade.xlsx')
dataset.head()
```
Penjelasan : Untuk membaca data dan menampilkan data 5 baris yang paling atas
```
dataset.columns
```
Penjelasan : Menampilkan kolom yang ada pada data
```
dataset.info()
```
Penjelasan : Digunakan untuk menampilkan ringkasan informasi tentang struktur dan data dari DataFrame dataset. Informasi yang ditampilkan meliputi jumlah kolom, nama kolom, tipe data, jumlah nilai non-null. dan penggunaan memori.
```
print(dataset.describe())
```
Penjelasan : Digunakan untuk menampilkan ringkasan statistik deskriptif untuk setiap kolom numerik dalam DataFrame dataset. Ringkasan meliputi jumlah, mean, median, modus, standar deviasi, min, dan max.
```
dataset.Class.value_counts("G, F, W")
```
Penjelasan : Kode ini menghitung berapa kali setiap nilai "G", "F", dan "W" muncul dalam kolom "Class" pada DataFrame dataset.
**Insight-insight yang didapatkan dalam proses EDA**
86% siswa mendapatkan label class G. 
12% siswa mendapatkan label class F. 
0,2% siswa mendapatkan label class W. 
Rata-rata nilai kuis satu 78 dengan std 14. 
Rata-rata nilai Assignment (01) 75 dengan std 18. 
Rata-rata nilai Midterm exam 77 dengan std 12.
Rata -rata nilai Assignment (02) 77 dengan std 15. 
Rata -rata nilai Assignment (03) 81 dengan std 13. 
Rata-rata final exam 62 dengan std 13. 
Rata-rata Course Grade 80 dengan std 11. 
Rata-rata total 80 dengan std 11. 

B. Data Preparation
```
dataset.dropna(inplace=True)
```
Penjelasan : Menghapus nilai dari baris yang kosong
```
dataset.empty
```
Penjelasan : Mengecek apakah ada data yang kosong
```
en = LabelEncoder()

dataset['Class'] = en.fit_transform(dataset['Class'])
dataset.head()
```
Penjelasan : Menggunakan LabelEncoder untuk mengubah data kategorikal menjadi numerik
```
x = dataset.iloc[:, :-1].values
y = dataset.iloc[:, -1].values
```
Penjelasan : Memisahkan fitur dan target

### Capstone 5
#### Modeling & Evaluasi
A. Data Modeling
```
x_train, x_test, y_train, y_test = train_test_split(x, y, test_size=0.2, random_state=123)
```
Penjelasan : Membagi data latih dan data uji
```
sc = StandardScaler()
x_train = sc.fit_transform(x_train)
x_test = sc.transform(x_test)
```
Penjelasan : Melakukan standarisasi fitur
```
classifier = GaussianNB()
classifier.fit(x_train,y_train)
```
Penjelasan : Pembuatan dan pelatihan model klasifikasi menggunakan algoritma Naive Bayes dengan distribusi Gaussian. Berikut detail angkah-langkahnya:
**classifier = GaussianNB():** Baris ini membuat objek klasifikasi menggunakan kelas GaussianNB dari pustaka scikit-learn. GaussianNB merujuk pada algoritma klasifikasi Naive Bayes dengan asumsi bahwa fitur-fiturnya memiliki distribusi Gaussian (normal).
**classifier.fit(x_train, y_train):** Baris ini melakukan pelatihan model menggunakan metode fit. Metode ini mengambil dua parameter:
**x_train:** Matriks fitur latihan yang berisi nilai-nilai fitur dari data pelatihan.
**y_train:** Larik target yang berisi label untuk data pelatihan.
Selama pelatihan, model belajar dari data latihan untuk memahami hubungan antara fitur dan label. Model ini menggunakan algoritma Naive Bayes untuk memprediksi label baru berdasarkan distribusi Gaussian fitur-fitur pada data latihan.
```
y_pred = classifier.predict(x_test)
```
Penjelasan : x_test adalah matriks fitur untuk data uji yang ingin Anda prediksi, dan y_pred akan berisi prediksi yang dihasilkan oleh model.
```
classifier.predict_proba(x_test)
```
Penjelasan : mengembalikan probabilitas prediksi kelas untuk setiap sampel dalam data uji berdasarkan model klasifikasi yang telah dilatih.
B. Evaluasi Data
```
cm = confusion_matrix(y_test, y_pred)
print(cm)
```
Penjelasan : Menghasilkan matriks kebingungan (confusion matrix) yang menunjukkan jumlah prediksi benar dan salah untuk setiap kelas pada data uji, dan print(cm) menampilkan matriks kebingungan tersebut ke konsol.
```
plt.scatter(range(len(y_test)), y_test, label='Aktual', marker='o')
plt.scatter(range(len(y_pred)), y_pred, label='Prediksi', marker='x')
plt.xlabel('Data Uji')
plt.ylabel('Kelas')
plt.title('Scatter Plot: Data Aktual vs. Data Prediksi')
plt.legend()
plt.show()
```
Penjelasan : Visualisasi data untuk menampilkan perbandingan data aktual dan data prediksi dalam bentuk scatter plot
```
akurasi = classification_report(y_test, y_pred)
print(akurasi)
```
Penjelasan : menghasilkan laporan klasifikasi yang mencakup metrik evaluasi seperti presisi, recall, f1-score, dan dukungan untuk setiap kelas pada data uji, dan print(akurasi) menampilkan laporan klasifikasi tersebut ke konsol.
```
print("Tingkat Akurasi: {:.2%}".format(akurasi))
```
Penjelasan : Untuk menampilkan presentasi akurasi dengan 2 digit di belakang koma
```
ydata = pd.DataFrame()
ydata['y_test'] = pd.DataFrame(y_test)
ydata['y_pred'] = pd.DataFrame(y_pred)
ydata
```
Penjelasan : ydata adalah DataFrame yang dibuat untuk membandingkan label sebenarnya (y_test) dengan label yang diprediksi (y_pred), dan ditampilkan sebagai tabel untuk memudahkan analisis.
