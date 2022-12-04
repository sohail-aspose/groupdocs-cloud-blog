---
title: "تبدیل تصویر به ورد در پایتون"
seoTitle: "تبدیل تصویر به ورد در پایتون | Python PNG، JPG، BMP GIF به Word | در نظر بگیرید"
description: "از Python Word API برای تبدیل تصاویر به Word در پایتون استفاده کنید. یک تصویر یا چند تصویر را در پایتون به یک Word تبدیل کنید."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /fa/words/convert-image-to-word-python/
author: "عثمان عزیز"
summary: "در موارد خاص، شما باید یک تصویر یا یک دسته از تصاویر را به یک سند Word تبدیل کنید. برای انجام این عملیات به صورت برنامه ای، این مقاله نحوه تبدیل تصاویر به Word DOC DOCX در پایتون را نشان می دهد."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="تبدیل تصویر به ورد در پایتون">}}

فرمت‌های MS Word [DOC][1] و [DOCX][9] به طور گسترده برای ایجاد اسناد متنی غنی استفاده می‌شوند. می توانید متن را قالب بندی کنید و عناصر مختلفی را در اسناد Word مانند تصاویر درج کنید. در موارد خاص، شما باید یک تصویر یا یک دسته از تصاویر را به یک سند Word تبدیل کنید. برای انجام این عملیات به صورت برنامه ای، این مقاله نحوه تبدیل تصاویر به Word DOC DOCX در پایتون را نشان می دهد.

* [کتابخانه مبدل تصویر به ورد پایتون](#Library-to-Convert-Image-to-Word)
* [تبدیل تصویر به Word DOC در پایتون](#Convert-an-Image-to-Word)
* [تبدیل چندین تصویر به DOCX در پایتون](#Convert-Multiple-Images-to-Word)

## کتابخانه تبدیل تصویر به ورد پایتون - دانلود رایگان {#Library-to-Convert-Image-to-Word}

برای تبدیل تصویر به Word DOC/DOCX، از [Aspose.Words برای Python][3] استفاده خواهیم کرد. این یک کتابخانه غنی از ویژگی ها برای کار با اسناد Word از جمله DOC، DOCX و غیره است. این کتابخانه دارای یک مبدل داخلی برای تبدیل پشت و رو اسناد Word است. با استفاده از دستور pip زیر می توانید کتابخانه را از [PyPI][4] نصب کنید.

```
> pip install aspose-words
```

## تبدیل تصویر به Word DOC در پایتون {#Convert-an-Image-to-Word}

در زیر مراحل تبدیل یک تصویر به Word DOC در پایتون آمده است.

* ابتدا با استفاده از کلاس Document یک سند جدید ایجاد کنید.
* سپس یک شی DocumentBuilder ایجاد کنید و آن را با شی Document مقداردهی اولیه کنید.
* با استفاده از روش DocumentBuilder.insertimage(fileName) تصویر را در سند وارد کنید.
* در نهایت سند Word را با استفاده از روش Document.save(fileName) ذخیره کنید.

نمونه کد زیر نحوه تبدیل یک تصویر PNG به DOC در پایتون را نشان می دهد.

```
import aspose.words as aw

# یک سند جدید ایجاد کنید
doc = aw.Document()

# یک سند ساز ایجاد کنید
builder = aw.DocumentBuilder(doc)

# درج تصویر در سند
builder.insert_image("logo.png")

# ذخیره به عنوان DOC
doc.save("image-to-word.doc")
```

## تبدیل چندین تصویر به ورد در پایتون {#Convert-Multiple-Images-to-Word}

در بخش قبل، تنها یک تصویر را به سند Word تبدیل کردیم. با این حال، در موارد خاص، ممکن است نیاز داشته باشید که بیش از یک تصویر را همزمان تبدیل کنید. در زیر مراحل تبدیل چندین تصویر به Word DOCX در پایتون آمده است.

* ابتدا با استفاده از کلاس Document یک سند جدید ایجاد کنید.
* سپس یک شی DocumentBuilder ایجاد کنید و آن را با شی Document مقداردهی اولیه کنید.
* لیست فایل های تصویری را از پوشه مورد نظر دریافت کنید.
* لیست فایل های تصویر را حلقه بزنید و هر تصویر را با استفاده از روش DocumentBuilder.insertimage(fileName) در سند وارد کنید.
* در نهایت سند Word را با استفاده از روش Document.save(fileName) ذخیره کنید.

نمونه کد زیر تبدیل چندین تصویر به Word DOCX در پایتون را نشان می دهد.

```
import aspose.words as aw
import os

# دایرکتوری تصویر
dir = "D:\\images\\"

# یک سند جدید ایجاد کنید
doc = aw.Document()

# یک سند ساز ایجاد کنید
builder = aw.DocumentBuilder(doc)

# حلقه بین تصاویر در پوشه
for imageFile in os.listdir(dir):
    # درج تصویر در سند
    builder.insert_image(os.path.join(dir, imageFile))

# ذخیره به عنوان DOCX
doc.save("images-to-word.docx")
```

## تبدیل تصویر به DOC پایتون - مجوز رایگان دریافت کنید {#Get-a-Free-License}

با [دریافت مجوز موقت رایگان] می توانید تصاویر را بدون محدودیت ارزیابی به فرمت های Word تبدیل کنید.

## تبدیل تصویر پایتون به DOCX - بیشتر بخوانید

می توانید با استفاده از [documentation][6] درباره Aspose.Words برای پایتون بیشتر کاوش کنید. اگر سؤالی دارید، از طریق [تالار گفتمان][7] ما را در جریان بگذارید.

## نتیجه

در این مقاله نحوه تبدیل تصویر به سند ورد در پایتون را یاد گرفتید. ما همچنین نحوه تبدیل چندین تصویر به یک سند Word DOC/DOCX را به صورت برنامه‌ریزی نشان دادیم. می توانید به راحتی نمونه کدهای ارائه شده را در برنامه خود ادغام کنید و تصویر را به DOC یا DOCX تبدیل کنید.

## همچنین ببینید

* [با استفاده از C# – .NET PDF API فایل های PDF تولید کنید](https://blog.aspose.com/fa/pdf/create-pdf-files-using-csharp/)
* [تبدیل Word به PDF در پایتون](https://blog.aspose.com/fa/words/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




