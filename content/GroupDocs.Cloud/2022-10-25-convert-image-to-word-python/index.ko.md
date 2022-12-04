---
title: "Python에서 이미지를 Word로 변환"
seoTitle: "Python에서 이미지를 Word로 변환 | Python PNG, JPG, BMP GIF를 Word로 | 어포즈"
description: "Python Word API를 사용하여 Python에서 이미지를 Word로 변환합니다. Python에서 단일 이미지 또는 여러 이미지를 Word로 변환합니다."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /ko/words/convert-image-to-word-python/
author: "우스만 아지즈"
summary: "경우에 따라 단일 이미지 또는 여러 이미지를 Word 문서로 변환해야 합니다. 이 작업을 프로그래밍 방식으로 수행하기 위해 이 문서에서는 Python에서 이미지를 Word DOC DOCX로 변환하는 방법을 보여줍니다."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Python에서 이미지를 Word로 변환">}}

MS Word [DOC][1] 및 [DOCX][9] 형식은 서식 있는 텍스트 문서를 만드는 데 널리 사용됩니다. 텍스트 서식을 지정하고 이미지와 같은 Word 문서에 다양한 요소를 삽입할 수 있습니다. 경우에 따라 단일 이미지 또는 여러 이미지를 Word 문서로 변환해야 합니다. 이 작업을 프로그래밍 방식으로 수행하기 위해 이 문서에서는 Python에서 이미지를 Word DOC DOCX로 변환하는 방법을 보여줍니다.

* [Python 이미지를 Word 변환기 라이브러리로](#Library-to-Convert-Image-to-Word)
* [Python에서 이미지를 Word DOC로 변환](#Convert-an-Image-to-Word)
* [Python에서 여러 이미지를 DOCX로 변환](#Convert-Multiple-Images-to-Word)

## Python 이미지를 Word 변환기 라이브러리로 - 무료 다운로드 {#Library-to-Convert-Image-to-Word}

이미지를 Word DOC/DOCX로 변환하려면 [Aspose.Words for Python][3]을 사용합니다. DOC, DOCX 등을 포함한 Word 문서 작업을 위한 기능이 풍부한 라이브러리입니다. 라이브러리에는 Word 문서의 앞뒤 변환을 위한 변환기가 내장되어 있습니다. 다음 pip 명령을 사용하여 [PyPI][4]에서 라이브러리를 설치할 수 있습니다.

```
> pip install aspose-words
```

## Python에서 이미지를 Word DOC로 변환 {#Convert-an-Image-to-Word}

다음은 Python에서 이미지를 Word DOC로 변환하는 단계입니다.

* 먼저 Document 클래스를 사용하여 새 문서를 만듭니다.
* 그런 다음 DocumentBuilder 개체를 만들고 Document 개체로 초기화합니다.
* DocumentBuilder.insert_image(fileName) 메서드를 사용하여 문서에 이미지를 삽입합니다.
* 마지막으로 Document.save(fileName) 메서드를 사용하여 Word 문서를 저장합니다.

다음 코드 샘플은 Python에서 PNG 이미지를 DOC로 변환하는 방법을 보여줍니다.

```
import aspose.words as aw

# 새 문서 만들기
doc = aw.Document()

# 문서 작성기 만들기
builder = aw.DocumentBuilder(doc)

# 문서에 이미지 삽입
builder.insert_image("logo.png")

# DOC로 저장
doc.save("image-to-word.doc")
```

## Python에서 여러 이미지를 Word로 변환 {#Convert-Multiple-Images-to-Word}

이전 섹션에서는 단일 이미지만 Word 문서로 변환했습니다. 그러나 어떤 경우에는 한 번에 둘 이상의 이미지를 변환해야 할 수도 있습니다. 다음은 Python에서 여러 이미지를 Word DOCX로 변환하는 단계입니다.

* 먼저 Document 클래스를 사용하여 새 문서를 만듭니다.
* 그런 다음 DocumentBuilder 개체를 만들고 Document 개체로 초기화합니다.
* 원하는 폴더에서 이미지 파일 목록을 가져옵니다.
* 이미지 파일 목록을 반복하고 DocumentBuilder.insert_image(fileName) 메서드를 사용하여 문서에 각 이미지를 삽입합니다.
* 마지막으로 Document.save(fileName) 메서드를 사용하여 Word 문서를 저장합니다.

다음 코드 샘플은 Python에서 여러 이미지를 Word DOCX로 변환하는 방법을 보여줍니다.

```
import aspose.words as aw
import os

# 이미지 디렉토리
dir = "D:\\images\\"

# 새 문서 만들기
doc = aw.Document()

# 문서 작성기 만들기
builder = aw.DocumentBuilder(doc)

# 폴더의 이미지 반복
for imageFile in os.listdir(dir):
    # 문서에 이미지 삽입
    builder.insert_image(os.path.join(dir, imageFile))

# DOCX로 저장
doc.save("images-to-word.docx")
```

## Image to DOC Python Converter - 무료 라이선스 받기 {#Get-a-Free-License}

[임시 무료 라이선스 받기][5]를 통해 평가 제한 없이 이미지를 Word 형식으로 변환할 수 있습니다.

## Python 이미지를 DOCX 변환기로 - 자세히 보기

[문서][6]를 사용하여 Python용 Aspose.Words에 대해 자세히 알아볼 수 있습니다. 질문이 있는 경우 [포럼][7]을 통해 언제든지 알려주십시오.

## 결론

이 기사에서는 Python에서 이미지를 Word 문서로 변환하는 방법을 배웠습니다. 또한 프로그래밍 방식으로 여러 이미지를 Word DOC/DOCX 문서로 변환하는 방법도 시연했습니다. 제공된 코드 샘플을 애플리케이션에 쉽게 통합하고 이미지를 DOC 또는 DOCX로 변환할 수 있습니다.

## 또한보십시오

* [C#을 사용하여 PDF 파일 생성 – .NET PDF API](https://blog.aspose.com/ko/2020/12/02/create-pdf-files-using-csharp/)
* [Python에서 Word를 PDF로 변환](https://blog.aspose.com/ko/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




