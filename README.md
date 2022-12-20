# PRAKTIKUM-11

NAMA    : NADYA KHAIRUNNISA

NIM     : 312210133

KELAS   : TI.22.A1

## Exception Handling
- Exception (eksepsi) merupakan suatu kesalahan (error) yang terjadi saat proses eksekusi program   sedang berjalan
- Kesalahan ini akan menyebabkan program berakhir dengan tidak normal.

## Handling
- Penanganan file adalah bagian penting dari aplikasi apa pun.

## Assertion
Assertion(pernyataan) adalah kewajaran program yang kamu bisa aktif/nonaktifkan ketika kamu selesai menjalankan program.
### The Assert Statement
- Saat menemukan pernyataan, Python mengevaluasi ekspresi yang menyertainya, yang mana semoga benar. Jika ekspresi salah, Python memunculkan pengecualian AssertionError.

#### Sintaks untuk pernyataan yaitu :

assert Expression[, Arguments]

Jika pernyataan gagal, Python menggunakan ArgumentExpression. ArgumentExpression sebagai argumen-argumen untuk AssertionError. 
Pengecualian AssertionError dapat ditangkap dan ditangani seperti pengecualian lainnya menggunakan try kecuali pernyataan, tetapi jika dibiarkan mereka akan menghentikan program dan menghasilkan backtrace.

#### Contoh :
- Berikut adalah fungsi fungsi yang mengubah suhu dari derajat Kelvin menjadi derajat Fahrenheit.Karena nol derajat Kelvin dingin, fungsi fungsi menyimpannya jika melihat negatif negatif suhu.
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![ERROR 1](https://user-images.githubusercontent.com/115801823/208604341-df020bab-42ed-4dd6-add3-87e33a816ba8.PNG)

![HASIL ERROR 1](https://user-images.githubusercontent.com/115801823/208604420-ed81ef56-43ef-420c-94ab-89cbc3c09c15.PNG)

## Menangani Pengecualian
Jika Anda memiliki beberapa kode mencurigakan yang mungkin mengeluarkan pengecualian, Anda dapat mempertahankan program Anda letakkan kode yang mencurigakan di *try: blok. Setelah coba: blok, sertakan pernyataan sertakan *except: statement, diikuti oleh blok kode yang menangani masalah seanggun mungkin.

#### Contoh :
- Contoh-contoh ini membuka file, menulis konten file, dan keluar dengan aman karena ada tidak masalah
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![ERROR 2](https://user-images.githubusercontent.com/115801823/208604694-426db412-54a0-434e-b58a-49cfe757d9e5.PNG)

![HASIL ERROR 2](https://user-images.githubusercontent.com/115801823/208604773-77885986-51aa-4693-8b95-93ca77743316.PNG)

- Contoh ini mencoba membuka file yang Anda tidak memiliki izin menulis, sehingga membuat file pengecualian
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![ERROR 3](https://user-images.githubusercontent.com/115801823/208605653-aeed67d5-eb1d-4cae-9101-5c9846417a4f.PNG)

![HASIL ERROR 3](https://user-images.githubusercontent.com/115801823/208605686-2f15ddb3-1c89-42d6-8369-5ce86d2c36db.PNG)

## Fasal kecuali tanpa Pengecualian
- Anda juga dapat menggunakan pernyataan exception tanpa exception yang didefinisikan sebagai berikut:

try: You do your operations here; ...................... except: If there is any exception, 
then execute this block. ...................... else: If there is no exception then execute this block.

Pernyataan coba-kecuali jenis ini menangkap semua pengecualian pengecualian yang terjadi. Menggunakan percobaan seperti try-expect pernyataan tidak dianggap sebagai praktik pemrograman yang baik, karena mereka menangkap semuanya pengecualian tetapi tidak membuat programmer mengidentifikasi kemungkinan penyebab masalah terjadi

## Klausa kecuali dengan Berbagai Pengecualian
- Anda juga dapat menggunakan pernyataan exception yang sama untuk menangani beberapa exception sebagai berikut:

try: You do your operations here; ...................... except(Exception1[, Exception2[,...ExceptionN]]]): If there is any exception from the given exception list, then execute this block. ...................... else: If there is no exception then execute this block.

### Klausa coba-akhirnya 
#### Contoh :
- Jika Anda tidak memiliki izin untuk membuka file dalam mode tulis yang dapat ditulis, maka ini akan menghasilkan hasil berikut:

![ERROR 4](https://user-images.githubusercontent.com/115801823/208605883-8ace5a62-8696-4fe5-b80d-0fc0a3f90001.PNG)

![HASIL ERROR 4](https://user-images.githubusercontent.com/115801823/208605924-0b157f20-7eb3-4714-840d-a02d9e1404bf.PNG)

- Contoh yang sama dapat ditulis lebih bersih sebagai berikut:

![ERROR 5](https://user-images.githubusercontent.com/115801823/208606005-7a851bc1-3e98-4eb3-97b5-f3eff7e2723e.PNG)

![HASIL ERROR 5](https://user-images.githubusercontent.com/115801823/208606084-5fd5aa75-9198-411a-83fe-830fa7d093c7.PNG)

- Ketika exception dilempar ke dalam blok try, eksekusi segera dilanjutkan ke akhir memblok. Setelah semua pernyataan di blok akhirnya dieksekusi, pengecualian dimunculkan lagi dan ditangani dalam pernyataan kecuali jika ada di lapisan berikutnya yang lebih tinggi dari percobaan-kecuali penyataan.

### Argumen Pengecualian 
#### Contoh :
- Berikut adalah contoh untuk satu pengecualian
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![ERROR 6](https://user-images.githubusercontent.com/115801823/208606205-2e552431-749d-4b36-b15b-72ec3f37cdaa.PNG)

![HASIL ERROR 6](https://user-images.githubusercontent.com/115801823/208606250-85cea2f7-e46b-4ecd-9817-bdb27f5f378d.PNG)

