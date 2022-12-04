---
title: "Konversi Gambar ke Word dengan Python"
seoTitle: "Konversi Gambar ke Kata dengan Python | Python PNG, JPG, BMP GIF ke Word | Asumsikan"
description: "Gunakan Python Word API untuk mengonversi gambar ke Word dengan Python. Konversi satu gambar atau beberapa gambar menjadi Word dengan Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /id/words/convert-image-to-word-python/
author: "Usman Aziz"
summary: "Dalam kasus tertentu, Anda harus mengonversi satu atau beberapa gambar ke dokumen Word. Untuk melakukan operasi ini secara terprogram, artikel ini menunjukkan cara mengonversi gambar ke Word DOC DOCX dengan Python."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Konversi Gambar ke Word dengan Python">}}

Format MS Word [DOC][1] dan [DOCX][9] banyak digunakan untuk membuat dokumen rich text. Anda dapat memformat teks dan menyisipkan berbagai elemen dalam dokumen Word seperti gambar. Dalam kasus tertentu, Anda harus mengonversi satu atau beberapa gambar ke dokumen Word. Untuk melakukan operasi ini secara terprogram, artikel ini menunjukkan cara mengonversi gambar ke Word DOC DOCX dengan Python.

* [Pustaka Pengonversi Gambar ke Kata Python](#Library-to-Convert-Image-to-Word)
* [Konversi Gambar ke Word DOC dengan Python](#Convert-an-Image-to-Word)
* [Konversi Banyak Gambar ke DOCX dengan Python](#Convert-Multiple-Images-to-Word)

## Pustaka Pengonversi Gambar ke Kata Python - Unduhan Gratis {#Library-to-Convert-Image-to-Word}

Untuk konversi gambar ke Word DOC/DOCX, kita akan menggunakan [Aspose.Words for Python][3]. Ini adalah pustaka kaya fitur untuk bekerja dengan dokumen Word termasuk DOC, DOCX, dll. Pustaka ini memiliki konverter bawaan untuk konversi bolak-balik dokumen Word. Anda dapat menginstal pustaka dari [PyPI][4] menggunakan perintah pip berikut.

```
> pip install aspose-words
```

## Konversi Gambar ke Word DOC dengan Python {#Convert-an-Image-to-Word}

Berikut ini adalah langkah-langkah untuk mengubah gambar menjadi Word DOC dengan Python.

* Pertama, buat dokumen baru menggunakan kelas Document.
* Kemudian, buat objek DocumentBuilder dan inisialisasi dengan objek Document.
* Sisipkan gambar ke dalam dokumen menggunakan metode DocumentBuilder.insertimage(fileName).
* Terakhir, simpan dokumen Word menggunakan metode Document.save(fileName).

Contoh kode berikut menunjukkan cara mengonversi gambar PNG ke DOC dengan Python.

```
import aspose.words as aw

# Buat dokumen baru
doc = aw.Document()

# Buat pembuat dokumen
builder = aw.DocumentBuilder(doc)

# Sisipkan gambar ke dalam dokumen
builder.insert_image("logo.png")

# Simpan sebagai DOC
doc.save("image-to-word.doc")
```

## Konversi Banyak Gambar ke Word dengan Python {#Convert-Multiple-Images-to-Word}

Di bagian sebelumnya, kami hanya mengonversi satu gambar ke dokumen Word. Namun, dalam kasus tertentu, Anda mungkin perlu mengonversi lebih dari satu gambar sekaligus. Berikut ini adalah langkah-langkah untuk mengonversi banyak gambar menjadi Word DOCX dengan Python.

* Pertama, buat dokumen baru menggunakan kelas Document.
* Kemudian, buat objek DocumentBuilder dan inisialisasi dengan objek Document.
* Dapatkan daftar file gambar dari folder yang diinginkan.
* Ulangi daftar file gambar dan masukkan setiap gambar ke dalam dokumen menggunakan metode DocumentBuilder.insertimage(fileName).
* Terakhir, simpan dokumen Word menggunakan metode Document.save(fileName).

Contoh kode berikut menunjukkan konversi beberapa gambar ke Word DOCX dengan Python.

```
import aspose.words as aw
import os

# Direktori gambar
dir = "D:\\images\\"

# Buat dokumen baru
doc = aw.Document()

# Buat pembuat dokumen
builder = aw.DocumentBuilder(doc)

# Ulangi gambar dalam folder
for imageFile in os.listdir(dir):
    # Sisipkan gambar ke dalam dokumen
    builder.insert_image(os.path.join(dir, imageFile))

# Simpan sebagai DOCX
doc.save("images-to-word.docx")
```

## Image to DOC Python Converter - Dapatkan Lisensi Gratis {#Get-a-Free-License}

Anda dapat mengonversi gambar ke format Word tanpa batasan evaluasi dengan [mendapatkan lisensi sementara gratis][5].

## Konverter Gambar Python ke DOCX - Baca Lebih Lanjut

Anda dapat mempelajari lebih lanjut tentang Aspose.Words for Python menggunakan [dokumentasi][6]. Jika Anda memiliki pertanyaan, silakan beri tahu kami melalui [forum][7] kami.

## Kesimpulan

Pada artikel ini, Anda telah mempelajari cara mengubah gambar menjadi dokumen Word dengan Python. Kami juga mendemonstrasikan cara mengonversi banyak gambar ke dokumen Word DOC/DOCX secara terprogram. Anda dapat dengan mudah mengintegrasikan contoh kode yang disediakan ke dalam aplikasi Anda dan melakukan konversi gambar ke DOC atau DOCX.

## Lihat juga

* [Hasilkan File PDF menggunakan C# – .NET PDF API](https://blog.aspose.com/id/pdf/create-pdf-files-using-csharp/)
* [Konversi Word ke PDF dengan Python](https://blog.aspose.com/id/words/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




