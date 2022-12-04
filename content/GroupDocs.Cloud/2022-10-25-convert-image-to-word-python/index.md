---
title: "Convert Image to Word in Python"
seoTitle: "Convert Image to Word in Python | Python PNG, JPG, BMP GIF to Word | Aspose"
description: "Use Python Word API to convert images to Word in Python. Convert a single image or multiple images to a Word in Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /words/convert-image-to-word-python/
author: Usman Aziz
summary: "In certain cases, you have to convert a single image or a bunch of images to a Word document. To perform this operation programmatically, this article shows **how to convert images to Word DOC DOCX in Python**."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Convert Image to Word in Python">}}

MS Word [DOC][1] and [DOCX][9] formats are widely used to create rich text documents. You can format text and insert various elements in Word documents such as images. In certain cases, you have to convert a single image or a bunch of images to a Word document. To perform this operation programmatically, this article shows **how to convert images to Word DOC DOCX in Python**.

*   [Python Image to Word Converter Library](#Library-to-Convert-Image-to-Word)
*   [Convert an Image to Word DOC in Python](#Convert-an-Image-to-Word)
*   [Convert Multiple Images to DOCX in Python](#Convert-Multiple-Images-to-Word)

## Python Image to Word Converter Library - Free Download {#Library-to-Convert-Image-to-Word}

For the image to Word DOC/DOCX conversion, we will use [Aspose.Words for Python][3]. It is a feature-rich library to work with Word documents including DOC, DOCX, etc. The library has a built-in converter for back-and-forth conversion of Word documents. You can install the library from [PyPI][4] using the following pip command.

```
> pip install aspose-words
```

## Convert an Image to Word DOC in Python {#Convert-an-Image-to-Word}

The following are the steps to convert an image to a Word DOC in Python.

*   First, create a new document using the **Document** class.
*   Then, create a **DocumentBuilder** object and initialize it with the **Document** object.
*   Insert image into the document using **DocumentBuilder.insert_image(fileName)** method.
*   Finally, save the Word document using **Document.save(fileName)** method.

The following code sample shows how to convert a PNG image to DOC in Python.

{{< gist aspose-com-gists 1cfe01153e120d3eca4adb73060626bc "convert-image-to-word.py" >}}

## Convert Multiple Images to Word in Python {#Convert-Multiple-Images-to-Word}

In the previous section, we converted only a single image to Word document. However, in certain cases, you may need to convert more than one image at once. The following are the steps to convert multiple images to a Word DOCX in Python.

*   First, create a new document using the **Document** class.
*   Then, create a **DocumentBuilder** object and initialize it with the **Document** object.
*   Get the list of the image files from the desired folder.
*   Loop through the list of the image files and insert each image into the document using **DocumentBuilder.insert_image(fileName)** method.
*   Finally, save the Word document using **Document.save(fileName)** method.

The following code sample shows the conversion of multiple images to a Word DOCX in Python.

{{< gist aspose-com-gists 1cfe01153e120d3eca4adb73060626bc "convert-multiple-images-to-word.py" >}}

## Image to DOC Python Converter - Get a Free License {#Get-a-Free-License}

You can convert images to Word formats without evaluation limitations by [getting a free temporary license][5].

## Python Image to DOCX Converter - Read More

You can explore more about Aspose.Words for Python using [documentation][6]. In case you would have any queries, feel free to let us know via our [forum][7].

## Conclusion

In this article, you have learned how to convert an image to a Word document in Python. We also demonstrated how to convert multiple images to a Word DOC/DOCX document programmatically. You can easily integrate the provided code samples into your application and perform the image to DOC or DOCX conversion. 

## See Also

*   [Generate PDF Files using C# – .NET PDF API](https://blog.aspose.com/pdf/create-pdf-files-using-csharp/)
*   [Convert Word to PDF in Python](https://blog.aspose.com/words/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/



