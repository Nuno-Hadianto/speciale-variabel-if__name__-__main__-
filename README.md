# speciale-variabel-if__name__-__main__-
apa itu ?? / what is dis ???

```
*** Pengertian ***

jika name sama dengan main adalah konstruksi yang menggunakan pernyataan aliran kontrol untuk memungkinkan Anda mengeksekusi kode hanya ketika skrip Python dijalankan dan bukan ketika diimpor sebagai modul.

** Contoh if __name__ == '__main__' **

Apa yang dilakukan oleh konstruk __name__ == '__main__' adalah ia menggunakan pernyataan kondisional if untuk memeriksa apakah Anda menjalankan modul (atau skrip) secara langsung, atau jika Anda mengimpor modul dari modul lain.

=================================
def nunox():
    print('samlekom mamank')

if __name__ == '__main__':
  nunox()
==================================

Apa yang dikatakannya adalah ini:

Jika Anda menjalankan modul secara langsung, jalankan fungsinya, jika Anda mengimpor modul, jangan dijalankan.

Singkatnya, kode di dalam pernyataan aliran kontrol (control flow statement) (jika name sama dengan main) dijalankan hanya ketika skrip dijalankan dari baris perintah atau melalui IDE. Itu tidak dieksekusi ketika digunakan sebagai modul oleh skrip Python lain. Dengan ungkapan(idiom) ini, Anda dapat memastikan bahwa skrip Python Anda berperilaku sebagaimana mestinya ketika dijalankan sebagai program mandiri atau sebagai modul dalam proyek yang lebih besar.

Mari kita uraikan.

*** Bagaimana Cara Kerja __name__ == '__main__'? ***

Pernyataan kondisional if __name__ == '__main__' adalah konstruksi pemrograman Python yang mengontrol eksekusi skrip. Saat skrip Python dijalankan, juru bahasa(interpreter) menyetel variabel nama ke string '__main__' jika skrip tersebut adalah program utama yang dijalankan. Jika file diimpor sebagai modul, maka variabel nama disetel ke nama modul.

*** Dasar-dasar tentang cara Python menjalankan file ***

Setiap kali Python membaca skrip, ia melakukan dua tindakan:
1. itu menetapkan beberapa variabel khusus(special) seperti __name__;
2. itu mengeksekusi kode yang ditemukan dalam skrip.

*** Apa yang __name__ Lakukan Saat Menjalankan Skrip ? ***

Atribut __name__ adalah variabel bawaan Python yang mewakili(represent) nama modul atau skrip saat ini.

Dengan kata sederhana, saat Anda menjalankan skrip Python, Python menetapkan nilai __name__. Jika Anda menjalankan skrip secara langsung, nilainya akan disetel ke "__main__".

Mari kita buat file main_module.py sebagai contoh.

Script akan mencetak variabel __name__.
![1](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/750e90b6-665e-415a-ad41-2dfdc6eb6f7f)





