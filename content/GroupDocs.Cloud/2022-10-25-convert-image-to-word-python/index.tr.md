---
title: "Python'da Görüntüyü Word'e Dönüştür"
seoTitle: "Görüntüyü Python'da Word'e Dönüştür | Python PNG, JPG, BMP GIF'den Word'e | varsayalım"
description: "Görüntüleri Python'da Word'e dönüştürmek için Python Word API'yi kullanın. Tek bir görüntüyü veya birden çok görüntüyü Python'da bir Word'e dönüştürün."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /tr/words/convert-image-to-word-python/
author: "Osman Aziz"
summary: "Bazı durumlarda, tek bir görüntüyü veya bir grup görüntüyü bir Word belgesine dönüştürmeniz gerekir. Bu işlemi programlı olarak gerçekleştirmek için bu makale, görüntülerin Python'da Word DOC DOCX'e nasıl dönüştürüleceğini gösterir."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Python'da Görüntüyü Word'e Dönüştür">}}

MS Word [DOC][1] ve [DOCX][9] biçimleri, zengin metin belgeleri oluşturmak için yaygın olarak kullanılır. Metni biçimlendirebilir ve Word belgelerine resimler gibi çeşitli öğeler ekleyebilirsiniz. Bazı durumlarda, tek bir görüntüyü veya bir grup görüntüyü bir Word belgesine dönüştürmeniz gerekir. Bu işlemi programlı olarak gerçekleştirmek için bu makale, görüntülerin Python'da Word DOC DOCX'e nasıl dönüştürüleceğini gösterir.

* [Python Görüntüsünden Word'e Dönüştürücü Kitaplığı](#Library-to-Convert-Image-to-Word)
* [Python'da Bir Görüntüyü Word DOC'a Dönüştürün](#Convert-an-Image-to-Word)
* [Birden Çok Görüntüyü Python'da DOCX'e Dönüştürün](#Convert-Multiple-Images-to-Word)

## Python Image to Word Converter Kitaplığı - Ücretsiz İndirme {#Library-to-Convert-Image-to-Word}

Görüntüyü Word DOC/DOCX'e dönüştürmek için [Aspose.Words for Python][3] kullanacağız. DOC, DOCX, vb. dahil olmak üzere Word belgeleriyle çalışmak için zengin özelliklere sahip bir kitaplıktır. Kitaplıkta, Word belgelerinin ileri geri dönüştürülmesi için yerleşik bir dönüştürücü vardır. Aşağıdaki pip komutunu kullanarak [PyPI][4]'ten kitaplığı yükleyebilirsiniz.

```
> pip install aspose-words
```

## Python'da Bir Görüntüyü Word DOC'a Dönüştürün {#Convert-an-Image-to-Word}

Python'da bir görüntüyü Word DOC'a dönüştürme adımları aşağıda verilmiştir.

* Öncelikle, Document sınıfını kullanarak yeni bir belge oluşturun.
* Ardından, bir DocumentBuilder nesnesi oluşturun ve onu Document nesnesiyle başlatın.
* DocumentBuilder.insertimage(fileName) yöntemini kullanarak belgeye resim ekleyin.
* Son olarak Document.save(fileName) yöntemini kullanarak Word belgesini kaydedin.

Aşağıdaki kod örneği, Python'da bir PNG görüntüsünün DOC'a nasıl dönüştürüleceğini gösterir.

```
import aspose.words as aw

# Yeni bir belge oluştur
doc = aw.Document()

# Bir belge oluşturucu oluşturun
builder = aw.DocumentBuilder(doc)

# Belgeye resim ekle
builder.insert_image("logo.png")

# DOC olarak kaydet
doc.save("image-to-word.doc")
```

## Python'da Birden Çok Görüntüyü Word'e Dönüştürün {#Convert-Multiple-Images-to-Word}

Bir önceki bölümde sadece tek bir görseli Word belgesine dönüştürdük. Ancak bazı durumlarda birden fazla görseli aynı anda dönüştürmeniz gerekebilir. Python'da birden çok görüntüyü bir Word DOCX'e dönüştürme adımları aşağıda verilmiştir.

* Öncelikle, Document sınıfını kullanarak yeni bir belge oluşturun.
* Ardından, bir DocumentBuilder nesnesi oluşturun ve onu Document nesnesiyle başlatın.
* İstediğiniz klasörden görüntü dosyalarının listesini alın.
* Görüntü dosyaları listesinde dolaşın ve DocumentBuilder.insertimage(fileName) yöntemini kullanarak her görüntüyü belgeye ekleyin.
* Son olarak Document.save(fileName) yöntemini kullanarak Word belgesini kaydedin.

Aşağıdaki kod örneği, birden çok görüntünün Python'da bir Word DOCX'e dönüştürülmesini gösterir.

```
import aspose.words as aw
import os

# Resim dizini
dir = "D:\\images\\"

# Yeni bir belge oluştur
doc = aw.Document()

# Bir belge oluşturucu oluşturun
builder = aw.DocumentBuilder(doc)

# Klasördeki görüntüler arasında geçiş yap
for imageFile in os.listdir(dir):
    # Belgeye resim ekle
    builder.insert_image(os.path.join(dir, imageFile))

# DOCX olarak kaydet
doc.save("images-to-word.docx")
```

## Image to DOC Python Converter - Ücretsiz Lisans Alın {#Get-a-Free-License}

[Ücretsiz bir geçici lisans alarak][5] değerlendirme sınırlamaları olmaksızın görüntüleri Word biçimlerine dönüştürebilirsiniz.

## Python Image to DOCX Converter - Devamını Okuyun

Aspose.Words for Python hakkında [documentation][6] kullanarak daha fazlasını keşfedebilirsiniz. Herhangi bir sorunuz olması durumunda [forumumuz][7] aracılığıyla bize bildirmekten çekinmeyin.

## Çözüm

Bu yazıda, Python'da bir görüntüyü Word belgesine nasıl dönüştüreceğinizi öğrendiniz. Ayrıca, birden çok görüntünün program aracılığıyla bir Word DOC/DOCX belgesine nasıl dönüştürüleceğini de gösterdik. Sağlanan kod örneklerini uygulamanıza kolayca entegre edebilir ve görüntüyü DOC veya DOCX'e dönüştürme işlemini gerçekleştirebilirsiniz.

## Ayrıca bakınız

* [C# kullanarak PDF Dosyaları Oluşturun – .NET PDF API](https://blog.aspose.com/tr/pdf/create-pdf-files-using-csharp/)
* [Python'da Word'ü PDF'ye Dönüştür](https://blog.aspose.com/tr/words/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




