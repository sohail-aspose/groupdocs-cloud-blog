---
title: "Chuyển đổi hình ảnh sang Word trong Python"
seoTitle: "Chuyển đổi hình ảnh sang Word trong Python | Python PNG, JPG, BMP GIF sang Word | Aspose"
description: "Sử dụng Python Word API để chuyển đổi hình ảnh sang Word bằng Python. Chuyển đổi một hình ảnh hoặc nhiều hình ảnh sang Word bằng Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /vi/words/convert-image-to-word-python/
author: "Usman Aziz"
summary: "Trong một số trường hợp nhất định, bạn phải chuyển đổi một hình ảnh hoặc một loạt hình ảnh sang tài liệu Word. Để thực hiện thao tác này theo chương trình, bài viết này hướng dẫn cách chuyển đổi hình ảnh sang Word DOC DOCX bằng Python."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Chuyển đổi hình ảnh sang Word trong Python">}}

Định dạng MS Word [DOC][1] và [DOCX][9] được sử dụng rộng rãi để tạo tài liệu văn bản đa dạng thức. Bạn có thể định dạng văn bản và chèn các phần tử khác nhau trong tài liệu Word, chẳng hạn như hình ảnh. Trong một số trường hợp nhất định, bạn phải chuyển đổi một hình ảnh hoặc một loạt hình ảnh sang tài liệu Word. Để thực hiện thao tác này theo chương trình, bài viết này hướng dẫn cách chuyển đổi hình ảnh sang Word DOC DOCX bằng Python.

* [Thư viện chuyển đổi hình ảnh sang Word trong Python](#Library-to-Convert-Image-to-Word)
* [Chuyển đổi hình ảnh sang Word DOC bằng Python](#Convert-an-Image-to-Word)
* [Chuyển đổi nhiều hình ảnh sang DOCX bằng Python](#Convert-Multiple-Images-to-Word)

## Thư viện chuyển đổi hình ảnh sang Word trong Python - Tải xuống miễn phí {#Library-to-Convert-Image-to-Word}

Để chuyển đổi hình ảnh sang Word DOC / DOCX, chúng tôi sẽ sử dụng [Aspose.Words dành cho Python][3]. Đây là một thư viện giàu tính năng để làm việc với các tài liệu Word bao gồm DOC, DOCX, v.v. Thư viện có bộ chuyển đổi tích hợp để chuyển đổi qua lại các tài liệu Word. Bạn có thể cài đặt thư viện từ [PyPI][4] bằng lệnh pip sau.

```
> pip install aspose-words
```

## Chuyển đổi hình ảnh sang Word DOC bằng Python {#Convert-an-Image-to-Word}

Sau đây là các bước để chuyển đổi hình ảnh sang Word DOC bằng Python.

* Đầu tiên, tạo một tài liệu mới bằng cách sử dụng lớp Tài liệu.
* Sau đó, tạo một đối tượng DocumentBuilder và khởi tạo nó bằng đối tượng Document.
* Chèn hình ảnh vào tài liệu bằng phương pháp DocumentBuilder.insertimage (fileName).
* Cuối cùng, lưu tài liệu Word bằng phương pháp Document.save (fileName).

Mẫu mã sau đây cho thấy cách chuyển đổi hình ảnh PNG sang DOC trong Python.

```
import aspose.words as aw

# Tạo một tài liệu mới
doc = aw.Document()

# Tạo một trình xây dựng tài liệu
builder = aw.DocumentBuilder(doc)

# Chèn hình ảnh vào tài liệu
builder.insert_image("logo.png")

# Lưu dưới dạng DOC
doc.save("image-to-word.doc")
```

## Chuyển đổi nhiều hình ảnh sang Word bằng Python {#Convert-Multiple-Images-to-Word}

Trong phần trước, chúng tôi chỉ chuyển đổi một hình ảnh duy nhất sang tài liệu Word. Tuy nhiên, trong một số trường hợp nhất định, bạn có thể cần chuyển đổi nhiều hình ảnh cùng một lúc. Sau đây là các bước để chuyển đổi nhiều hình ảnh sang Word DOCX bằng Python.

* Đầu tiên, tạo một tài liệu mới bằng cách sử dụng lớp Tài liệu.
* Sau đó, tạo một đối tượng DocumentBuilder và khởi tạo nó bằng đối tượng Document.
* Nhận danh sách các tệp hình ảnh từ thư mục mong muốn.
* Lặp qua danh sách các tệp hình ảnh và chèn từng hình ảnh vào tài liệu bằng phương pháp DocumentBuilder.insertimage (fileName).
* Cuối cùng, lưu tài liệu Word bằng phương pháp Document.save (fileName).

Mẫu mã sau đây cho thấy việc chuyển đổi nhiều hình ảnh sang Word DOCX bằng Python.

```
import aspose.words as aw
import os

# Thư mục hình ảnh
dir = "D:\\images\\"

# Tạo một tài liệu mới
doc = aw.Document()

# Tạo một trình xây dựng tài liệu
builder = aw.DocumentBuilder(doc)

# Lặp qua các hình ảnh trong thư mục
for imageFile in os.listdir(dir):
    # Chèn hình ảnh vào tài liệu
    builder.insert_image(os.path.join(dir, imageFile))

# Lưu dưới dạng DOCX
doc.save("images-to-word.docx")
```

## Chuyển đổi hình ảnh sang DOC Python - Nhận giấy phép miễn phí {#Get-a-Free-License}

Bạn có thể chuyển đổi hình ảnh sang định dạng Word mà không bị giới hạn đánh giá bằng cách [nhận giấy phép tạm thời miễn phí][5].

## Python Image to DOCX Converter - Đọc thêm

Bạn có thể khám phá thêm về Aspose. AdWords for Python bằng [tài liệu][6]. Trong trường hợp bạn có bất kỳ thắc mắc nào, vui lòng cho chúng tôi biết qua [diễn đàn][7] của chúng tôi.

## Sự kết luận

Trong bài viết này, bạn đã học cách chuyển đổi hình ảnh sang tài liệu Word bằng Python. Chúng tôi cũng đã trình bày cách chuyển đổi nhiều hình ảnh sang tài liệu Word DOC / DOCX theo lập trình. Bạn có thể dễ dàng tích hợp các mẫu mã được cung cấp vào ứng dụng của mình và thực hiện chuyển đổi hình ảnh sang DOC hoặc DOCX.

## Xem thêm

* [Tạo tệp PDF bằng C# - .NET PDF API](https://blog.aspose.com/vi/pdf/create-pdf-files-using-csharp/)
* [Chuyển Word sang PDF bằng Python](https://blog.aspose.com/vi/words/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




