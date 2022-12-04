---
title: "Convertir une image en Word en Python"
seoTitle: "Convertir une image en Word en Python | Python PNG, JPG, BMP GIF vers Word | Asposé"
description: "Utilisez l'API Python Word pour convertir des images en Word en Python. Convertissez une ou plusieurs images en un mot en Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /fr/words/convert-image-to-word-python/
author: "Usman Aziz"
summary: "Dans certains cas, vous devez convertir une seule image ou un groupe d'images en un document Word. Pour effectuer cette opération par programmation, cet article montre comment convertir des images en Word DOC DOCX en Python."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Convertir une image en Word en Python">}}

Les formats MS Word [DOC][1] et [DOCX][9] sont largement utilisés pour créer des documents en texte enrichi. Vous pouvez formater du texte et insérer divers éléments dans des documents Word tels que des images. Dans certains cas, vous devez convertir une seule image ou un groupe d'images en un document Word. Pour effectuer cette opération par programmation, cet article montre comment convertir des images en Word DOC DOCX en Python.

* [Bibliothèque de conversion d'images en mots Python](#Library-to-Convert-Image-to-Word)
* [Convertir une image en Word DOC en Python](#Convert-an-Image-to-Word)
* [Convertir plusieurs images en DOCX en Python](#Convert-Multiple-Images-to-Word)

## Bibliothèque de conversion d'image en mot Python - Téléchargement gratuit {#Library-to-Convert-Image-to-Word}

Pour la conversion de l'image en Word DOC/DOCX, nous utiliserons [Aspose.Words for Python][3]. Il s'agit d'une bibliothèque riche en fonctionnalités pour travailler avec des documents Word, y compris DOC, DOCX, etc. La bibliothèque dispose d'un convertisseur intégré pour la conversion aller-retour des documents Word. Vous pouvez installer la bibliothèque à partir de [PyPI][4] à l'aide de la commande pip suivante.

```
> pip install aspose-words
```

## Convertir une image en Word DOC en Python {#Convert-an-Image-to-Word}

Voici les étapes pour convertir une image en Word DOC en Python.

* Tout d'abord, créez un nouveau document à l'aide de la classe Document.
* Ensuite, créez un objet DocumentBuilder et initialisez-le avec l'objet Document.
* Insérez l'image dans le document à l'aide de la méthode DocumentBuilder.insert_image(fileName).
* Enfin, enregistrez le document Word à l'aide de la méthode Document.save(fileName).

L'exemple de code suivant montre comment convertir une image PNG en DOC en Python.

```
import aspose.words as aw

# Créer un nouveau document
doc = aw.Document()

# Créer un générateur de documents
builder = aw.DocumentBuilder(doc)

# Insérer une image dans le document
builder.insert_image("logo.png")

# Enregistrer au format DOC
doc.save("image-to-word.doc")
```

## Convertir plusieurs images en Word en Python {#Convert-Multiple-Images-to-Word}

Dans la section précédente, nous avons converti une seule image en document Word. Cependant, dans certains cas, vous devrez peut-être convertir plusieurs images à la fois. Voici les étapes pour convertir plusieurs images en un Word DOCX en Python.

* Tout d'abord, créez un nouveau document à l'aide de la classe Document.
* Ensuite, créez un objet DocumentBuilder et initialisez-le avec l'objet Document.
* Obtenez la liste des fichiers image du dossier souhaité.
* Parcourez la liste des fichiers image et insérez chaque image dans le document à l'aide de la méthode DocumentBuilder.insert_image(fileName).
* Enfin, enregistrez le document Word à l'aide de la méthode Document.save(fileName).

L'exemple de code suivant montre la conversion de plusieurs images en un Word DOCX en Python.

```
import aspose.words as aw
import os

# Répertoire d'images
dir = "D:\\images\\"

# Créer un nouveau document
doc = aw.Document()

# Créer un générateur de documents
builder = aw.DocumentBuilder(doc)

# Boucle à travers les images dans le dossier
for imageFile in os.listdir(dir):
    # Insérer une image dans le document
    builder.insert_image(os.path.join(dir, imageFile))

# Enregistrer au format DOCX
doc.save("images-to-word.docx")
```

## Image to DOC Python Converter - Obtenez une licence gratuite {#Get-a-Free-License}

Vous pouvez convertir des images au format Word sans limitation d'évaluation en [obtenant une licence temporaire gratuite][5].

## Convertisseur d'image Python en DOCX - En savoir plus

Vous pouvez en savoir plus sur Aspose.Words for Python en utilisant [documentation][6]. Si vous avez des questions, n'hésitez pas à nous en faire part via notre [forum][7].

## Conclusion

Dans cet article, vous avez appris à convertir une image en document Word en Python. Nous avons également montré comment convertir plusieurs images en un document Word DOC/DOCX par programme. Vous pouvez facilement intégrer les exemples de code fournis dans votre application et effectuer la conversion de l'image en DOC ou DOCX.

## Voir également

* [Générer des fichiers PDF à l'aide de C # - API PDF .NET](https://blog.aspose.com/fr/2020/12/02/create-pdf-files-using-csharp/)
* [Convertir Word en PDF en Python](https://blog.aspose.com/fr/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




