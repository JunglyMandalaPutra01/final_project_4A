# EDA
### Berikut ini Insight yang diperoleh pada proses EDA :
1. Rata-rata umur nasabah adalah 38 tahun dan umur nasabah yang paling banyak melakukan Churn berkisar antara 37-50 tahun yang mengartikan bahwa nasabah tergolong kelompok usia dewasa sampai lansia. Sedangkan Nasabah yang stay atau bertahan di Bank tergolong di usia dewasa yang umurnya berkisar antara 30-40 tahun.
2. Nasabah yang tidak memiliki saldo lebih banya melakukan Churn.
3. 50% dari seluruh Nasabah berasal dari negara Prancis dan jumlah nasabah Churn di negara ini lebih tinggi dari beberapa negara yang ada. Namun, berdasarkan jumlah nasabah pernegara, persentase jumlah nasabah Churn di Jerman lebih tinggi dibandingkan negara Prancis dan Spanyol.
4. Tenure tidak terlalu mempengaruhi tingkat keinginan nasabah Churn.
5. Nasabah wanita cenderung lebih banyak melakukan churn dibandingkan dengan nasabah pria.

# Proses data Preprocessing
## A. Data Cleansing 
1. Pada dataset tidak terdapat missing values
2. Pada dataset tidak terdapat duplicated data
3. Pada dataset ada dua feature yang di Handle outliers yaitu feature CreditScore dan Age. Handling ourliers menggunakan Z-Score
4. Pada saat melakukan feature transformation dilakukan menggunakan MinMaxScaler dengan mentransformasikan feature-feature yang memiliki data numerik
5. Terdapat dua Feature yang dilakukan encod yaitu feature Gender dan Geography. Metode yang digunakan adalah label endcoding untuk feature Gender dan One-hot-encoding untuk feature Geography
5. Pada proses Handle class imbalance menggunakan oversampling SMOTE
## B. Feature Engineering
1. Feature yang di seleksi adalah RowNumber, CustomerId, Surname dan Geography
2. Feature yang ditambah ada tiga yaitu Balance-to-SallaryRatio, Tenure-to-AgeRatio dan Age-to-CreditRatio
3. Feature yang bisa menjadi pendukung dalam pemodelan meskipun tidak ada dalam dataset adalah feature Partner, total tanggungan, Profesi dan masa aktif nasabah