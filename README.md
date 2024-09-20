Project ini adalah lanjutan dari project mata kuliah Machine Learning yang dapat dilihat pada link berikut : https://github.com/Zweych/Weather-Data-Analysis-Clustering-as-Prediction-Tools.git

Di project sebelumnya, proses berhenti pada proses clustering dimana diperoleh n_cluster optimal yaitu 4 lalu membuat tabel "Spectral_Cluster" untuk menyimpan hasil cluster dari 1-4 dan menyimpan file hasil clustering ke file "hasil_clustering.ipynb".

Pada project ini, saya melakukan analisa untuk menentukan kemungkinan cuaca di masing-masing cluster dengan mempertimbangkan niai-nilai seperti suhu (Tn, Tx, Tavg), kelembapan (RH_avg), curah hujan (RR), dan lama penyinaran matahari (ss) yang ada di dalam dataset. Dari hasil analisa, didapat kesimpulan sebagai berikut:
1. Cluster 1: Cerah
2. Cluster 2: Berawan
3. Cluster 3: Gerimis
4. Cluster 4: Hujan/Badai

Detail analisa dapat dilihat di dalam file "data_labeling.ipynb". Setelah proses penamaan pada setiap cluster selesai, saya membuat tabel baru untuk menyimpan nama cuaca bernama "Cuaca". Setelah itu, file yang sudah diproses sebelumnya saya simpan ke file baru bernama "new_dataset.csv".

File "new_dataset.csv" saya gunakan untuk task classification dimana saya akan menggunakan 4 model yaitu:
- K-Nearest Neighbor Classifier, akurasi: 93%
- Support Vector Classifier, akurasi: 98%
- Gaussian Naive Bayes, akurasi: 93%
- Random Forest Classifier, akurasi: 94%

Detail dapat dilihat dalam file "weather_classification.ipynb".
