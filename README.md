# E-commerce-Customer-Churn
Purwadhika Capstone project

#### **Outline**
- Business Problem
- Data Understanding
- Data Cleaning
- Data Analysis
- Data Preprocessing and Feature Engineering
- Modeling
- Conclusion and Recommendation

**Latar Belakang**  
  
Pada era modern ini, retensi pelanggan merupakan faktor penting dalam kelangsungan bisnis untuk bersaing dengan kompetitor. Sebuah riset mengatakan peningkatan retensi pelanggan 5% saja dapat meningkatkan 25% laba [(Fred Reichheld)](https://media.bain.com/Images/BB_Prescription_cutting_costs.pdf), dan pelanggan loyal menghabiskan 67% lebih pada bulan 31-36 dibanding bulan 0-6 [(Fred Reichheld)](https://media.bain.com/Images/Value_online_customer_loyalty_you_capture.pdf). Selain itu, untuk memperoleh pelanggan baru dapat menghabiskan biaya lima kali lebih banyak daripada mempertahankan pelanggan yang sudah ada [(Amy Gallo, 2014)](https://hbr.org/2014/10/the-value-of-keeping-the-right-customers).     

Hal diatas menegaskan bahwa setiap bisnis perlu memelihara hubungan dengan pelanggan loyal, tidak terkecuali pada perusahan E-commerce. Sebuah perusahaan E-commerce ingin melakukan evaluasi pelanggan yang meninggalkan layanan dalam waktu tertentu atau biasa disebut dengan *customer churn*. Apabila pelanggan loyal berpaling, dapat merugikan karena biaya yang dikeluarkan perusahaan bisa 16 kali lebih banyak untuk membawa pelanggan baru ke tingkat yang sama dengan pelanggan loyal. Dengan mengetahui pelanggan mana yang akan berpaling, perusahaan dapat menyesuaikan strategi marketing dan memberikan perlakuan khusus terhadap kelompok pelanggan tersebut.

**Pernyataan Masalah**  
  
Pelanggan loyal yang *churn* dapat merugikan perusahaan apabila tidak dihiraukan, untuk itu perusahaan perlu mempertahankan aktivitas pelanggan loyal di platform E-commerce. Salah satu cara yang dapat dilakukan adalah memberikan promosi. Namun, biaya dan sumber daya yang dikeluarkan menjadi kurang efektif apabila promosi dilakukan tanpa strategi. 

**Tujuan**  
  
Berdasarkan permasalahan diatas, perusahaan dapat melakukan tindakan preventif yaitu dengan prediksi *customer churn*. Dengan mengetahui pelanggan yang berpotensi untuk *churn*, strategi pemasaran yang diberikan lebih tepat sasaran. Hal ini dapat menurunkan biaya marketing dan diharapkan dapat meningkatkan profit dengan mempertahankan pelanggan loyal.

Selain itu, dengan mengetahui faktor apa saja yang mempengaruhi pelanggan *churn* dapat menjadi pendukung pengambilan keputusan strategi pemasaran.

**Pendekatan Analitik**  
  
Pendekatan analitik yang dilakukan berupa pembuatan, evaluasi, dan implementasi model machine learning klasifikasi yang dapat memprediksi apabila pelanggan akan *churn* atau tidak berdasarkan riwayat data sebelumnya. 

**Metrik Evaluasi**



|       | N-Pred| P-Pred |
| --- | --- | --- |
| **N-Act**     | TP | FP |
| **P-Act**      | FN | TP |

Target:   
0 : Pelanggan tidak *churn*  
1 : Pelanggan *churn*

Type 1 error : False Positive  
Konsekuensi: Mengeluarkan biaya untuk pelanggan yang kurang tepat atau pelanggan yang tidak akan churn. 

Type 2 error : False Negative  
Konsekuensi: Hilangnya pelanggan loyal

Berdasarkan konsekuensinya, langkah yang tepat untuk pemilihan model adalah model yang mengurangi hilangnya pelanggan loyal, tetapi tetap memperhatikan pengeluaran biaya pemasaran untuk pelanggan yang kurang tepat. Recall dan precision yang diseimbangkan akan dari kelas positif (Pelanggan *churn*). Metrik yang akan digunakan adalah ROC-AUC. 
