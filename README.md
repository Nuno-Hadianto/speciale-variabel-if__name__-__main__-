# special-variabel-if__name__-__main__-
apa itu ?? / what is dis ???


*** Pengertian ***
```
jika name sama dengan main adalah konstruksi yang menggunakan pernyataan aliran kontrol untuk memungkinkan Anda mengeksekusi kode hanya ketika skrip Python dijalankan dan bukan ketika diimpor sebagai modul.
```

** Contoh if __name__ == '__main__' **
```
Apa yang dilakukan oleh konstruk __name__ == '__main__' adalah ia menggunakan pernyataan kondisional if untuk memeriksa apakah Anda menjalankan modul (atau skrip) secara langsung, atau jika Anda mengimpor modul dari modul lain.
```
![Screenshot 2023-10-18 170149](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/2b63ba4a-7bca-456d-ab76-35c92716384a)

```
Apa yang dikatakannya adalah ini:
Jika Anda menjalankan modul secara langsung, jalankan fungsinya, jika Anda mengimpor modul, jangan dijalankan.
Singkatnya, kode di dalam pernyataan aliran kontrol (control flow statement) (jika name sama dengan main) dijalankan hanya ketika skrip dijalankan dari baris perintah atau melalui IDE. Itu tidak dieksekusi ketika digunakan sebagai modul oleh skrip Python lain. Dengan ungkapan(idiom) ini, Anda dapat memastikan bahwa skrip Python Anda berperilaku sebagaimana mestinya ketika dijalankan sebagai program mandiri atau sebagai modul dalam proyek yang lebih besar.

Mari kita uraikan.
```

*** Bagaimana Cara Kerja __name__ == '__main__'? ***
```
Pernyataan kondisional if __name__ == '__main__' adalah konstruksi pemrograman Python yang mengontrol eksekusi skrip. Saat skrip Python dijalankan, juru bahasa(interpreter) menyetel variabel nama ke string '__main__' jika skrip tersebut adalah program utama yang dijalankan. Jika file diimpor sebagai modul, maka variabel nama disetel ke nama modul.
```
*** Dasar-dasar tentang cara Python menjalankan file ***
```
Setiap kali Python membaca skrip, ia melakukan dua tindakan:
1. itu menetapkan beberapa variabel khusus(special) seperti __name__;
2. itu mengeksekusi kode yang ditemukan dalam skrip.
```
*** Apa yang __name__ Lakukan Saat Menjalankan Skrip ? ***
```
Atribut __name__ adalah variabel bawaan Python yang mewakili(represent) nama modul atau skrip saat ini.
Dengan kata sederhana, saat Anda menjalankan skrip Python, Python menetapkan nilai __name__. Jika Anda menjalankan skrip secara langsung, nilainya akan disetel ke "__main__".
Mari kita buat file main_module.py sebagai contoh.
```
```
Script akan mencetak variabel __name__.
```
![Screenshot 2023-10-16 212055](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/e0c09edd-6b3c-44b7-8931-7dd2d7d98c0c)

```
Ketika saya menjalankan kode menggunakan python main_module.py di Terminal, skrip akan mengembalikan __main__.
```
![Screenshot 2023-10-16 212510](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/7415c6b3-c34c-4741-b271-ebacf11247c8)

*** Apa yang dilakukan __name__ Saat Mengimpor Skrip ***
```
Sekarang, mari kita lihat apa yang terjadi ketika saya mencoba mengimpor modul.
Saya membuat skrip python import_main.py yang tujuannya hanya untuk mengimpor main_module.py.
```

![Screenshot 2023-10-16 213338](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/32ba5a60-9279-4b06-9d06-64bfc8e193c3)

```
Jika Anda belum memahami cara kerja impor, yang dilakukannya hanyalah mengeksekusi skrip yang Anda impor.
Saat saya menjalankan python import_main.py, ia menjalankan fungsi print(__name__) yang ku tulis di main_module.py.
```
![Screenshot 2023-10-16 215707](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/4ffad15e-a081-41b3-9e97-4dff6560958e)


*** Penutup: if __name__ == '__main__' ***
```
Kembali ke main_module.py, mari kita perjelas dengan contoh lengkap.
```
![Screenshot 2023-10-18 164606](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/c3f88e0e-a916-44f0-8dd2-bbee20e4f7e3)

```
Apa yang main_module.py sekarang akan lakukan adalah:
Jika saya menjalankan main_module.py, cetak/print Fungsi/Function Main() Dieksekusi, lain jika/else if saya mengimpor main_module.py print Fungsi main() tidak dijalankan.
```
![Screenshot 2023-10-18 164644](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/e26428b3-719e-4653-88a7-f13260e0b2b4)


*** Jalankan Fungsi Main() Dari Import_main ***
```
Sekarang, Jika mau, Anda dapat menjalankan fungsi apa pun yang tersedia di main_module.py dari import_main.py.
```
![Screenshot 2023-10-18 165210](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/829889ca-dd77-45d3-9de2-da53244a78e9)

![Screenshot 2023-10-18 165300](https://github.com/Nuno-Hadianto/speciale-variabel-if__name__-__main__-/assets/63713816/a924b29a-0dd8-442c-9fb9-70bd1ad29c7e)

```
Ini dia, jika __name__ == '__main__' berguna untuk mengimpor Modul untuk menggunakan fungsi di dalamnya, tanpa menjalankan skrip.
```











