# Moodify
Aplikasi web yang yang digunakan untuk translasi dan  meringkas bacaan dari foto buku fisik. <br/>

NAMA KELOMPOK ANDA  <br/>
Ketua Kelompok: Alvin Indra Kurniawan  <br/>
Anggota 1: Alvin Indra Kurniawan -19/439808/TK/48538 <br/>
Anggota 2:  Dimas Mahendra Nugraha - 19/444048/TK/49244 <br/>
Anggota 3: Roby Attoillah - 19/444068/TK/49264  <br/>
Anggota 4: Raihan Ramadhan Hanif Mintarso - 19/444066/TK/49262 <br/>


aplikasi web ini akan memproses photo buku fisik yang kita input, setelahnya akan diproses dam akan menampilkan text hasil ringkasan dari foto buku.
untuk skematik kerangkanya seperti berukut>> <br/>

#### Skematik
![image info](./assets/skematik_PR5.png) <br/>

#### Paparan 
Pada Project ini, menggunakan NextJs sebagai framework ReactJs untuk keperluan frontendnya. dan akan dideploy menggunakan azure app service.
pada bagian frontend nantinya akan menuntun pengguna untuk melakukan input foto buku fisik yang ingin mereka dapatkan hasil ringkasannya. <br/>

setelah foto tersebut diterima selanjutnya akan diteruskan ke azure app service untuk keperluan backend yang akan disimpan data sementaranya di CosmosDB.<br/>
pada bagian backend terdapat beberaoa flow yang berlangsung:<br/>

1. Foto akan diproses dan dibaca oleh azure cognitive service-computer vision dan didapatkan isi text dari foto yang diinput tadi.<br/>
2. setelah itu text akan ditranslate dengan menggunakan azure cognitive service-Translator dan didapatkan diterjemahkan ke bahasa yang diinginkan<br/>
3. setelah itu text yang sudah diterjemahkan, selanjutnya di rinkas pada ML yaitu NLTK dengan menggunakan text summarization.<br/>
4. text yang telah di ringkas ditampilkan pada web Moodify.<br/>
<br/>
Skematik masih dapat berubah sesuai dengan pertimbangan dan setelah mendapatkan ilmu baru ketika melakukan praktikum di modul selanjutnya.<br/>