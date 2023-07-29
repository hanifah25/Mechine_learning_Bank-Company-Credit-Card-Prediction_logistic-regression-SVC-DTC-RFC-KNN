--- keterangan kolom

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
