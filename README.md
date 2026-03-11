# CAD Dataset Preprocessing

Repository ini berisi dokumentasi pengolahan data medis dari dataset Z-Alizadeh Sani untuk persiapan prediksi penyakit arteri koroner (CAD).

## Fitur Utama
* **Kategorisasi Fitur**: Klasifikasi otomatis berdasarkan persentase outlier dan nilai skewness.
* **Implementasi Scaling**: Transformasi data dilakukan secara manual tanpa library tambahan:
    * **Robust Scaler**: Untuk fitur dengan outlier > 2% (contoh: FBS, TG, PLT).
    * **Standard Scaler**: Untuk fitur berdistribusi normal (contoh: Age, Weight).
    * **Min-Max Scaler**: Untuk fitur miring tanpa outlier ekstrem (contoh: LDL, HDL).
* **Strukturisasi Data**: Penataan ulang kolom dengan menempatkan variabel Cath (target) pada posisi terakhir (paling kanan).

## Struktur File
* `Wijdanadam_Rafifilmi_N_103052400027_partisipatif1.ipynb`: File utama proses pembersihan dan transformasi data.
* `preprocessed_cad_alizadeh.csv`: Dataset hasil akhir yang telah melalui proses scaling.

## Sumber Data
Dataset berasal dari materi perkuliahan, kemungkinan merupakan subset atau turunan dari Z-Alizadeh Sani Dataset (UCI Machine Learning Repository).
