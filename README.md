## Mechine_learning_Bank-Company-Credit-Card-Prediction_logistic-regression-SVC-DTC-RFC-KNN

## Problem Statement
model Classification untuk memprediksi default_payment_next_month dalam Prediksi pembayaran tertunda kartu kredit.

## Objective
Prediksi pembayaran tertunda: Berdasarkan riwayat pembayaran kartu kredit sebelumnya, dapat diprediksi apakah seseorang akan membayar tagihan kartu kredit mereka pada waktu yang tepat atau akan terlambat. Jika seseorang cenderung terlambat membayar tagihan, bank penerbit kartu kredit dapat mengambil tindakan preventif, seperti mengirimkan pemberitahuan, menyesuaikan batas kredit atau jika memang tidak membayar berkelanjutan akan disuspend.

## Result 
best model: nb
cross-val mean: 0.34072995534847605
Cross validation Metrik yang digunakan untuk evaluasi adalah recall, dan skema cross-validation yang digunakan adalah Stratified K-Fold. Pada setiap iterasi, code akan menghitung nilai recall pada data train yang dipartisi menggunakan skema Stratified K-Fold. Setelah selesai melakukan cross validation pada masing-masing model, code akan menampilkan nilai recall rata-rata dan standar deviasi pada setiap fold, serta menampilkan rentang nilai recall yang dihasilkan pada setiap model.juga membandingkan nilai recall rata-rata dari semua model dan memilih model yang memiliki nilai recall rata-rata tertinggi sebagai model terbaik. dari data di atas dapat kita lihat best model dari hasil prediksi adalah nb dengan nilai cross-val mean: 0.34. namun dalam hal ini NB cenderung tidak efektif pada dataset yang tidak seimbang, di mana jumlah sampel pada setiap kelas tidak seimbang dan Model GaussianNB tidak memiliki hyperparameter yang signifikan yang dapat diatur secara manual, maka dari itu untuk dalam pemodelan prediksi lebih lanjut akan di gunakan model SCV yang lebih cocok untuk data set ini.

## keterangan kolom

* LIMIT_BAL: Jumlah kredit yang diberikan, termasuk kredit individu dan tambahan.
* SEX: Jenis kelamin pelanggan (1 = pria, 2 = wanita)
* EDUCATION: (1 = graduate school; 2 = university; 3 = high school; 4 = others)
* MARRIAGE: (1 = married; 2 = single; 3 = others)
* AGE: Usia pelanggan
* PAY_0: Riwayat status pelunasan sebelumnya, apakah dibayar tepat waktu atau keterlambatan pembayaran. PAY_0 = status pembayaran di bulan September. Skala (berlaku untuk PAY_0 hingga Pay_6): -1 = bayar dengan semestinya, 1 = penundaan pembayaran selama * 1 bulan, 2 = penundaan pembayaran selama 2 bulan, ... 9 = penundaan pembayaran selama 9 bulan atau lebih)
* -2 : Saldo telah dibayar dan belum ada transaksi untuk bulan tersebut, yaitu. tidak ada kredit yang harus dibayar
* -1 : Saldo telah dibayar penuh tetapi ada beberapa transaksi selama bulan tersebut yang tidak tercermin pada laporan tagihan saat ini
* 0 : Pelanggan telah membayar minimal jumlah minimum yang dipersyaratkan, namun masih ada sisa saldo yang harus dibayar
* 1-9 Ketika seorang pelanggan tidak membayar jumlah minimum yang disyaratkan, itu dianggap sebagai pembayaran yang terlewatkan untuk bulan itu. Angka 1-9 akan sesuai dengan bulan kumulatif dari pembayaran yang terlewatkan pada saat itu.
* PAY_2: repayment status in August
* PAY_3: repayment status in July
* PAY_4: repayment status in June
* PAY_5: repayment status in May
* PAY_6: repayment status in April
* BILL_AMT1: Jumlah tagihan September
* BILL_AMT2: Jumlah tagihan August
* BILL_AMT3: Jumlah tagihan July
* BILL_AMT4: Jumlah tagihan June
* BILL_AMT5: Jumlah tagihan May
* BILL_AMT6: Jumlah tagihan April
* PAY_AMT1: Jumlah yang dibayarkan September
* PAY_AMT2: Jumlah yang dibayarkan August
* PAY_AMT3: Jumlah yang dibayarkan July
* PAY_AMT4: Jumlah yang dibayarkan June
* PAY_AMT5: Jumlah yang dibayarkan May
* PAY_AMT6: Jumlah yang dibayarkan April
* default_payment_next_month: apakah klien gagal membayar (0 = No, 1 = Yes)
