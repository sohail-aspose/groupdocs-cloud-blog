---
title: "แปลงรูปภาพเป็น Word ใน Python"
seoTitle: "แปลงรูปภาพเป็น Word ใน Python | Python PNG, JPG, BMP GIF เป็น Word | ตั้งสติ"
description: "ใช้ Python Word API เพื่อแปลงรูปภาพเป็น Word ใน Python แปลงภาพเดียวหรือหลายภาพเป็น Word ใน Python"
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /th/words/convert-image-to-word-python/
author: "อุสมาน อาซิซ"
summary: "ในบางกรณี คุณต้องแปลงรูปภาพเดียวหรือหลายรูปภาพเป็นเอกสาร Word ในการดำเนินการนี้โดยทางโปรแกรม บทความนี้แสดงวิธีการแปลงรูปภาพเป็น Word DOC DOCX ใน Python"
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="แปลงรูปภาพเป็น Word ใน Python">}}

รูปแบบ MS Word [DOC][1] และ [DOCX][9] ใช้กันอย่างแพร่หลายในการสร้างเอกสารข้อความที่มีรูปแบบ คุณสามารถจัดรูปแบบข้อความและแทรกองค์ประกอบต่างๆ ในเอกสาร Word เช่น รูปภาพ ในบางกรณี คุณต้องแปลงรูปภาพเดียวหรือหลายรูปภาพเป็นเอกสาร Word ในการดำเนินการนี้โดยทางโปรแกรม บทความนี้แสดงวิธีการแปลงรูปภาพเป็น Word DOC DOCX ใน Python

* [ไลบรารี Python Image เป็น Word Converter](#Library-to-Convert-Image-to-Word)
* [แปลงรูปภาพเป็น Word DOC ใน Python](#Convert-an-Image-to-Word)
* [แปลงหลายภาพเป็น DOCX ใน Python](#Convert-Multiple-Images-to-Word)

## Python Image to Word Converter Library - ดาวน์โหลดฟรี {#Library-to-Convert-Image-to-Word}

สำหรับการแปลงรูปภาพเป็น Word DOC/DOCX เราจะใช้ [Aspose.Words for Python][3] เป็นไลบรารีที่มีคุณลักษณะหลากหลายสำหรับการทำงานกับเอกสาร Word รวมถึง DOC, DOCX เป็นต้น ไลบรารีมีตัวแปลงในตัวสำหรับการแปลงเอกสาร Word แบบกลับไปกลับมา คุณสามารถติดตั้งไลบรารีได้จาก [PyPI][4] โดยใช้คำสั่ง pip ต่อไปนี้

```
> pip install aspose-words
```

## แปลงรูปภาพเป็น Word DOC ใน Python {#Convert-an-Image-to-Word}

ต่อไปนี้เป็นขั้นตอนในการแปลงรูปภาพเป็น Word DOC ใน Python

* ขั้นแรก สร้างเอกสารใหม่โดยใช้คลาส Document
* จากนั้น สร้างวัตถุ DocumentBuilder และเริ่มต้นด้วยวัตถุเอกสาร
* แทรกรูปภาพลงในเอกสารโดยใช้เมธอด DocumentBuilder.insertimage(fileName)
* สุดท้าย บันทึกเอกสาร Word โดยใช้วิธี Document.save(fileName)

ตัวอย่างโค้ดต่อไปนี้แสดงวิธีการแปลงรูปภาพ PNG เป็น DOC ใน Python

```
import aspose.words as aw

# สร้างเอกสารใหม่
doc = aw.Document()

# สร้างตัวสร้างเอกสาร
builder = aw.DocumentBuilder(doc)

# แทรกรูปภาพลงในเอกสาร
builder.insert_image("logo.png")

# บันทึกเป็น DOC
doc.save("image-to-word.doc")
```

## แปลงหลายรูปภาพเป็น Word ใน Python {#Convert-Multiple-Images-to-Word}

ในส่วนก่อนหน้านี้ เราแปลงเพียงภาพเดียวเป็นเอกสาร Word อย่างไรก็ตาม ในบางกรณี คุณอาจต้องแปลงรูปภาพมากกว่าหนึ่งภาพพร้อมกัน ต่อไปนี้เป็นขั้นตอนในการแปลงรูปภาพหลายรูปเป็น Word DOCX ใน Python

* ขั้นแรก สร้างเอกสารใหม่โดยใช้คลาส Document
* จากนั้น สร้างวัตถุ DocumentBuilder และเริ่มต้นด้วยวัตถุเอกสาร
* รับรายการไฟล์รูปภาพจากโฟลเดอร์ที่ต้องการ
* วนซ้ำรายการไฟล์ภาพและแทรกแต่ละภาพลงในเอกสารโดยใช้เมธอด DocumentBuilder.insertimage(fileName)
* สุดท้าย บันทึกเอกสาร Word โดยใช้วิธี Document.save(fileName)

ตัวอย่างโค้ดต่อไปนี้แสดงการแปลงรูปภาพหลายรูปเป็น Word DOCX ใน Python

```
import aspose.words as aw
import os

# ไดเรกทอรีรูปภาพ
dir = "D:\\images\\"

# สร้างเอกสารใหม่
doc = aw.Document()

# สร้างตัวสร้างเอกสาร
builder = aw.DocumentBuilder(doc)

# วนซ้ำรูปภาพในโฟลเดอร์
for imageFile in os.listdir(dir):
    # แทรกรูปภาพลงในเอกสาร
    builder.insert_image(os.path.join(dir, imageFile))

# บันทึกเป็น DOCX
doc.save("images-to-word.docx")
```

## Image to DOC Python Converter - รับใบอนุญาตฟรี {#Get-a-Free-License}

คุณสามารถแปลงรูปภาพเป็นรูปแบบ Word ได้โดยไม่มีข้อจำกัดในการประเมินโดย [รับใบอนุญาตชั่วคราวฟรี][5]

## Python Image เป็น DOCX Converter - อ่านเพิ่มเติม

คุณสามารถสำรวจเพิ่มเติมเกี่ยวกับ Aspose.Words for Python โดยใช้ [เอกสารประกอบ][6] ในกรณีที่คุณมีข้อสงสัย โปรดแจ้งให้เราทราบผ่านทาง [ฟอรัม][7] ของเรา

## บทสรุป

ในบทความนี้ คุณได้เรียนรู้วิธีแปลงรูปภาพเป็นเอกสาร Word ใน Python เรายังสาธิตวิธีแปลงรูปภาพหลายรูปเป็นเอกสาร Word DOC/DOCX โดยทางโปรแกรม คุณสามารถรวมตัวอย่างโค้ดที่ให้ไว้ในแอปพลิเคชันของคุณได้อย่างง่ายดาย และดำเนินการแปลงอิมเมจเป็น DOC หรือ DOCX

## ดูสิ่งนี้ด้วย

* [สร้างไฟล์ PDF โดยใช้ C# – .NET PDF API](https://blog.aspose.com/th/pdf/create-pdf-files-using-csharp/)
* [แปลง Word เป็น PDF ใน Python](https://blog.aspose.com/th/words/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




