---
title: "在 Python 中将图像转换为 Word"
seoTitle: "在 Python 中将图像转换为 Word | Python PNG、JPG、BMP GIF 转 Word |假设"
description: "使用 Python Word API 将图像转换为 Python 中的 Word。在 Python 中将单个图像或多个图像转换为 Word。"
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /zh/words/convert-image-to-word-python/
author: "乌斯曼·阿齐兹"
summary: "在某些情况下，您必须将单个图像或一堆图像转换为 Word 文档。为了以编程方式执行此操作，本文展示了如何在 Python 中将图像转换为 Word DOC DOCX。"
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="在 Python 中将图像转换为 Word">}}

MS Word [DOC][1] 和 [DOCX][9] 格式被广泛用于创建富文本文档。您可以格式化文本并在 Word 文档中插入各种元素，例如图像。在某些情况下，您必须将单个图像或一堆图像转换为 Word 文档。为了以编程方式执行此操作，本文展示了如何在 Python 中将图像转换为 Word DOC DOCX。

* [Python 图像到 Word 转换器库](#Library-to-Convert-Image-to-Word)
* [在 Python 中将图像转换为 Word DOC](#Convert-an-Image-to-Word)
* [在 Python 中将多个图像转换为 DOCX](#Convert-Multiple-Images-to-Word)

## Python 图像到 Word 转换器库 - 免费下载 {#Library-to-Convert-Image-to-Word}

对于图像到 Word DOC/DOCX 的转换，我们将使用 [Aspose.Words for Python][3]。它是一个功能丰富的库，可处理包括 DOC、DOCX 等在内的 Word 文档。该库具有用于 Word 文档来回转换的内置转换器。您可以使用以下 pip 命令从 [PyPI][4] 安装库。

```
> pip install aspose-words
```

## 在 Python 中将图像转换为 Word DOC {#Convert-an-Image-to-Word}

以下是在 Python 中将图像转换为 Word DOC 的步骤。

* 首先，使用 Document 类创建一个新文档。
* 然后，创建一个 DocumentBuilder 对象并使用 Document 对象对其进行初始化。
* 使用 DocumentBuilder.insert_image(fileName) 方法将图像插入到文档中。
* 最后，使用 Document.save(fileName) 方法保存 Word 文档。

以下代码示例展示了如何在 Python 中将 PNG 图像转换为 DOC。

```
import aspose.words as aw

# 创建一个新文档
doc = aw.Document()

# 创建文档构建器
builder = aw.DocumentBuilder(doc)

# 将图像插入文档
builder.insert_image("logo.png")

# 另存为 DOC
doc.save("image-to-word.doc")
```

## 在 Python 中将多个图像转换为 Word {#Convert-Multiple-Images-to-Word}

在上一节中，我们仅将单个图像转换为 Word 文档。但是，在某些情况下，您可能需要一次转换多个图像。以下是在 Python 中将多个图像转换为 Word DOCX 的步骤。

* 首先，使用 Document 类创建一个新文档。
* 然后，创建一个 DocumentBuilder 对象并使用 Document 对象对其进行初始化。
* 从所需文件夹中获取图像文件列表。
* 遍历图像文件列表并使用 DocumentBuilder.insert_image(fileName) 方法将每个图像插入到文档中。
* 最后，使用 Document.save(fileName) 方法保存 Word 文档。

以下代码示例显示了在 Python 中将多个图像转换为 Word DOCX。

```
import aspose.words as aw
import os

# 图像目录
dir = "D:\\images\\"

# 创建一个新文档
doc = aw.Document()

# 创建文档构建器
builder = aw.DocumentBuilder(doc)

# 循环浏览文件夹中的图像
for imageFile in os.listdir(dir):
    # 将图像插入文档
    builder.insert_image(os.path.join(dir, imageFile))

# 另存为 DOCX
doc.save("images-to-word.docx")
```

## 图像到 DOC Python 转换器 - 获得免费许可证 {#Get-a-Free-License}

通过[获得免费临时许可证][5]，您可以将图像转换为 Word 格式而不受评估限制。

## Python 图像到 DOCX 转换器 - 阅读更多

您可以使用 [文档][6] 探索更多关于 Aspose.Words for Python 的信息。如果您有任何疑问，请随时通过我们的 [论坛][7] 告诉我们。

## 结论

在本文中，您学习了如何在 Python 中将图像转换为 Word 文档。我们还演示了如何以编程方式将多个图像转换为 Word DOC/DOCX 文档。您可以轻松地将提供的代码示例集成到您的应用程序中，并执行图像到 DOC 或 DOCX 的转换。

## 也可以看看

* [使用 C# 生成 PDF 文件 – .NET PDF API](https://blog.aspose.com/zh/2020/12/02/create-pdf-files-using-csharp/)
* [在 Python 中将 Word 转换为 PDF](https://blog.aspose.com/zh/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




