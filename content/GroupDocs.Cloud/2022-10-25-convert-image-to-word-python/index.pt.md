---
title: "Converter imagem para Word em Python"
seoTitle: "Converter imagem para palavra em Python | Python PNG, JPG, GIF BMP para Word | Aspor"
description: "Use a API do Python Word para converter imagens para o Word em Python. Converta uma única imagem ou várias imagens para um Word em Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /pt/words/convert-image-to-word-python/
author: "Usman Aziz"
summary: "Em certos casos, você precisa converter uma única imagem ou várias imagens em um documento do Word. Para executar essa operação programaticamente, este artigo mostra como converter imagens em Word DOC DOCX em Python."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Converter imagem para Word em Python">}}

Os formatos MS Word [DOC][1] e [DOCX][9] são amplamente usados para criar documentos rich text. Você pode formatar texto e inserir vários elementos em documentos do Word, como imagens. Em certos casos, você precisa converter uma única imagem ou várias imagens em um documento do Word. Para executar essa operação programaticamente, este artigo mostra como converter imagens em Word DOC DOCX em Python.

* [Biblioteca de conversores de imagem para Word do Python](#Library-to-Convert-Image-to-Word)
* [Converter uma imagem para Word DOC em Python](#Convert-an-Image-to-Word)
* [Converter várias imagens para DOCX em Python](#Convert-Multiple-Images-to-Word)

## Biblioteca Python Image to Word Converter - Download Gratuito {#Library-to-Convert-Image-to-Word}

Para a conversão de imagem para Word DOC/DOCX, usaremos [Aspose.Words for Python][3]. É uma biblioteca rica em recursos para trabalhar com documentos do Word, incluindo DOC, DOCX, etc. A biblioteca possui um conversor embutido para conversão de documentos do Word. Você pode instalar a biblioteca de [PyPI][4] usando o seguinte comando pip.

```
> pip install aspose-words
```

## Converter uma imagem para Word DOC em Python {#Convert-an-Image-to-Word}

A seguir estão as etapas para converter uma imagem em um Word DOC em Python.

* Primeiro, crie um novo documento usando a classe Document.
* Em seguida, crie um objeto DocumentBuilder e inicialize-o com o objeto Document.
* Insira a imagem no documento usando o método DocumentBuilder.insert_image(fileName).
* Finalmente, salve o documento do Word usando o método Document.save(fileName).

O exemplo de código a seguir mostra como converter uma imagem PNG em DOC em Python.

```
import aspose.words as aw

# Criar um novo documento
doc = aw.Document()

# Criar um construtor de documentos
builder = aw.DocumentBuilder(doc)

# Inserir imagem no documento
builder.insert_image("logo.png")

# Salvar como DOC
doc.save("image-to-word.doc")
```

## Converter várias imagens para o Word em Python {#Convert-Multiple-Images-to-Word}

Na seção anterior, convertemos apenas uma única imagem em documento do Word. No entanto, em certos casos, pode ser necessário converter mais de uma imagem de uma só vez. A seguir estão as etapas para converter várias imagens em um Word DOCX em Python.

* Primeiro, crie um novo documento usando a classe Document.
* Em seguida, crie um objeto DocumentBuilder e inicialize-o com o objeto Document.
* Obtenha a lista dos arquivos de imagem da pasta desejada.
* Percorra a lista de arquivos de imagem e insira cada imagem no documento usando o método DocumentBuilder.insert_image(fileName).
* Finalmente, salve o documento do Word usando o método Document.save(fileName).

O exemplo de código a seguir mostra a conversão de várias imagens em um Word DOCX em Python.

```
import aspose.words as aw
import os

# Diretório de imagens
dir = "D:\\images\\"

# Criar um novo documento
doc = aw.Document()

# Criar um construtor de documentos
builder = aw.DocumentBuilder(doc)

# Faça um loop pelas imagens na pasta
for imageFile in os.listdir(dir):
    # Inserir imagem no documento
    builder.insert_image(os.path.join(dir, imageFile))

# Salvar como DOCX
doc.save("images-to-word.docx")
```

## Conversor de imagem para DOC Python - Obtenha uma licença gratuita {#Get-a-Free-License}

Você pode converter imagens para formatos Word sem limitações de avaliação [obtendo uma licença temporária gratuita][5].

## Conversor de imagem Python para DOCX - Leia mais

Você pode explorar mais sobre o Aspose.Words for Python usando [documentação][6]. Caso você tenha alguma dúvida, sinta-se à vontade para nos informar através do nosso [fórum][7].

## Conclusão

Neste artigo, você aprendeu como converter uma imagem em um documento do Word em Python. Também demonstramos como converter várias imagens em um documento Word DOC/DOCX programaticamente. Você pode integrar facilmente os exemplos de código fornecidos em seu aplicativo e realizar a conversão da imagem para DOC ou DOCX.

## Veja também

* [Gerar arquivos PDF usando C# – .NET PDF API](https://blog.aspose.com/pt/2020/12/02/create-pdf-files-using-csharp/)
* [Converter Word para PDF em Python](https://blog.aspose.com/pt/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




