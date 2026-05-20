# MB-CBA: Multi-Band CNN–BiLSTM–Attention untuk Deteksi Kognitif EEG
### Pipeline lengkap: Kaggle dataset → Multi-band preprocessing → LOSO evaluation

**Perubahan utama dari notebook asli:**
- Data `.mat` dibaca langsung dari Kaggle (14 channel, sama seperti notebook asli)
- Ditambahkan **multi-band decomposition** (delta/theta/alpha/SMR/beta) → input (14×5=70, 256)
- Evaluasi diubah dari random split → **LOSO cross-validation** (cross-subject)
- Model ditambahkan **attention mechanism**
- Semua metrik Q1 dilaporkan: accuracy, weighted F1, macro F1, per-class F1, confusion matrix

