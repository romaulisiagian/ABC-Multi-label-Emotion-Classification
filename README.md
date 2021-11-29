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
<h2 id="user-content-pendahuluan" dir="auto"><a id="user-content-pendahuluan" class="anchor" aria-hidden="true" href="#pendahuluan"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Pendahuluan</h2>
<h4 id="user-content-lb" dir="auto"><a id="user-content-latar-belakang" class="anchor" aria-hidden="true" href="#latar-belakang"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Latar Belakang</h4>
<p dir="auto">
Natural Language Processing (NLP) merupakan salah satu bidang ilmu dalam kategori keilmuan Artificial Intelligence (AI). NLP fokus pada pengolahan bahasa alami yang diterapkan pada piranti komputer, sehingga komputer dapat memahami apa yang diinginkan oleh pengguna. Bahasa alami tidak memiliki compiler atau interpreter untuk dapat dipahami sebagai halnya bahasa pemrograman, akan tetapi ketika bahasa alami ini diterapkan dalam NLP maka dapat menggunakan bahasa pemrograman sebagai instruksi dari manusia kepada komputer. NLP digunakan dalam aplikasi-aplikasi yang membutuhkan pengolahan bahasa. Model aplikasinya diantaranya berupa aplikasi yang dapat digunakan untuk meringkas dokumen, penerjemahan bahasa asing, hingga aplikasi mengenai ucapan pengguna.  Pada penelitian kali ini, pengaplikasian NLP yang akan dibahas adalah emotion recognition. 
</p>
<p dir="auto">
Agar konten yang menggambarkan emotion dapat dipahami dan dicari, terdapat suatu metode yang cukup efektif untuk menangani masalah ini yaitu dengan cara pelabelan. Pelabelan dilakukan dengan memberikan tanda atau label terhadap suatu teks. Pelabelan dipilih karena label merupakan bagian dari struktur hirarkis dari teks, sehingga dapat mewakili konten dari suatu teks. Jika data yang akan dianalisis banyak, maka klasifikasi multi-label  dapat dijadikan solusi untuk melabelkan konten ke dalam beberapa kelas sekaligus. Setelah konten terlabeli, untuk mengetahui suatu konten masuk ke dalam label mana, perlu dilakukan proses klasifikasi. Emosi seseorang dapat dilihat dari segi ucapan, ekspresi wajah, nada suara dan juga teks yang ditulis. Pengekspresian emosi dapat diketahui dalam sebuah kalimat. Emosi dalam kalimat  dapat diidentifikasi melalui kata sifat. Klasifikasi emosi merupakan tugas penting dalam Natural Language Processing (NLP). Secara otomatis menyimpulkan emosi merupakan langkah awal untuk aplikasi seperti chatbots emosional (Zhou et al, 2018). Pada pengklasifikasian emosi memilih lebih dari 1 emosi dalam teks. Pengklasifikasian emosi sangat diperlukan untuk mengetahui suasana hati atau  perasaan orang tersebut. Pengekspresian emosi dapat kita lihat dari postingan , chat ataupun komentar di media sosial. 
</p>
<p dir="auto">
Deteksi emosi membantu menjelaskan sifat kompleks dari emosi yang muncul secara bersamaan , sehingga memberikan pemahaman tentang karakteristik setiap emosi.  Analisis emosi memiliki beberapa manfaat dalam berbagai aplikasi dalam perdagangan, kesehatan masyarakat, kesejahteraan sosial dan lain-lain. Analisis ini menunjukkan  sikap terhadap suatu target atau topik. Seringkali ketika kita membaca teks atau email, seringkali kita tidak mengetahui emosi yang terkandung pada teks tersebut sehingga perlu dilakukan klasifikasi emosi dengan menggunakan multi label seperti emosi kegembiraan, kemarahan, kecemasan , kekecewaan, ketidaksetujuan dan lain-lain. Sehingga perlu dilakukan penelitian untuk melakukan klasifikasi emosi dengan multi label dalam sebuah kalimat.  
</p>
<br>
<h4 id="user-content-rm" dir="auto"><a id="user-content-rumusan-masalah" class="anchor" aria-hidden="true" href="#rumusan-masalah"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Rumusan Masalah</h4>
<ul dir="auto">
  <li>Bagaimana penerapan algoritma Support Vector Machine dalam pengklasifikasian emosi multi-label berdasarkan skor prediksi emosi yang dihasilkan terhadap data training dan testing?</li>
</ul>
<ul dir="auto">
  <li>Bagaimana hasil dari pengklasifikasian emosi multi-lable dengan menggunakan algoritma SVM?</li>
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
