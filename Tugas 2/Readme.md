<h1>TUGAS 2 RISET INFORMATIKA</h1>
<h2>Contoh Paper Metode / Metodologi Penelitian</h2><br>

<ol>
  <li>
    Metode<br> 
    Judul : MRI-based brain tumour image detection using CNN based deep learning method <br>
    Link : https://www.sciencedirect.com/science/article/pii/S277252862200022X
  </li><br>
  <li>
    Metodologi <br>
    Judul : Classification of White blood cell using Convolution Neural Network <br>
    Link : https://www.sciencedirect.com/science/article/abs/pii/S1746809421007539
  </li>
</ol>
<br>

<h1>
  Metode Penelitian Pendeteksian Kerusakan Cat pada Bak Dump Truck Menggunakan Convolutional Neural Network (CNN)
</h1>

<ol>
  <li>Arsitektur Convolutional Neural Network (CNN)</li>
    <p align="justify">&emsp;&emsp;Pemilihan arsitektur kecerdasan buatan CNN (Convolutional Neural Network) yang tepat adalah langkah kunci dalam pengembangan sistem ini. Lapisan-lapisan     konvolusi dalam CNN akan membantu model dalam mengidentifikasi pola-pola kompleks dalam gambar, sedangkan pada lapisan-lapisan pengelompokan (pooling) bertujuan membantu dalam mereduksi dimensi data. Dengan menggunakan arsitektur yang sesuai, diharapkan model yang dibuat dapat belajar secara efektif dan akurat mengenali kerusakan pada cat bak dump truck dari gambar yang diberikan.
      
  <li>Pengumpulan Dataset</li>
      <p align="justify">&emsp;&emsp;Pada tahap pengumpulan dataset, dilakukan pengumpulan data foto dump truck dari samping yang mencakup berbagai kondisi dan jenis kerusakan pada bak. Data dikumpulkan dengan berbagai variasi kondisi cahaya, sudut pengambilan gambar, dan tipe kerusakan (seperti retak, korosi, dan deformasi). Pengumpulan data yang representatif menjadi kunci keberhasilan pelatihan model CNN. Dengan melakukan gabungan gambar-gambar dengan keragaman yang memadai, diharapkan model CNN dapat belajar untuk mengenali berbagai bentuk dan intensitas kerusakan cat pada bak dump truck.
      <ul>
        <li>Pra-pemrosesan Data</li>
        <p align="justify">&emsp;&emsp;Pada tahap pra-pemrosesan data, citra dump truck yang dijadikan masukan menjalani dua proses utama yaitu wrapping dan cropping. Dalam proses wrapping, citra masukan akan diperiksa untuk menemukan tepi objek utama dalam citra tersebut. Tepi tersebut akan digunakan sebagai acuan dalam menentukan ukuran maksimal objek sehingga hasil dari cropping objek pada citra tetap utuh. Tahap awal pelatihan dimulai dengan mengubah citra input menjadi bentuk vektor, memungkinkan representasi visual dari citra tersebut dalam model. Proses ini direpresentasikan dalam Diagram 2.1.
Dimulai dengan citra berukuran sembarang, ukuran citra kemudian diubah menjadi 140 x 140. Dataset citra yang digunakan dalam penelitian ini adalah gambar dump truck dengan kerusakan cat bagian luar bak truk dan gambar dump truck tanpa kerusakan pada cat baknya, yang diolah sebagai dataset pelatihan. Setelah pengumpulan data, CNN akan memproses data tersebut sebagai data latih. Setelah CNN membentuk fitur, fitur tersebut dapat mendeteksi kerusakan pada cat bak dump truck. Proses ini bertujuan memastikan bahwa citra-citra yang akan diolah memiliki dimensi yang konsisten, memudahkan proses pelatihan model dan meningkatkan akurasi deteksi kerusakan.
        <li>Proses Training</li>
          <p align="justify">&emsp;&emsp;Proses pelatihan merupakan fase krusial di mana CNN akan diajarkan untuk mencapai tingkat akurasi tinggi dalam melakukan klasifikasi. Tahap ini terdiri dari dua proses utama, yaitu feedforward dan backpropagation. Pada tahap feedforward, diperlukan pengaturan jumlah dan dimensi lapisan yang akan dibangun, serta ukuran subsampling, dan citra vektor yang dihasilkan dari data dump truck yang rusak. Proses feedforward melibatkan konvolusi dan Max pooling untuk mereduksi ukuran citra dan memperluas jaringan neuronnya, menciptakan variasi data yang kaya untuk pembelajaran. Hasil dari proses feedforward adalah bobot yang akan digunakan untuk mengevaluasi jaringan saraf yang telah dibentuk. Proses ini diilustrasikan dalam Gambar 2.2.
        <ul>
          <li>Proses Feedforward : Proses ini merupakan langkah pertama dalam pelatihan. Di sini, beberapa lapisan dibentuk untuk mengklasifikasikan data citra menggunakan bobot dan bias yang diperbarui dari tahap backpropagation. Hasil dari tahap feedforward ini juga akan digunakan kembali selama proses pengujian.
          <li>Proses Backpropagation : Tahap backpropagation, yang merupakan langkah kedua dalam pelatihan, melibatkan pelacakan kesalahan dari lapisan output hingga lapisan input. Selama tahap ini, bobot dan bias yang baru diperoleh untuk menandai kesalahan dalam feedforward.
          <li>Perhitungan Gradient : Dalam proses gradient pada jaringan konvolusi, nilai bobot dan bias yang baru dihitung, dan informasi ini esensial untuk proses pelatihan selanjutnya. Langkah-langkah ini secara bersama-sama
membentuk dasar pelatihan CNN, memastikan bahwa model memahami
dan belajar dari data citra dump truck dengan efisien dan akurat.
        </ul>
        <li>Proses Testing</li>
          <p align="justify">&emsp;&emsp;Proses pengujian (testing) merupakan tahapan penting dalam evaluasi model yang telah dilatih. Pada tahap ini, klasifikasi dilakukan dengan menggunakan bobot dan bias yang telah diperoleh setelah proses pelatihan (training). Proses pengujian tidak jauh berbeda dengan pelatihan, kecuali bahwa tidak ada proses backpropagation setelah proses feedforward. Hasil akhir dari tahap ini mencakup akurasi dari klasifikasi yang dilakukan, data yang tidak berhasil diklasifikasi, nomor citra yang gagal diklasifikasi, dan struktur jaringan yang terbentuk dari proses feedforward. Dalam proses pengujian, bobot dan bias yang baru diterapkan pada proses feedforward, yang kemudian menghasilkan lapisan output. Lapisan output ini sepenuhnya terhubung dengan label yang telah disediakan. Hasil dari lapisan output ini memberikan informasi tentang data yang berhasil diklasifikasi dengan benar dan data yang gagal diklasifikasi. Proses ini memungkinkan evaluasi terhadap kinerja model, memastikan bahwa model CNN mampu mengenali dan mengklasifikasikan citra dump truck dengan akurasi yang diharapkan. Alur proses pengujian ini dijelaskan dalam Gambar 2.3,
menggambarkan langkah-langkah yang diambil dalam menguji kemampuan model pada data uji.
      </ul>
  
  <li>Validasi dan Analisis Hasil</li>
  <p align="justify">&emsp;&emsp;Setelah model telah dianggap optimal, validasi dilakukan dengan melakukan pengujian pada data yang belum pernah dilihat sebelumnya, yang mungkin mencakup gambar-gambar dump truck dari produksi terbaru. Hasil dari pendeteksian kerusakan cat akan dianalisis secara mendalam, termasuk melakukan identifikasi jenis kerusakan yang paling sering terdeteksi dan area spesifik pada bak dump truck yang paling rentan terhadap kerusakan cat. Analisis ini bertujuan memberikan wawasan berharga bagi pabrik karoseri untuk melakukan perbaikan dan meningkatkan proses pengecatan mereka.
</ol>
