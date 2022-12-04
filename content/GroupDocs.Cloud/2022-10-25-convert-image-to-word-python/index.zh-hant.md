---
title: "在 Python 中將圖像轉換為 Word"
seoTitle: "在 Python 中將圖像轉換為 Word | Python PNG、JPG、BMP GIF 到 Word | Aspose"
description: "使用 Python Word API 在 Python 中將圖像轉換為 Word。在 Python 中將單個圖像或多個圖像轉換為 Word。"
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /zh-hant/words/convert-image-to-word-python/
author: "烏斯曼阿茲"
summary: "在某些情況下，您必須將單個圖像或一堆圖像轉換為 Word 文檔。為了以編程方式執行此操作，本文介紹瞭如何在 Python 中將圖像轉換為 Word DOC DOCX。"
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="在 Python 中將圖像轉換為 Word">}}

MS Word [DOC][1] 和 [DOCX][9] 格式廣泛用於創建富文本文檔。您可以設置文本格式並在 Word 文檔中插入各種元素，例如圖像。在某些情況下，您必須將單個圖像或一堆圖像轉換為 Word 文檔。為了以編程方式執行此操作，本文介紹瞭如何在 Python 中將圖像轉換為 Word DOC DOCX。

* [Python 圖像到 Word 轉換器庫](#Library-to-Convert-Image-to-Word)
* [在 Python 中將圖像轉換為 Word DOC](#Convert-an-Image-to-Word)
* [在 Python 中將多個圖像轉換為 DOCX](#Convert-Multiple-Images-to-Word)

## Python 圖像到 Word 轉換器庫 - 免費下載 {#Library-to-Convert-Image-to-Word}

對於圖像到 Word DOC/DOCX 的轉換，我們將使用 [Aspose.Words for Python][3]。它是一個功能豐富的庫，可以處理 Word 文檔，包括 DOC、DOCX 等。該庫有一個內置的轉換器，用於 Word 文檔的來迴轉換。您可以使用以下 pip 命令從 [PyPI][4] 安裝庫。

```
> pip install aspose-words
```

## 在 Python 中將圖像轉換為 Word DOC {#Convert-an-Image-to-Word}

以下是在 Python 中將圖像轉換為 Word DOC 的步驟。

* 首先，使用 Document 類創建一個新文檔。
* 然後，創建一個 DocumentBuilder 對象並使用 Document 對像對其進行初始化。
* 使用 DocumentBuilder.insertimage(fileName) 方法將圖像插入到文檔中。
* 最後，使用 Document.save(fileName) 方法保存 Word 文檔。

以下代碼示例顯示瞭如何在 Python 中將 PNG 圖像轉換為 DOC。

```
import aspose.words as aw

# 創建一個新文檔
doc = aw.Document()

# 創建文檔生成器
builder = aw.DocumentBuilder(doc)

# 在文檔中插入圖像
builder.insert_image("logo.png")

# 另存為文檔
doc.save("image-to-word.doc")
```

## 在 Python 中將多個圖像轉換為 Word {#Convert-Multiple-Images-to-Word}

在上一節中，我們只將單個圖像轉換為 Word 文檔。但是，在某些情況下，您可能需要一次轉換多個圖像。以下是在 Python 中將多個圖像轉換為 Word DOCX 的步驟。

* 首先，使用 Document 類創建一個新文檔。
* 然後，創建一個 DocumentBuilder 對象並使用 Document 對像對其進行初始化。
* 從所需文件夾中獲取圖像文件列表。
* 遍歷圖像文件列表並使用 DocumentBuilder.insertimage(fileName) 方法將每個圖像插入到文檔中。
* 最後，使用 Document.save(fileName) 方法保存 Word 文檔。

以下代碼示例顯示了在 Python 中將多個圖像轉換為 Word DOCX。

```
import aspose.words as aw
import os

# 圖片目錄
dir = "D:\\images\\"

# 創建一個新文檔
doc = aw.Document()

# 創建文檔生成器
builder = aw.DocumentBuilder(doc)

# 循環瀏覽文件夾中的圖像
for imageFile in os.listdir(dir):
    # 在文檔中插入圖像
    builder.insert_image(os.path.join(dir, imageFile))

# 另存為 DOCX
doc.save("images-to-word.docx")
```

## 圖像到 DOC Python 轉換器 - 獲得免費許可證 {#Get-a-Free-License}

您可以通過 [獲得免費的臨時許可證][5] 將圖像轉換為 Word 格式而不受評估限制。

## Python 圖像到 DOCX 轉換器 - 閱讀更多

您可以使用 [文檔][6] 探索更多關於 Aspose.Words for Python 的信息。如果您有任何疑問，請隨時通過我們的 [論壇][7] 告訴我們。

## 結論

在本文中，您學習瞭如何使用 Python 將圖像轉換為 Word 文檔。我們還演示瞭如何以編程方式將多個圖像轉換為 Word DOC/DOCX 文檔。您可以輕鬆地將提供的代碼示例集成到您的應用程序中，並執行圖像到 DOC 或 DOCX 的轉換。

## 也可以看看

* [使用 C# – .NET PDF API 生成 PDF 文件](https://blog.aspose.com/zh-hant/pdf/create-pdf-files-using-csharp/)
* [在 Python 中將 Word 轉換為 PDF](https://blog.aspose.com/zh-hant/words/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




