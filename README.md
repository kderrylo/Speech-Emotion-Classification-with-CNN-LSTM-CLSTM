# Speech Emotion Recognition

Speech Emotion Recognition (SER) bertujuan untuk mengenali dan mengklasifikasikan emosi yang terdapat pada suara manusia. Proyek ini mengimplementasikan tiga model deep learning: Convolutional Neural Network (CNN), Long Short-Term Memory (LSTM), dan kombinasi Convolutional-LSTM (CLSTM) untuk melakukan klasifikasi emosi berdasarkan data suara.

Proyek ini mengeksplorasi tiga model deep learning (CNN, LSTM, dan CLSTM) untuk melakukan klasifikasi emosi suara manusia. Dataset dilatih dengan rasio train-test sebesar 3:1 menggunakan 40 epoch. Evaluasi dilakukan dengan *classification report* dari *scikit-learn*, yang mencakup metrik akurasi, presisi, *recall*, dan *f1-score*. 

Hasil akhir dari evaluasi menunjukkan bahwa model CLSTM memberikan hasil terbaik dengan akurasi 83%, sedangkan model LSTM menghasilkan akurasi terendah yaitu 72%. Semua model berhasil mencapai performa rata-rata di atas 70%, dengan detail metrik bervariasi antara 66% hingga 90% pada setiap emosi yang diujicobakan.

## Fitur

- Klasifikasi emosi suara dengan tiga model: CNN, LSTM, dan CLSTM.
- Pelatihan model dengan rasio data train-test sebesar 3:1.
- Evaluasi model menggunakan metrik akurasi, presisi, *recall*, dan *f1-score*.
- Mampu mengenali beberapa emosi dengan akurasi hingga 83%.

## Evaluasi

Setiap model diuji menggunakan *classification report* dari *scikit-learn*, mencakup metrik akurasi, presisi, recall, dan f1-score. Hasil evaluasi adalah sebagai berikut:

| Model | F1-score | Presisi | Recall | Akurasi |
|-------|----------|---------|--------|---------|
| CNN   | 80%      | 80%     | 80%    | 80%     |
| LSTM  | 72%      | 72%     | 72%    | 72%     |
| CLSTM | 83%      | 83%     | 83%    | **83%** |

Setiap emosi memiliki metrik yang bervariasi dengan kisaran antara 66% hingga 90% di ketiga model.

## Pengembangan Selanjutnya

Beberapa langkah pengembangan lebih lanjut yang dapat dilakukan:
1. **Ekstraksi Fitur Lanjutan:** Mengeksplorasi penggunaan teknik ekstraksi fitur yang lebih canggih seperti *wav2vec* atau embedding lain yang berbasis suara untuk meningkatkan performa model.
2. **Model Lainnya:** Bereksperimen dengan model lain seperti Transformer atau menggunakan teknik transfer learning dari model suara yang sudah terlatih.
3. **Penyesuaian Hyperparameter:** Mengoptimalkan hyperparameter seperti jumlah lapisan, ukuran batch, atau teknik regularisasi untuk meningkatkan akurasi model.
4. **Augmentasi Data:** Menambahkan data augmentasi pada dataset untuk meningkatkan keanekaragaman data pelatihan.

---

**Catatan:** Proyek ini masih dalam tahap pengembangan dan hasil akurasi dapat terus ditingkatkan seiring dengan eksperimen dan pengembangan lebih lanjut.

---

Jika ada pertanyaan lebih lanjut atau ingin berkontribusi, silakan buat *issue* atau kirim *pull request*.
