KATA PENGANTAR

Puji syukur diucapkan kehadirat Allah SWT. Atas segala rahmat nya sehingga makalah ini dapat tersusun sampai selesai. Tidak lupa mengucapkan terima kasih terhadap bantuan dari pihak yang telah berkontribusi dengan memberikan sumbangan baik pikiranh maupun materi.
Penulis berharap semoga makalah ini dapat menambah pengetahuan dan pengalaman bagi pembaca. Bahkan kami berharap lebih jauh lagi agar makalah ini bisa pembaca praktikkan dalam kehidupan sehari-hari.
Bagi saya sebagai penyusun merasa bahwa masih banyak kekurangan dalam penyusunan makalah ini karena keterbatasan pengetahuan dan pengalaman saya. Untuk itu saya sangat mengharapkan kritik dan saran yang membangun dari pembaca demi kesempurnaan makalah ini.








						Palembang, 20 Agustus 2024


						Ridho Mulya




DAFTAR ISI

JUDUL…………………………………………………………………………………………………..i
KATA PENGANTAR………………………………………………………………….ii
DAFTAR ISI……………………………………………………..………………………iii
BAB I
PENDAHULUAN……………………………………………………………………………...1
Tinjauan Pustaka………………………………………………………………...2

BAB  II 

Metodologi……………………………………………………………………………………...3

Hasil Pembahasan………………………………………………………………...4

BAB III 
Kesimpulan…………………………………………………………………………………...5
DAFTAR PUSTAKA



BAB 1

Pendahuluan
Internet of Things (IoT) adalah konsep yang menghubungkan berbagai perangkat fisik yang dilengkapi dengan sensor, perangkat lunak, dan teknologi lainnya ke internet. Perangkat-perangkat ini mampu mengumpulkan dan bertukar data, memungkinkan mereka berinteraksi dengan lingkungan mereka, pengguna, atau perangkat lain tanpa memerlukan interaksi manusia-ke-manusia atau manusia-ke-komputer.manusia-ke-komputer
Secara sederhana, IoT memungkinkan perangkat "pintar" untuk saling terhubung dan berkomunikasi melalui jaringan internet, menciptakan sistem yang dapat memantau, menganalisis, dan merespons kondisi lingkungan secara otomatis.

Tinjauan Pustaka
1. Sensor Suhu
DHT11/DHT22: Sensor suhu dan kelembaban ini populer karena murah dan mudah digunakan. DHT11 memiliki akurasi yang lebih rendah dibandingkan DHT22, tetapi keduanya banyak digunakan dalam proyek IoT skala kecil.
LM35: Sensor suhu analog dengan akurasi tinggi dan keluaran tegangan yang linier. Sensor ini sering digunakan dalam aplikasi yang memerlukan pengukuran suhu presisi.
DS18B20: Sensor suhu digital yang menggunakan komunikasi 1-Wire. Cocok untuk aplikasi dengan banyak sensor karena dapat dihubungkan dalam satu kabel
2. Sensor Kelembaban
DHT11/DHT22: Selain mengukur suhu, sensor ini juga mengukur kelembaban relatif dengan rentang akurasi yang berbeda.
HDC1080: Sensor digital yang mengukur suhu dan kelembaban dengan akurasi tinggi dan konsumsi daya rendah, ideal untuk aplikasi IoT portabel.
AM2302: Mirip dengan DHT22, sensor ini juga dapat mengukur kelembaban dan suhu dengan akurasi yang lebih baik.
3. Sensor Kualitas Udara
MQ-135: Sensor gas yang dapat mendeteksi berbagai gas berbahaya seperti amonia (NH3), nitrogen oksida (NOx), alkohol, benzena, asap, dan karbon dioksida (CO2). Sering digunakan untuk mendeteksi polusi udara di area perkotaan.
PMS5003: Sensor partikel yang digunakan untuk mengukur konsentrasi partikel debu PM1.0, PM2.5, dan PM10. Sensor ini sangat penting dalam pemantauan kualitas udara, terutama terkait polusi debu halus.
CCS811: Sensor gas digital yang mengukur konsentrasi karbon dioksida (CO2) dan senyawa organik volatil (VOC) total. Sensor ini sering digunakan untuk mendeteksi kualitas udara dalam ruangan.
BME680: Sensor multifungsi yang dapat mengukur suhu, kelembaban, tekanan udara, dan kualitas udara (VOC). Sensor ini sangat berguna untuk aplikasi IoT yang memerlukan pengukuran parameter lingkungan yang lengkap.
4. Sensor Tekanan Udara
BMP280: Sensor tekanan udara dan suhu yang sering digunakan dalam aplikasi IoT untuk mengukur ketinggian dan perubahan cuaca.
BME280: Sensor multifungsi yang dapat mengukur tekanan udara, suhu, dan kelembaban. Sensor ini sering digunakan dalam stasiun cuaca portabel.
5. Sensor Cahaya
BH1750: Sensor intensitas cahaya yang mengukur cahaya dalam satuan lux. Sensor ini digunakan untuk aplikasi seperti otomatisasi pencahayaan dan pengukuran paparan cahaya di lingkungan.
TSL2561: Sensor cahaya digital yang mampu mengukur cahaya inframerah dan cahaya tampak, sering digunakan untuk pengukuran intensitas cahaya yang lebih presisi.
6. Sensor Suara
KY-037: Sensor suara yang mendeteksi level suara di sekitarnya. Meskipun tidak langsung terkait dengan kualitas udara, sensor ini bisa digunakan untuk mengukur polusi suara, yang juga merupakan parameter lingkungan penting.

BAB 2

Metodologi
1. Perencanaan dan Identifikasi Kebutuhan
Penentuan Tujuan: Identifikasi masalah spesifik yang ingin diselesaikan oleh sistem IoT. Misalnya, memantau kualitas udara di area perkotaan atau mengelola kelembaban tanah dalam pertanian.
Pemilihan Parameter: Tentukan parameter lingkungan yang akan dipantau (misalnya, suhu, kelembaban, CO2, VOC, dll.).
Studi Kelayakan: Lakukan analisis kelayakan untuk menilai teknologi, biaya, dan waktu yang dibutuhkan untuk mengembangkan prototipe.
2. Desain Sistem
Pemilihan Sensor dan Perangkat Keras: Pilih sensor yang sesuai untuk mengukur parameter yang ditargetkan. Tentukan mikrokontroler (seperti Arduino, Raspberry Pi, atau ESP8266) dan modul komunikasi (Wi-Fi, Zigbee, LoRa) yang akan digunakan.
Arsitektur Sistem: Rancang arsitektur sistem, termasuk bagaimana sensor akan terhubung ke perangkat, cara data akan dikirim ke cloud, dan bagaimana pengguna akan mengakses data tersebut.
Prototipe Awal: Buat sketsa atau diagram alur sistem untuk memvisualisasikan aliran data dari sensor ke pengguna akhir.
3. Pengembangan Prototipe
Pengembangan Perangkat Keras: Rakit perangkat keras sesuai dengan desain sistem. Ini melibatkan pemasangan sensor, mikrokontroler, dan modul komunikasi. Pastikan bahwa semua komponen terhubung dan berfungsi dengan baik.
Pengembangan Perangkat Lunak: Tulis kode untuk mengumpulkan data dari sensor, memproses data, dan mengirimkannya ke cloud. Ini juga mencakup pengembangan antarmuka pengguna (misalnya, dashboard atau aplikasi mobile) untuk mengakses dan memvisualisasikan data.
Integrasi Cloud dan Analisis Data: Hubungkan sistem dengan platform IoT cloud (seperti AWS IoT, Google Cloud IoT, atau Microsoft Azure IoT) untuk penyimpanan, analisis, dan pengolahan data.
4. Pengujian Laboratorium
Validasi Fungsionalitas: Uji sistem di laboratorium untuk memastikan bahwa semua komponen bekerja sesuai desain. Lakukan uji fungsional untuk memastikan sensor dapat mengukur parameter dengan akurat dan mengirimkan data ke cloud.
Pengujian Keandalan: Uji sistem dalam kondisi yang disimulasikan untuk memeriksa keandalan dan ketahanan terhadap gangguan, seperti kehilangan sinyal atau gangguan daya.
Pengujian Kalibrasi: Kalibrasi sensor untuk memastikan pengukuran yang akurat. Bandingkan data dari sensor dengan instrumen referensi untuk memverifikasi akurasi.
5. Pengujian Lapangan
Penempatan Prototipe: Tempatkan prototipe di lokasi sebenarnya yang akan dipantau. Ini bisa berupa lahan pertanian, area perkotaan, atau situs industri, tergantung pada aplikasi yang dikembangkan.
Pengujian Kondisi Nyata: Operasikan sistem dalam kondisi lingkungan sebenarnya. Periksa bagaimana sistem menangani perubahan cuaca, gangguan fisik, atau variasi lainnya.
Pengumpulan Data Jangka Panjang: Biarkan sistem beroperasi selama beberapa waktu untuk mengumpulkan data dalam jangka panjang. Analisis data untuk mengidentifikasi pola atau anomali.
Validasi dan Optimasi: Bandingkan data yang dikumpulkan dengan ekspektasi atau standar yang berlaku. Jika diperlukan, lakukan penyesuaian pada perangkat keras atau perangkat lunak untuk mengoptimalkan kinerja.
6. Analisis dan Evaluasi
Analisis Data: Gunakan data yang dikumpulkan selama pengujian lapangan untuk melakukan analisis mendalam. Identifikasi tren, anomali, atau korelasi yang relevan.
Evaluasi Kinerja: Evaluasi sistem berdasarkan kriteria seperti akurasi, keandalan, konsumsi daya, dan waktu respon. Pertimbangkan juga masukan dari pengguna atau pemangku kepentingan.
Identifikasi Masalah: Temukan kelemahan atau masalah yang terjadi selama pengujian lapangan, seperti kesalahan data, kegagalan perangkat, atau masalah konektivitas.
7. Penyempurnaan dan Iterasi
Penyempurnaan Prototipe: Berdasarkan hasil evaluasi, lakukan perbaikan pada prototipe. Ini bisa melibatkan kalibrasi ulang sensor, pengoptimalan kode, atau perbaikan perangkat keras.
Pengujian Ulang: Setelah melakukan perbaikan, lakukan pengujian ulang untuk memastikan bahwa masalah telah terselesaikan dan sistem bekerja dengan lebih baik.
Iterasi Desain: Proses desain dan pengujian dapat diulang beberapa kali sampai prototipe memenuhi semua persyaratan kinerja.
8. Implementasi dan Skalabilitas
Produksi Skala Besar: Jika prototipe telah berhasil diuji, pertimbangkan untuk memproduksi sistem dalam skala besar.
Skalabilitas Sistem: Rancang sistem agar dapat diskalakan untuk menangani lebih banyak perangkat atau data jika diperlukan di masa depan.
Deployment: Implementasikan sistem di lokasi yang lebih luas atau di jaringan IoT yang lebih besar untuk penggunaan yang lebih luas.
Kesimpulan
Prototipe sistem IoT memerlukan perencanaan, pengembangan, dan pengujian yang cermat untuk memastikan bahwa sistem bekerja dengan baik di lingkungan sebenarnya. Pengujian lapangan adalah langkah krusial untuk memastikan bahwa sistem dapat beroperasi dengan andal dalam kondisi dunia nyata, dan memberikan hasil yang sesuai dengan kebutuhan pengguna atau proyek yang sedang dikembangkan.
Hasil dan Pembahasan

1. Ringkasan Data yang Dikumpulkan
Sistem IoT yang diterapkan telah mengumpulkan berbagai data lingkungan secara real-time dari sensor yang terpasang di berbagai lokasi. Data ini meliputi parameter berikut:

Suhu: Data suhu dikumpulkan dari sensor yang terpasang di berbagai titik pemantauan, memberikan gambaran tentang variasi suhu di area yang berbeda.
Kelembaban: Sensor kelembaban memberikan informasi tentang tingkat kelembaban relatif di lokasi yang dipantau, penting untuk memahami kondisi atmosfer.
Kualitas Udara: Data kualitas udara termasuk konsentrasi gas berbahaya seperti CO2, NO2, dan PM2.5, yang memberikan indikasi tentang tingkat pencemaran udara.
2. Analisis Data
Variasi Suhu dan Kelembaban

Data Suhu: Data menunjukkan fluktuasi suhu yang signifikan antara siang dan malam hari, serta perbedaan suhu antara area urban dan rural. Peningkatan suhu di area urban mungkin menunjukkan efek dari urban heat island.
Data Kelembaban: Variasi kelembaban di berbagai lokasi menunjukkan bahwa area dengan vegetasi lebih tinggi memiliki kelembaban yang lebih stabil, sementara area yang lebih kering mengalami fluktuasi yang lebih besar.
Kualitas Udara

Konsentrasi Gas Berbahaya: Data menunjukkan bahwa konsentrasi gas berbahaya cenderung lebih tinggi di area dengan lalu lintas padat dan industri. Puncak konsentrasi sering terjadi selama jam sibuk, yang mengindikasikan hubungan langsung antara aktivitas manusia dan pencemaran udara.
Partikel PM2.5: Pengukuran PM2.5 menunjukkan tingkat polusi yang lebih tinggi di area industri dan dekat jalan raya, yang dapat berdampak negatif pada kesehatan masyarakat.
3. Dampak terhadap Keputusan Lingkungan
Pengelolaan Kualitas Udara

Intervensi Pengendalian Polusi: Data kualitas udara yang menunjukkan konsentrasi gas berbahaya tinggi di area tertentu dapat digunakan untuk merancang kebijakan pengendalian polusi yang lebih efektif. Misalnya, pengaturan emisi kendaraan dan pembatasan kegiatan industri selama jam puncak.
Kampanye Kesadaran: Data ini dapat mendukung kampanye kesadaran publik tentang kualitas udara dan kesehatan. Menyediakan informasi kepada masyarakat tentang tingkat polusi dapat meningkatkan kepedulian dan mendorong perilaku ramah lingkungan.
Perencanaan Kota dan Manajemen Lingkungan

Urban Heat Island Effect: Temuan mengenai fluktuasi suhu di area urban dapat digunakan untuk merancang strategi mitigasi, seperti peningkatan area hijau dan penggunaan material yang lebih reflektif di bangunan dan jalan.
Pengelolaan Vegetasi: Data kelembaban dapat membantu dalam perencanaan dan pengelolaan vegetasi di kota, seperti menentukan lokasi yang ideal untuk penanaman pohon dan pengelolaan taman.
Tanggap Darurat dan Respon Bencana

Deteksi Dini: Data suhu dan kualitas udara yang menunjukkan pola tidak biasa dapat digunakan untuk mendeteksi potensi bencana seperti kebakaran hutan atau pencemaran udara yang tiba-tiba. Ini memungkinkan respon yang lebih cepat dan efisien.
Perencanaan Respon Bencana: Informasi yang akurat tentang kondisi lingkungan dapat membantu dalam perencanaan dan penilaian risiko selama situasi darurat.
Peningkatan Kualitas Hidup

Kesehatan Masyarakat: Dengan menyediakan data akurat tentang kualitas udara dan kondisi lingkungan, sistem IoT dapat membantu meningkatkan kualitas hidup masyarakat. Data ini memungkinkan pengambilan keputusan berbasis bukti untuk memperbaiki kondisi lingkungan yang berdampak langsung pada kesehatan masyarakat.
Kebijakan dan Regulasi

Rekomendasi Kebijakan: Data yang dikumpulkan dapat digunakan untuk merekomendasikan kebijakan baru atau perubahan regulasi yang lebih efektif dalam mengelola kualitas lingkungan. Misalnya, peraturan yang lebih ketat mengenai emisi kendaraan atau penggunaan bahan kimia berbahaya.
4. Kesimpulan
Data yang dikumpulkan dari sistem IoT memberikan wawasan berharga tentang kondisi lingkungan dan dampak aktivitas manusia terhadap kualitas lingkungan. Dengan menganalisis data ini, pembuat kebijakan, perencana kota, dan masyarakat dapat membuat keputusan yang lebih terinformasi untuk meningkatkan pengelolaan lingkungan, mengurangi dampak negatif, dan meningkatkan kualitas hidup.






















BAB 3
Kesimpulan
Manfaat
Pemantauan Real-Time

Manfaat: IoT memungkinkan pemantauan parameter lingkungan seperti suhu, kelembaban, dan kualitas udara secara real-time, memberikan data yang up-to-date untuk analisis dan pengambilan keputusan cepat.
Contoh: Pemantauan kualitas udara di kota-kota besar untuk mengidentifikasi polusi dan merespons dengan kebijakan yang tepat.
Pengumpulan Data yang Luas dan Terperinci

Manfaat: Sistem IoT dapat mengumpulkan data dari banyak lokasi secara bersamaan, memberikan gambaran yang lebih komprehensif tentang kondisi lingkungan.
Contoh: Jaringan sensor untuk memantau kelembaban tanah di area pertanian, membantu dalam manajemen irigasi.
Pengelolaan Sumber Daya yang Efisien

Manfaat: Data dari sensor IoT membantu dalam mengelola sumber daya secara lebih efisien dengan memonitor penggunaan dan mendeteksi kebocoran atau pemborosan.
Contoh: Pemantauan penggunaan air untuk mencegah pemborosan dan memastikan distribusi yang adil.
Peringatan Dini dan Respons Cepat

Manfaat: IoT dapat memberikan peringatan dini tentang perubahan lingkungan yang berbahaya atau bencana alam, memungkinkan respons yang cepat dan efektif.
Contoh: Sistem peringatan dini untuk kebakaran hutan berdasarkan data suhu dan kualitas udara.
Peningkatan Kesadaran dan Partisipasi Publik

Manfaat: Data yang mudah diakses oleh publik dapat meningkatkan kesadaran tentang isu lingkungan dan mendorong partisipasi masyarakat dalam inisiatif pelestarian lingkungan.
Contoh: Aplikasi smartphone yang menyediakan informasi tentang kualitas udara lokal kepada pengguna.
Tantangan
Masalah Privasi dan Keamanan Data

Tantangan: Pengumpulan dan penyimpanan data lingkungan dapat menimbulkan masalah privasi dan keamanan, terutama jika data sensitif atau informasi lokasi disalahgunakan.
Solusi: Implementasi enkripsi data dan kebijakan keamanan yang ketat untuk melindungi informasi.
Kendala Teknologi dan Infrastruktur

Tantangan: Keterbatasan infrastruktur, terutama di daerah terpencil, dapat menghambat pemasangan dan pemeliharaan perangkat IoT.
Solusi: Penggunaan teknologi komunikasi yang rendah daya dan infrastruktur jaringan yang diperluas untuk menjangkau daerah-daerah terpencil.
Konsumsi Energi dan Daya Tahan Baterai

Tantangan: Banyak sensor IoT bergantung pada baterai yang memiliki umur terbatas dan perlu diganti atau diisi ulang secara berkala.
Solusi: Penggunaan teknologi penghemat energi dan pengembangan sensor dengan konsumsi daya rendah.
Kompleksitas Integrasi dan Interoperabilitas

Tantangan: Integrasi berbagai perangkat dan protokol IoT dari berbagai produsen dapat menjadi kompleks, menghambat interoperabilitas.
Solusi: Standarisasi protokol dan penggunaan platform IoT terbuka untuk memfasilitasi integrasi yang lebih baik.
Biaya Implementasi dan Pemeliharaan

Tantangan: Biaya awal untuk implementasi sistem IoT dan pemeliharaan jangka panjang bisa tinggi, terutama untuk skala besar.
Solusi: Perencanaan anggaran yang matang dan pemanfaatan solusi IoT yang skalabel untuk mengurangi biaya.
Analisis dan Pengolahan Data

Tantangan: Volume besar data yang dikumpulkan memerlukan kapasitas penyimpanan dan kemampuan analisis yang signifikan untuk menghasilkan wawasan yang berguna.
Solusi: Penggunaan alat analitik dan teknologi big data untuk mengelola dan menganalisis data secara efisien.
Kesimpulan
Penerapan IoT untuk pemantauan lingkungan menawarkan manfaat signifikan dalam hal pemantauan real-time, pengelolaan sumber daya, dan peningkatan kesadaran publik. Namun, tantangan terkait privasi, keamanan, infrastruktur, dan biaya perlu diatasi untuk memaksimalkan potensi teknologi ini. Dengan solusi yang tepat, IoT dapat berkontribusi besar dalam pengelolaan lingkungan dan keberlanjutan.

Daftar Pustaka

Gubbi, J., Buyya, R., Marusic, S., & Palaniswami, M. (2013). Internet of Things (IoT): A Vision, Architectural Elements, and Future Directions. Future Generation Computer Systems, 29(7), 1645-1660. doi:10.1016/j.future.2013.01.010.

Atzori, L., Iera, A., & Morabito, G. (2010). The Internet of Things: A Survey. Computer Networks, 54(15), 2787-2805. doi:10.1016/j.comnet.2010.05.010.

Ahmed, E., Yaqoob, I., Hashem, I. A. T., Khan, I., Ahmed, A. I. A., Imran, M., & Vasilakos, A. V. (2017). The Role of Big Data Analytics in Internet of Things. Computer Networks, 129, 459-471. doi:10.1016/j.comnet.2017.06.013.

Perera, C., Zaslavsky, A., Christen, P., & Georgakopoulos, D. (2014). Context Aware Computing for The Internet of Things: A Survey. IEEE Communications Surveys & Tutorials, 16(1), 414-454. doi:10.1109/SURV.2013.042313.00197.

Zanella, A., Bui, N., Castellani, A., Vangelista, L., & Zorzi, M. (2014). Internet of Things for Smart Cities. IEEE Internet of Things Journal, 1(1), 22-32. doi:10.1109/JIOT.2014.2306328.
