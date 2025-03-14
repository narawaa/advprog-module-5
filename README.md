Pemrograman Lanjut (Advanced Programming) 2024/2025 Genap
* Nama    : Nashwa Ghania
* NPM     : 2306241770
* Kelas   : Pemrograman Lanjut - A

## JMeter Report and Test Results
### Test Plan 1 (all-student request)
**Before Optimization: **<br/>
<img width="1070" alt="testresults1" src="https://github.com/user-attachments/assets/43a524fd-f0a8-4ceb-90c2-9b897ff3ec64" />

<img width="1070" alt="test_plan_1" src="https://github.com/user-attachments/assets/22eceec8-0460-4544-8ac5-e0bbbb65cd4f" />

**After Optimization: **<br/>
<img width="1070" alt="Screenshot 2025-03-14 at 19 52 48" src="https://github.com/user-attachments/assets/4fcfe7fd-b51d-41d3-8fbd-bfb24470f08e" />

### Test Plan 2 (all-student-name request)
**Before Optimization: <br/>**
<img width="1070" alt="testresults2" src="https://github.com/user-attachments/assets/d80a7de5-881c-49e1-943a-a5f4ad487169" />

<img width="1070" alt="test_plan_2" src="https://github.com/user-attachments/assets/b71213f4-920f-4d53-9b5e-798179356796" />

**After Optimization: <br/>**
<img width="1070" alt="Screenshot 2025-03-14 at 19 53 12" src="https://github.com/user-attachments/assets/e368b1dd-61c4-4eb0-9826-ecc0f6a051d6" />

### Test Plan 3 (highest-gpa request)
**Before Optimization: <br/>**
<img width="1070" alt="testresults3" src="https://github.com/user-attachments/assets/43fb086c-f822-47a2-95cf-13caa8d203db" />

<img width="1070" alt="test_plan_3" src="https://github.com/user-attachments/assets/8711830d-12ca-4f16-9326-26602a137893" />

**After Optimization: <br/>**
<img width="1070" alt="Screenshot 2025-03-14 at 19 53 28" src="https://github.com/user-attachments/assets/bf3203b2-7571-4e83-9fd7-cd939e152f7a" />

**Kesimpulan:**
Berdasarkan analisis visual pada gambar, terlihat adanya peningkatan performa yang signifikan. Sample time menunjukkan bahwa waktu eksekusi sebelum optimisasi jauh lebih lama dibandingkan setelah optimisasi. Peningkatan ini membuktikan efektivitas strategi yang diterapkan dengan dukungan JMeter untuk uji performa dan IntelliJ Profiler untuk analisis mendalam.

## Reflection
1. **Perbedaan antara JMeter dan IntelliJ Profiler**<br/>
JMeter digunakan untuk pengujian performa (load testing) dan mengukur responsivitas aplikasi, throughput, serta tingkat kesalahan dengan mensimulasikan banyak permintaan dari pengguna. IntelliJ Profiler digunakan untuk menganalisis performa pada level kode, seperti penggunaan CPU, alokasi memori, serta mendeteksi bottleneck pada proses eksekusi kode.<br/><br/>

2. **Bagaimana proses profiling membantu mengidentifikasi titik lemah aplikasi**<br/>
Profiling memungkinkan untuk mengidentifikasi loop yang tidak efisien, pemanggilan database yang berlebihan, serta kebocoran memori.<br/><br/>

3. **Apakah IntelliJ Profiler efektif dalam menganalisis dan mengidentifikasi bottleneck**<br/>
IntelliJ Profiler sangat efektif karena dapat menunjukkan penggunaan CPU, aktivitas thread, serta waktu eksekusi query database secara real-time. Hal ini memungkinkan untuk menemukan area mana yang paling banyak memakan sumber daya.<br/><br/>

4. **Tantangan utama saat melakukan pengujian performa dan profiling serta cara mengatasinya**<br/>
Proses optimasi kode cukup menantang karena saya harus mengeksplorasi berbagai solusi, menganalisis performa aplikasi, serta menjalankan profiling berulang kali untuk mengidentifikasi bottleneck dan memastikan hasil yang optimal. Selain itu, saya juga perlu memastikan perubahan yang dilakukan tidak mengganggu fungsionalitas aplikasi.<br/><br/>

5. **Manfaat utama menggunakan IntelliJ Profiler**<br/>
Memberikan wawasan mendalam tentang penggunaan CPU dan memori, mengidentifikasi query database yang lambat, dan membantu mengoptimalkan logika yang memakan banyak sumber daya.<br/><br/>

6. **Cara menangani hasil yang tidak konsisten antara profiling dengan IntelliJ Profiler dan pengujian performa JMeter**<br/>
Caranya adalah dengan mencocokkan endpoint yang lambat di JMeter dengan hasil profiling di IntelliJ Profiler untuk menentukan apakah masalahnya berasal dari latensi database, overhead jaringan, atau kode yang terlalu berat secara komputasi.<br/><br/>

7. **Strategi untuk mengoptimalkan kode setelah menganalisis hasil pengujian dan profiling**
- Menggunakan metode repository yang efisien seperti findTopByOrderByGpaDesc.
- Memanfaatkan stream API untuk manipulasi data yang lebih ringkas.
- Menghindari penggabungan string secara manual dengan menggunakan Collectors.joining().
- Melakukan profiling berulang untuk mengidentifikasi bottleneck yang tersisa.
- Melakukan load testing ulang untuk memastikan performa yang stabil.
  
