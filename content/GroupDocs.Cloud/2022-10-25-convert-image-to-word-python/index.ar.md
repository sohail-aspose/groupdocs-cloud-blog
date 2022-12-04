---
title: "تحويل الصورة إلى كلمة في بايثون"
seoTitle: "تحويل الصورة إلى كلمة في بايثون | Python PNG و JPG و BMP GIF إلى Word | أسبوس"
description: "استخدم Python Word API لتحويل الصور إلى Word في Python. قم بتحويل صورة واحدة أو عدة صور إلى كلمة في Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /ar/words/convert-image-to-word-python/
author: "عثمان عزيز"
summary: "في بعض الحالات ، يجب عليك تحويل صورة واحدة أو مجموعة من الصور إلى مستند Word. لإجراء هذه العملية برمجيًا ، توضح هذه المقالة كيفية تحويل الصور إلى Word DOC DOCX في Python."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="تحويل الصورة إلى كلمة في بايثون">}}

يتم استخدام تنسيقات MS Word [DOC][1] و [DOCX][9] على نطاق واسع لإنشاء مستندات نصية منسقة. يمكنك تنسيق النص وإدراج عناصر متنوعة في مستندات Word مثل الصور. في بعض الحالات ، يجب عليك تحويل صورة واحدة أو مجموعة من الصور إلى مستند Word. لإجراء هذه العملية برمجيًا ، توضح هذه المقالة كيفية تحويل الصور إلى Word DOC DOCX في Python.

* [صورة Python إلى مكتبة محول الكلمات](#Library-to-Convert-Image-to-Word)
* [تحويل صورة إلى Word DOC في Python](#Convert-an-Image-to-Word)
* [تحويل صور متعددة إلى DOCX في Python](#Convert-Multiple-Images-to-Word)

## Python Image to Word Converter Library - تنزيل مجاني {#Library-to-Convert-Image-to-Word}

لتحويل الصورة إلى Word DOC / DOCX ، سنستخدم [Aspose.Words for Python][3]. إنها مكتبة غنية بالميزات للعمل مع مستندات Word بما في ذلك DOC و DOCX وما إلى ذلك. تحتوي المكتبة على محول مضمن لتحويل مستندات Word ذهابًا وإيابًا. يمكنك تثبيت المكتبة من [PyPI][4] باستخدام أمر pip التالي.

```
> pip install aspose-words
```

## تحويل صورة إلى Word DOC في Python {#Convert-an-Image-to-Word}

فيما يلي خطوات تحويل صورة إلى مستند Word DOC في Python.

* أولاً ، قم بإنشاء مستند جديد باستخدام فئة المستند.
* ثم قم بإنشاء كائن DocumentBuilder وتهيئته باستخدام كائن Document.
* أدخل الصورة في المستند باستخدام طريقة DocumentBuilder.insert_image(fileName).
* أخيرًا ، احفظ مستند Word باستخدام طريقة Document.save(fileName).

يوضح نموذج التعليمات البرمجية التالي كيفية تحويل صورة PNG إلى DOC في Python.

```
import aspose.words as aw

# قم بإنشاء مستند جديد
doc = aw.Document()

# قم بإنشاء منشئ المستندات
builder = aw.DocumentBuilder(doc)

# أدخل الصورة في المستند
builder.insert_image("logo.png")

# حفظ كملف DOC
doc.save("image-to-word.doc")
```

## تحويل صور متعددة إلى Word في Python {#Convert-Multiple-Images-to-Word}

في القسم السابق ، قمنا بتحويل صورة واحدة فقط إلى مستند Word. ومع ذلك ، في بعض الحالات ، قد تحتاج إلى تحويل أكثر من صورة في وقت واحد. فيما يلي خطوات تحويل صور متعددة إلى Word DOCX في Python.

* أولاً ، قم بإنشاء مستند جديد باستخدام فئة المستند.
* ثم قم بإنشاء كائن DocumentBuilder وتهيئته باستخدام كائن Document.
* احصل على قائمة ملفات الصور من المجلد المطلوب.
* قم بالتكرار خلال قائمة ملفات الصور وأدخل كل صورة في المستند باستخدام طريقة DocumentBuilder.insert_image (fileName).
* أخيرًا ، احفظ مستند Word باستخدام طريقة Document.save(fileName).

يوضح نموذج التعليمات البرمجية التالي تحويل صور متعددة إلى Word DOCX في Python.

```
import aspose.words as aw
import os

# دليل الصور
dir = "D:\\images\\"

# قم بإنشاء مستند جديد
doc = aw.Document()

# قم بإنشاء منشئ المستندات
builder = aw.DocumentBuilder(doc)

# حلقة من خلال الصور في المجلد
for imageFile in os.listdir(dir):
    # أدخل الصورة في المستند
    builder.insert_image(os.path.join(dir, imageFile))

# حفظ بتنسيق DOCX
doc.save("images-to-word.docx")
```

## صورة لتحويل DOC Python - احصل على ترخيص مجاني {#Get-a-Free-License}

يمكنك تحويل الصور إلى تنسيقات Word بدون قيود تقييمية عن طريق [الحصول على ترخيص مؤقت مجاني][5].

## Python Image to DOCX Converter - قراءة المزيد

يمكنك استكشاف المزيد حول Aspose.Words for Python باستخدام [التوثيق][6]. إذا كان لديك أي استفسارات ، فلا تتردد في إخبارنا عبر [المنتدى][7].

## استنتاج

في هذه المقالة ، تعلمت كيفية تحويل صورة إلى مستند Word في Python. أوضحنا أيضًا كيفية تحويل صور متعددة إلى مستند Word DOC / DOCX برمجيًا. يمكنك بسهولة دمج نماذج التعليمات البرمجية المتوفرة في التطبيق الخاص بك وتنفيذ الصورة لتحويل DOC أو DOCX.

## أنظر أيضا

* [قم بإنشاء ملفات PDF باستخدام C# - .NET PDF API](https://blog.aspose.com/ar/2020/12/02/create-pdf-files-using-csharp/)
* [تحويل Word إلى PDF في Python](https://blog.aspose.com/ar/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




