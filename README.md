Pemrograman Lanjut (Advanced Programming) 2024/2025 Genap
* Nama    : Nashwa Ghania
* NPM     : 2306241770
* Kelas   : Pemrograman Lanjut - A

<details>
<summary>Module 5</summary>

## JMeter Report and Test Results
### Test Plan 1 (all-student request)
Before Optimization: <br/>


After Optimization: <br/>


### Test Plan 2 (all-student-name request)
Before Optimization: <br/>


After Optimization: <br/>


### Test Plan 3 (highest-gpa request)
Before Optimization: <br/>


After Optimization: <br/>



## Reflection
1. **Perbedaan antara JMeter dan IntelliJ Profiler**<br/>
JMeter digunakan untuk pengujian kinerja (load testing) dan mengukur responsivitas aplikasi, throughput, serta tingkat 
kesalahan dengan mensimulasikan banyak permintaan dari pengguna. IntelliJ Profiler digunakan untuk menganalisis performa 
pada level kode, seperti penggunaan CPU, alokasi memori, serta mendeteksi bottleneck pada proses eksekusi kode.<br/><br/>

2. **Bagaimana proses profiling membantu mengidentifikasi titik lemah aplikasi**<br/>
Profiling memungkinkan untuk mengidentifikasi loop yang tidak efisien, pemanggilan database yang berlebihan, serta 
kebocoran memori.<br/><br/>

3. **Apakah IntelliJ Profiler efektif dalam menganalisis dan mengidentifikasi bottleneck?**<br/>
IntelliJ Profiler sangat efektif karena dapat menunjukkan penggunaan CPU, aktivitas thread, serta waktu eksekusi query 
database secara real-time. Hal ini memungkinkan untuk menemukan area mana yang paling banyak memakan sumber daya.<br/><br/>

4. **Tantangan utama saat melakukan pengujian performa dan profiling serta cara mengatasinya**<br/>
Proses optimasi kode cukup menantang karena saya harus mengeksplorasi berbagai solusi, menganalisis performa aplikasi, 
serta menjalankan profiling berulang kali untuk mengidentifikasi bottleneck dan memastikan hasil yang optimal. 
Selain itu, saya juga perlu memastikan perubahan yang dilakukan tidak mengganggu fungsionalitas aplikasi.<br/><br/>

5. **Manfaat utama menggunakan IntelliJ Profiler**<br/>
Memberikan wawasan mendalam tentang penggunaan CPU dan memori, mengidentifikasi query database yang lambat, dan membantu 
mengoptimalkan logika bisnis yang memakan banyak sumber daya.<br/><br/>

6. **Cara menangani hasil yang tidak konsisten antara profiling dengan IntelliJ Profiler dan pengujian performa JMeter**<br/>
Caranya adalah dengan mencocokkan endpoint yang lambat di JMeter dengan hasil profiling di IntelliJ Profiler untuk 
menentukan apakah masalahnya berasal dari latensi database, overhead jaringan, atau kode yang terlalu berat secara komputasi.<br/><br/>

7. **Strategi untuk mengoptimalkan kode setelah menganalisis hasil pengujian dan profiling**
- Menggunakan metode repository yang efisien seperti findTopByOrderByGpaDesc.
- Memanfaatkan stream API untuk manipulasi data yang lebih ringkas.
- Menghindari penggabungan string secara manual, gunakan Collectors.joining().
- Melakukan profiling berulang untuk mengidentifikasi bottleneck yang tersisa.
- Melakukan load testing ulang untuk memastikan performa yang stabil.

</details>