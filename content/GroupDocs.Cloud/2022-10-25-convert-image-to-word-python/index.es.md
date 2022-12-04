---
title: "Convertir imagen a Word en Python"
seoTitle: "Convertir imagen a Word en Python | Python PNG, JPG, BMP GIF a Word | Asponer"
description: "Use Python Word API para convertir imágenes a Word en Python. Convierta una sola imagen o varias imágenes en Word en Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /es/words/convert-image-to-word-python/
author: "usman aziz"
summary: "En ciertos casos, debe convertir una sola imagen o un grupo de imágenes en un documento de Word. Para realizar esta operación mediante programación, este artículo muestra cómo convertir imágenes a Word DOC DOCX en Python."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Convertir imagen a Word en Python">}}

Los formatos de MS Word [DOC][1] y [DOCX][9] se utilizan ampliamente para crear documentos de texto enriquecido. Puede formatear texto e insertar varios elementos en documentos de Word, como imágenes. En ciertos casos, debe convertir una sola imagen o un grupo de imágenes en un documento de Word. Para realizar esta operación mediante programación, este artículo muestra cómo convertir imágenes a Word DOC DOCX en Python.

* [Biblioteca de conversión de imagen a Word de Python](#Library-to-Convert-Image-to-Word)
* [Convertir una imagen a Word DOC en Python](#Convert-an-Image-to-Word)
* [Convierta múltiples imágenes a DOCX en Python](#Convert-Multiple-Images-to-Word)

## Biblioteca de conversión de imagen a Word de Python - Descarga gratuita {#Library-to-Convert-Image-to-Word}

Para la conversión de imagen a Word DOC/DOCX, usaremos [Aspose.Words for Python][3]. Es una biblioteca rica en funciones para trabajar con documentos de Word, incluidos DOC, DOCX, etc. La biblioteca tiene un convertidor incorporado para la conversión de documentos de Word de ida y vuelta. Puede instalar la biblioteca desde [PyPI][4] usando el siguiente comando pip.

```
> pip install aspose-words
```

## Convertir una imagen a Word DOC en Python {#Convert-an-Image-to-Word}

Los siguientes son los pasos para convertir una imagen a un DOC de Word en Python.

* Primero, cree un nuevo documento usando la clase Document.
* Luego, cree un objeto DocumentBuilder e inicialícelo con el objeto Document.
* Inserte la imagen en el documento usando el método DocumentBuilder.insert_image(fileName).
* Finalmente, guarde el documento de Word usando el método Document.save(fileName).

El siguiente ejemplo de código muestra cómo convertir una imagen PNG a DOC en Python.

```
import aspose.words as aw

# Crear un nuevo documento
doc = aw.Document()

# Crear un generador de documentos
builder = aw.DocumentBuilder(doc)

# Insertar imagen en el documento
builder.insert_image("logo.png")

# Guardar como DOC
doc.save("image-to-word.doc")
```

## Convertir múltiples imágenes a Word en Python {#Convert-Multiple-Images-to-Word}

En la sección anterior, convertimos solo una imagen en un documento de Word. Sin embargo, en ciertos casos, es posible que deba convertir más de una imagen a la vez. Los siguientes son los pasos para convertir múltiples imágenes a un DOCX de Word en Python.

* Primero, cree un nuevo documento usando la clase Document.
* Luego, cree un objeto DocumentBuilder e inicialícelo con el objeto Document.
* Obtenga la lista de archivos de imagen de la carpeta deseada.
* Recorra la lista de archivos de imagen e inserte cada imagen en el documento utilizando el método DocumentBuilder.insert_image(fileName).
* Finalmente, guarde el documento de Word usando el método Document.save(fileName).

El siguiente ejemplo de código muestra la conversión de varias imágenes a un DOCX de Word en Python.

```
import aspose.words as aw
import os

# Directorio de imágenes
dir = "D:\\images\\"

# Crear un nuevo documento
doc = aw.Document()

# Crear un generador de documentos
builder = aw.DocumentBuilder(doc)

# Bucle a través de las imágenes en la carpeta
for imageFile in os.listdir(dir):
    # Insertar imagen en el documento
    builder.insert_image(os.path.join(dir, imageFile))

# Guardar como DOCX
doc.save("images-to-word.docx")
```

## Image to DOC Python Converter - Obtenga una licencia gratuita {#Get-a-Free-License}

Puede convertir imágenes a formatos de Word sin limitaciones de evaluación [obteniendo una licencia temporal gratuita][5].

## Convertidor de imagen de Python a DOCX - Leer más

Puede explorar más sobre Aspose.Words for Python usando [documentación][6]. En caso de que tenga alguna consulta, no dude en hacérnosla saber a través de nuestro [foro][7].

## Conclusión

En este artículo, ha aprendido cómo convertir una imagen en un documento de Word en Python. También demostramos cómo convertir varias imágenes en un documento Word DOC/DOCX mediante programación. Puede integrar fácilmente los ejemplos de código provistos en su aplicación y realizar la conversión de imagen a DOC o DOCX.

## Ver también

* [Genere archivos PDF usando C# – .NET PDF API](https://blog.aspose.com/es/2020/12/02/create-pdf-files-using-csharp/)
* [Convertir Word a PDF en Python](https://blog.aspose.com/es/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




