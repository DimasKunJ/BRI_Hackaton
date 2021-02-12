# People Analytics

## Brief

Binary Classification menggunakan AUC sebagai metricsnya.

## To Do

1. Nyoba menggunakan model lain (Boosting klo bisa kyk Catboost, LGBM, dst)
2. Nyobain macem" Imbalance Learning
3. Feature Selection(?)
4. Cari metode yang optimal buat nanganin `GPA`
5. Ensemble Learning (?)

## Log

Model - model yang udah di coba dan scorenya bisa di liat [di sini ](https://docs.google.com/spreadsheets/d/1dmZuqc1NWMqfaD5kJaXSihSpY6FnKLt5WguQh2YXDrk/edit?usp=sharing)

## Hal yang udah dilakuin

1. Preprocess
   1. Imputation (Missing data)<br>
   Missing datanya cuman 1 jadi di starter di buang aja. **Tapi mungkin bisa di improve tanpa harus dibuang**
   2. Feature Encoding<br>
   Udah cukup baik
   3. EDA<br>
   Udah dikit" **Perlu di tambahin sih**, perlu metode lain buat menghandle variable `GPA`.
   4. Handling Outlier
2. Handle Imbalance
   1. `stratify`<br>
      Lewat `StratifiedKFold`
   2. Imbalance Learn
      1. SMOTENC<br>
         SMOTE tapi bisa handle variable categorik juga (hasilnya kurang memuaskan)
3. Ensemble
   Ensemble 9 dari 10 Fold pakai `rata-rata` (hasilnya kurang memuaskan)

## Note

1. Untuk sekarang kyknya fokus dulu buat nyari model terbaiknya. Kalau buat **Tuning**-nya nanti" aja setelah model terbaiknya dah dapet.
2. Entah kenapa scalling data pada variable `GPA` malah nurunin true score padahal nambah bagus di CV

© Catatan Cakrawala 2021