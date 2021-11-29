# ABC-Multi-label-Emotion-Classification
<p dir="auto"> Kelompok ABC - Multi lable Emotion Classification </p>
<ol dir="auto">
  <li>11S18027 Romauli Siagian</li>
  <li>11S18003 Febby Irene Siringoringo</li>
  <li>11S18011 Awit Hutabalian</li>
  <li>11S18032 Rido Sitanggang</li>
  <li>11S18057 Marlyse Sitorus</li>
  <li>11S18059 Kristiane Purba</li>
</ol>

*Proyek ini menggunakan :*
<li> Python 3.8
<li> Google Colab

  <h1 dir="auto"><a id="user-content-daftar-isi" class="anchor" aria-hidden="true" href="#daftar-isi"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Daftar Isi</h1>
<ol dir="auto">
  <li><a href="#pendahuluan">Pendahuluan</a></li>
  <ul dir="auto">
    <li><a href="#lb">Latar Belakang</a></li>
    <li><a href="#rm">Rumusan Masalah</a></li>
    <li><a href="#tp">Tujuan Penelitian</a></li>
    <li><a href="#mp">Manfaat Penelitian</a></li>
    <li><a href="#rlp">Ruang Lingkup Penelitian</a></li>
  </ul>
  <li><a href="#hp">Hasil Penelitian</a></li>
</ol>
<hr>

  <hr>
<h2 id="user-content-pendahuluan" dir="auto"><a id="user-content-pendahuluan" class="anchor" aria-hidden="true" href="#pendahuluan"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Pendahuluan</h2>
<h4 id="user-content-lb" dir="auto"><a id="user-content-latar-belakang" class="anchor" aria-hidden="true" href="#latar-belakang"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Latar Belakang</h4>
<p dir="auto">
Emosi adalah pola reaksi yang kompleks, yang melibatkan pengalaman, perilaku, dan fisiologis, di mana seorang individu mencoba untuk menangani masalah atau peristiwa yang signifikan secara pribadi. Dalam kehidupan sehari-hari, penyampaian emosi dapat disampaikan secara non-verbal menggunakan ekspresi wajah maupun verbal berupa tingkah laku. Emosi bersifat subjektif dan temporer yang muncul atau dipicu oleh stimulus seperti perlakuan dari orang sekitar atau lingkungannya.
</p>
<p dir="auto">
Deteksi emosi dilakukan dengan pendekatan klasifikasi emosi. Klasifikasi adalah proses dengan menggabungkan atau mengelompokkan dua atau lebih data yang memiliki kesamaan pada suatu kriterianya. Terdapat beberapa metode yang dapat digunakan untuk melakukan klasifikasi pada teks, diantaranya Support Vector Machine, Naïve Bayes, K-Nearest Neighbor, Multinomial Naïve Bayes, Multi Task Regression, Algoritma Incremental Regression, dan lain-lain. Sedangkan untuk metode fitur ekstraksi juga terdapat beberapa yang sering digunakan, diantaranya TF-IDF, N-Gram, Word Embedding, dan lain-lain. Namun pada penelitian ini beberapa pendekatan atau metode yang akan digunakan dalam melakukan fitur ekstraksi yaitu TF-IDF yang kemudian diklasifikasikan dengan metode Naïve Bayes. Berdasarkan penelitian sebelumnya fitur TF-IDF memberikan hasil yang lebih baik sekitar 3% - 4% jika dibandingkan dengan fitur N-Gram (Ahuja et al., 2019). TF-IDF merupakan teknik yang paling sederhana sehingga mudah untuk melakukan pengecekan corpus yang besar dan juga dapat menghitung banyak istilah yang ada dalam sebuah dokumen. Algoritma pengklasifikasian Naive Bayes adalah salah satu pengklasifikasian statistik, pengklasifikasian ini dapat memprediksi probabilitas anggota kelas data yang akan masuk ke kelas tertentu, menurut perhitungan probabilitas. Klasifikasi ini menunjukkan akurasi dan kecepatan yang tinggi bila diterapkan kedalam database yang besar. Metode ini sering digunakan untuk memecahkan masalah di bidang Machine Learning karena metode ini memiliki tingkat akurasi yang tinggi dengan perhitungan sederhana.
</p>
<br>
<h4 id="user-content-rm" dir="auto"><a id="user-content-rumusan-masalah" class="anchor" aria-hidden="true" href="#rumusan-masalah"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Rumusan Masalah</h4>
<ul dir="auto">
  <li>Bagaimana mengklasifikasikan emosi berdasarkan data komentar menggunakan algoritma Naive Bayes.</li>
</ul>
<br>
<h4 id="user-content-tp" dir="auto"><a id="user-content-tujuan-penelitian" class="anchor" aria-hidden="true" href="#tujuan-penelitian"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Tujuan Penelitian</h4>
<ul dir="auto">
  <li>Melakukan implementasi Naive Bayes dalam mengklasifikasikan emosi berdasarkan data komentar.</li>
</ul>
<br>
<h4 id="user-content-mp" dir="auto"><a id="user-content-manfaat-penelitian" class="anchor" aria-hidden="true" href="#manfaat-penelitian"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Manfaat Penelitian</h4>
<ul dir="auto">
  <li>Penelitian ini diharapkan mampu melakukan klasifikasi emosi berdasarkan kalimat yang diberikan dengan memberi label pada setiap kelas emosi sesuai dengan dataset yang diberikan.</li>
</ul>
<br>
<h4 id="user-content-rlp" dir="auto"><a id="user-content-ruang-lingkup-penelitian" class="anchor" aria-hidden="true" href="#ruang-lingkup-penelitian"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Ruang Lingkup Penelitian</h4>
<ul dir="auto">
  <li>Data yang diolah dikumpulkan dari website reddit.</li>
  <li>Penelitian ini melakukan normalisasi hanya dalam bentuk huruf.</li>
  <li>Penelitian ini menerima inputan dalam bentuk kalimat yang mempunyai kata singkatan bahasa Inggris.</li>
  <li>Penelitian ini akan melakukan normalisasi kata singkatan yang di-input oleh user.</li>
</ul>
