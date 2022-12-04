---
title: "Python で画像を Word に変換する"
seoTitle: "Python で画像を Word に変換 | Python PNG、JPG、BMP GIF から Word へ |アスポーズ"
description: "Python Word API を使用して、Python で画像を Word に変換します。 Python で単一の画像または複数の画像を Word に変換します。"
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /ja/words/convert-image-to-word-python/
author: "ウスマン・アジズ"
summary: "場合によっては、単一の画像または一連の画像を Word 文書に変換する必要があります。この操作をプログラムで実行するために、この記事では Python で画像を Word DOC DOCX に変換する方法を示します。"
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Python で画像を Word に変換する">}}

MS Word [DOC][1] および [DOCX][9] 形式は、リッチ テキスト ドキュメントの作成に広く使用されています。テキストの書式を設定したり、画像などの Word ドキュメントにさまざまな要素を挿入したりできます。場合によっては、単一の画像または一連の画像を Word 文書に変換する必要があります。この操作をプログラムで実行するために、この記事では Python で画像を Word DOC DOCX に変換する方法を示します。

* [Python 画像から Word へのコンバーター ライブラリ](#Library-to-Convert-Image-to-Word)
* [Python で画像を Word DOC に変換する](#Convert-an-Image-to-Word)
* [Python で複数の画像を DOCX に変換する](#Convert-Multiple-Images-to-Word)

## Python Image to Word Converter Library - 無料ダウンロード {#Library-to-Convert-Image-to-Word}

画像から Word DOC/DOCX への変換には、[Aspose.Words for Python][3] を使用します。 DOC、DOCX などの Word ドキュメントを操作するための機能豊富なライブラリです。このライブラリには、Word ドキュメントを相互に変換するためのコンバータが組み込まれています。次の pip コマンドを使用して、[PyPI][4] からライブラリをインストールできます。

```
> pip install aspose-words
```

## Python で画像を Word DOC に変換する {#Convert-an-Image-to-Word}

Python で画像を Word DOC に変換する手順は次のとおりです。

* まず、Document クラスを使用して新しいドキュメントを作成します。
* 次に、DocumentBuilder オブジェクトを作成し、Document オブジェクトで初期化します。
* DocumentBuilder.insert_image(fileName) メソッドを使用してドキュメントに画像を挿入します。
* 最後に、Document.save(fileName) メソッドを使用して Word 文書を保存します。

次のコード サンプルは、Python で PNG 画像を DOC に変換する方法を示しています。

```
import aspose.words as aw

# 新しいドキュメントを作成する
doc = aw.Document()

# ドキュメント ビルダーを作成する
builder = aw.DocumentBuilder(doc)

# ドキュメントに画像を挿入する
builder.insert_image("logo.png")

# DOCとして保存
doc.save("image-to-word.doc")
```

## Python で複数の画像を Word に変換する {#Convert-Multiple-Images-to-Word}

前のセクションでは、単一の画像のみを Word ドキュメントに変換しました。ただし、場合によっては、一度に複数の画像を変換する必要がある場合があります。 Python で複数の画像を Word DOCX に変換する手順は次のとおりです。

* まず、Document クラスを使用して新しいドキュメントを作成します。
* 次に、DocumentBuilder オブジェクトを作成し、Document オブジェクトで初期化します。
* 目的のフォルダーから画像ファイルのリストを取得します。
* 画像ファイルのリストをループし、DocumentBuilder.insert_image(fileName) メソッドを使用して各画像をドキュメントに挿入します。
* 最後に、Document.save(fileName) メソッドを使用して Word 文書を保存します。

次のコード サンプルは、Python で複数の画像を Word DOCX に変換する方法を示しています。

```
import aspose.words as aw
import os

# 画像ディレクトリ
dir = "D:\\images\\"

# 新しいドキュメントを作成する
doc = aw.Document()

# ドキュメント ビルダーを作成する
builder = aw.DocumentBuilder(doc)

# フォルダ内の画像をループ
for imageFile in os.listdir(dir):
    # ドキュメントに画像を挿入する
    builder.insert_image(os.path.join(dir, imageFile))

# DOCX として保存
doc.save("images-to-word.docx")
```

## Image to DOC Python Converter - 無料ライセンスを取得 {#Get-a-Free-License}

[無料の一時ライセンスを取得][5]することで、評価制限なしで画像を Word 形式に変換できます。

## Python 画像から DOCX へのコンバーター - 続きを読む

[ドキュメンテーション][6] を使用して、Aspose.Words for Python の詳細を調べることができます。ご不明な点がございましたら、[フォーラム][7] からお気軽にお問い合わせください。

## 結論

この記事では、Python で画像を Word ドキュメントに変換する方法を学習しました。また、複数の画像をプログラムで Word DOC/DOCX ドキュメントに変換する方法も示しました。提供されているコード サンプルをアプリケーションに簡単に統合し、画像から DOC または DOCX への変換を実行できます。

## 関連項目

* [C# を使用して PDF ファイルを生成 – .NET PDF API](https://blog.aspose.com/ja/2020/12/02/create-pdf-files-using-csharp/)
* [Python で Word を PDF に変換する](https://blog.aspose.com/ja/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




