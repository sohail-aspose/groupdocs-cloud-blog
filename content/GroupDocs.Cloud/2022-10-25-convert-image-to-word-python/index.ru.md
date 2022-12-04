---
title: "Преобразование изображения в слово в Python"
seoTitle: "Преобразование изображения в Word в Python | Python PNG, JPG, BMP GIF в Word | Aspose"
description: "Используйте Python Word API для преобразования изображений в Word на Python. Преобразуйте одно или несколько изображений в Word на Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /ru/words/convert-image-to-word-python/
author: "Усман Азиз"
summary: "В некоторых случаях вам необходимо преобразовать одно изображение или группу изображений в документ Word. Чтобы выполнить эту операцию программно, в этой статье показано, как преобразовать изображения в Word DOC DOCX в Python."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Преобразование изображения в слово в Python">}}

Форматы MS Word [DOC][1] и [DOCX][9] широко используются для создания форматированных текстовых документов. Вы можете форматировать текст и вставлять в документы Word различные элементы, например изображения. В некоторых случаях вам необходимо преобразовать одно изображение или группу изображений в документ Word. Чтобы выполнить эту операцию программно, в этой статье показано, как преобразовать изображения в Word DOC DOCX в Python.

* [Библиотека конвертера изображений Python в Word](#Library-to-Convert-Image-to-Word)
* [Преобразование изображения в Word DOC в Python](#Convert-an-Image-to-Word)
* [Преобразование нескольких изображений в DOCX в Python](#Convert-Multiple-Images-to-Word)

## Библиотека конвертера изображений Python в Word — скачать бесплатно {#Library-to-Convert-Image-to-Word}

Для преобразования изображения в Word DOC/DOCX мы будем использовать [Aspose.Words for Python][3]. Это многофункциональная библиотека для работы с документами Word, включая DOC, DOCX и т. д. Библиотека имеет встроенный конвертер для прямого преобразования документов Word. Вы можете установить библиотеку из [PyPI][4] с помощью следующей команды pip.

```
> pip install aspose-words
```

## Преобразование изображения в Word DOC в Python {#Convert-an-Image-to-Word}

Ниже приведены шаги для преобразования изображения в Word DOC в Python.

* Сначала создайте новый документ, используя класс Document.
* Затем создайте объект DocumentBuilder и инициализируйте его с помощью объекта Document.
* Вставьте изображение в документ, используя метод DocumentBuilder.insert_image(fileName).
* Наконец, сохраните документ Word, используя метод Document.save(fileName).

В следующем примере кода показано, как преобразовать изображение PNG в DOC в Python.

```
import aspose.words as aw

# Создать новый документ
doc = aw.Document()

# Создать конструктор документов
builder = aw.DocumentBuilder(doc)

# Вставить изображение в документ
builder.insert_image("logo.png")

# Сохранить как DOC
doc.save("image-to-word.doc")
```

## Преобразование нескольких изображений в Word в Python {#Convert-Multiple-Images-to-Word}

В предыдущем разделе мы преобразовали только одно изображение в документ Word. Однако в некоторых случаях вам может потребоваться преобразовать несколько изображений одновременно. Ниже приведены шаги для преобразования нескольких изображений в Word DOCX в Python.

* Сначала создайте новый документ, используя класс Document.
* Затем создайте объект DocumentBuilder и инициализируйте его с помощью объекта Document.
* Получите список файлов изображений из нужной папки.
* Прокрутите список файлов изображений и вставьте каждое изображение в документ, используя метод DocumentBuilder.insert_image(fileName).
* Наконец, сохраните документ Word, используя метод Document.save(fileName).

В следующем примере кода показано преобразование нескольких изображений в Word DOCX в Python.

```
import aspose.words as aw
import os

# Каталог изображений
dir = "D:\\images\\"

# Создать новый документ
doc = aw.Document()

# Создать конструктор документов
builder = aw.DocumentBuilder(doc)

# Перебирать изображения в папке
for imageFile in os.listdir(dir):
    # Вставить изображение в документ
    builder.insert_image(os.path.join(dir, imageFile))

# Сохранить как DOCX
doc.save("images-to-word.docx")
```

## Конвертер изображений в DOC Python — получите бесплатную лицензию {#Get-a-Free-License}

Вы можете конвертировать изображения в форматы Word без ограничений пробной версии, [получив бесплатную временную лицензию][5].

## Конвертер изображений Python в DOCX — Подробнее

Вы можете узнать больше об Aspose.Words for Python, используя [документацию][6]. Если у вас возникнут какие-либо вопросы, сообщите нам об этом через наш [форум][7].

## Вывод

В этой статье вы узнали, как преобразовать изображение в документ Word в Python. Мы также продемонстрировали, как программно преобразовать несколько изображений в документ Word DOC/DOCX. Вы можете легко интегрировать предоставленные образцы кода в свое приложение и выполнить преобразование изображения в DOC или DOCX.

## Смотрите также

* [Создание PDF-файлов с помощью C# — .NET PDF API](https://blog.aspose.com/ru/2020/12/02/create-pdf-files-using-csharp/)
* [Преобразование Word в PDF в Python](https://blog.aspose.com/ru/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




