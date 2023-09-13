# Final Submission : Machine Learning Pipeline - Customer Classification
| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Customer Segmentation Classification dataset](https://www.kaggle.com/datasets/kaushiksuresh147/customer-segmentation) |
| Masalah | Dalam dunia pemasaran diperlukan strategi yang tepat dalam melakukan pendekatan pada custemer. Salah satu strategi yang dapat dilakukan adalah dengan menglasifikasikan customer sehingga pendekatan dapat dilakukan dengan tepat. Kasus ini biasa terjadi pada seorang Digital Marketer untuk menentukan target iklan mereka|
| Solusi machine learning | Model machine learning yang dikembangkan didasari dengan Gender (Jenis Kelamin), Ever_Married (Pernah Menikah), Age (Umur), Graduated(Lulus Kuliah), Profession(Pekerjaan), Work_Experience(Pengalaman Kerja), Spending_Score (Skor Pengeluaran), dan Family_Size (Jumlah Anggota Keluarga)|
| Metode pengolahan | Pada kasus ini, terdapat sembilan feature dimana delapan akan digunakan untuk features klasifikasi, dan satu sebagai class, terdapat dua categorical feature dan enam numerical, kemudian akan dilakukan split data menjadi 80:20 untuk data train dan eval. Proses transform akan dilakukan renaming untuk feature yang telah ditransform, one hot encoding untuk class data |
| Arsitektur model | Arsitektur yang digunakan dalam projek ini terdiri dari beberapa layer. Untuk tiap layer menggunakan Dense 256, Dense 64, Dense 16 dengan activation relu, kemudian layer terakhir menggunakan Dense 1 dengan activation sigmoid untuk menglasifikasi class yang memiliki dua nilai yaitu 1 dan 0. Untuk model compile menggunakan optimizers Adam dengan learning_rate 0.001, loss binary_crossentropy dengan metrics BinaryAccuracy |
| Metrik evaluasi | Metrik evaluasi yang digunakan yaitu AUC, Precision, Recall, ExampleCount dan BinaryAccuracy |
| Performa model | Peformanya sendiri menunjukan nilai yang bagus, dengan nilai akurasi diatas 80%  |
| Opsi deployment | Untuk deployment, sistem ini akan dideploy menggunakan platform railway |
| Web app | [Customer-Classification](https://sub2-production.up.railway.app/v1/models/customer-model:predict)|
| Monitoring | Monitoring pada sistem ini dilakukan menggunakan prometheus |