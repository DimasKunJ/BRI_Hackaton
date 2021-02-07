# People Analytics

## Brief

Binary Classification menggunakan AUC sebagai metricsnya.

## To Do

1. Nyoba menggunakan model lain (Boosting klo bisa kyk XGboost, Catboost, LGBM, dst)
2. Nyobain macem" Imbalance Learning
3. Feature Selection(?)

## Log

Model - model yang udah di coba dan scorenya bisa di liat [di sini ](https://docs.google.com/spreadsheets/d/1dmZuqc1NWMqfaD5kJaXSihSpY6FnKLt5WguQh2YXDrk/edit?usp=sharing)

## Hal yang udah dilakuin

1. Preprocess
   1. Imputation (Missing data)<br>
   Missing datanya cuman 1 jadi di starter di buang aja. **Tapi mungkin bisa di improve tanpa harus dibuang**
   2. Feature Encoding<br>
   Udah cukup baik
   3. EDA<br>
   Udah dikit" **Perlu di tambahin sih** dan mungkin itu ada cara lain buat ngehandle variable `GPA`
2. Handle Imbalance<br>
Masih pake cara biasa yaitu `stratify` biar proporsi data yang imbalance di train sma di valid sama. **Mesti di improve pake imbalance learning**

## Note

1. Untuk sekarang kyknya fokus dulu buat nyari model terbaiknya. Kalau buat **Tuning**-nya nanti" aja setelah model terbaiknya dah dapet.
2. Entah kenapa scalling data pada variable `GPA` malah nurunin true score di model `Random Forest Classifier`

© Catatan Cakrawala 2021