---
title: "Bild in Word in Python konvertieren"
seoTitle: "Bild in Word in Python konvertieren | Python PNG, JPG, BMP GIF in Word | Stellen Sie sich vor"
description: "Verwenden Sie die Python-Word-API, um Bilder in Python in Word zu konvertieren. Konvertieren Sie ein einzelnes Bild oder mehrere Bilder in ein Word in Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /de/words/convert-image-to-word-python/
author: "Usman Aziz"
summary: "In bestimmten Fällen müssen Sie ein einzelnes Bild oder mehrere Bilder in ein Word Dokument konvertieren. Um diesen Vorgang programmgesteuert auszuführen, zeigt dieser Artikel, wie Sie Bilder in Python in Word DOC DOCX konvertieren."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Bild in Word in Python konvertieren">}}

Die MS Word-Formate [DOC][1] und [DOCX][9] werden häufig zum Erstellen von Rich-Text Dokumenten verwendet. Sie können Text formatieren und verschiedene Elemente wie Bilder in Word Dokumente einfügen. In bestimmten Fällen müssen Sie ein einzelnes Bild oder mehrere Bilder in ein Word Dokument konvertieren. Um diesen Vorgang programmgesteuert auszuführen, zeigt dieser Artikel, wie Sie Bilder in Python in Word DOC DOCX konvertieren.

* [Bibliothek zum Konvertieren von Python bildern in Word](#Library-to-Convert-Image-to-Word)
* [Konvertieren Sie ein Bild in Word DOC in Python](#Convert-an-Image-to-Word)
* [Konvertieren Sie mehrere Bilder in Python in DOCX](#Convert-Multiple-Images-to-Word)

## Bibliothek zum Konvertieren von Python bildern in Word – kostenloser Download {#Library-to-Convert-Image-to-Word}

Für die Konvertierung von Bildern in Word DOC/DOCX verwenden wir [Aspose.Words for Python][3]. Es ist eine funktionsreiche Bibliothek zum Arbeiten mit Word Dokumenten, einschließlich DOC, DOCX usw. Die Bibliothek verfügt über einen integrierten Konverter für die Hin und Her-Konvertierung von Word Dokumenten. Sie können die Bibliothek von [PyPI][4] mit dem folgenden Pip-Befehl installieren.

```
> pip install aspose-words
```

## Konvertieren Sie ein Bild in Word DOC in Python {#Convert-an-Image-to-Word}

Im Folgenden sind die Schritte zum Konvertieren eines Bildes in ein Word-DOC in Python aufgeführt.

* Erstellen Sie zunächst ein neues Dokument mit der Document Klasse.
* Erstellen Sie dann ein DocumentBuilder Objekt und initialisieren Sie es mit dem Document Objekt.
* Fügen Sie das Bild mithilfe der Methode DocumentBuilder.insert_image(fileName) in das Dokument ein.
* Speichern Sie abschließend das Word Dokument mit der Methode Document.save(fileName).

Das folgende Codebeispiel zeigt, wie Sie ein PNG bild in Python in DOC konvertieren.

```
import aspose.words as aw

# Erstellen Sie ein neues Dokument
doc = aw.Document()

# Erstellen Sie einen Dokumentenersteller
builder = aw.DocumentBuilder(doc)

# Bild in das Dokument einfügen
builder.insert_image("logo.png")

# Als DOC speichern
doc.save("image-to-word.doc")
```

## Konvertieren Sie mehrere Bilder in Python in Word {#Convert-Multiple-Images-to-Word}

Im vorherigen Abschnitt haben wir nur ein einzelnes Bild in ein Word Dokument konvertiert. In bestimmten Fällen müssen Sie jedoch möglicherweise mehr als ein Bild auf einmal konvertieren. Im Folgenden sind die Schritte zum Konvertieren mehrerer Bilder in ein Word-DOCX in Python aufgeführt.

* Erstellen Sie zunächst ein neues Dokument mit der Document Klasse.
* Erstellen Sie dann ein DocumentBuilder Objekt und initialisieren Sie es mit dem Document Objekt.
* Holen Sie sich die Liste der Bilddateien aus dem gewünschten Ordner.
* Durchlaufen Sie die Liste der Bilddateien und fügen Sie jedes Bild mit der Methode DocumentBuilder.insert_image(fileName) in das Dokument ein.
* Speichern Sie abschließend das Word Dokument mit der Methode Document.save(fileName).

Das folgende Codebeispiel zeigt die Konvertierung mehrerer Bilder in ein Word-DOCX in Python.

```
import aspose.words as aw
import os

# Bildverzeichnis
dir = "D:\\images\\"

# Erstellen Sie ein neues Dokument
doc = aw.Document()

# Erstellen Sie einen Dokumentenersteller
builder = aw.DocumentBuilder(doc)

# Bilder im Ordner durchlaufen
for imageFile in os.listdir(dir):
    # Bild in das Dokument einfügen
    builder.insert_image(os.path.join(dir, imageFile))

# Als DOCX speichern
doc.save("images-to-word.docx")
```

## Image to DOC Python Converter - Holen Sie sich eine kostenlose Lizenz {#Get-a-Free-License}

Sie können Bilder ohne Evaluierungseinschränkungen in Word-Formate konvertieren, indem Sie [eine kostenlose temporäre Lizenz erwerben][5].

## Python-Image zu DOCX-Konverter - Mehr erfahren

Weitere Informationen zu Aspose.Words for Python finden Sie unter [Dokumentation][6]. Falls Sie Fragen haben, können Sie uns diese gerne über unser [Forum][7] mitteilen.

## Fazit

In diesem Artikel haben Sie gelernt, wie Sie ein Bild in Python in ein Word Dokument konvertieren. Wir haben auch gezeigt, wie Sie mehrere Bilder programmgesteuert in ein Word DOC/DOCX Dokument konvertieren. Sie können die bereitgestellten Codebeispiele einfach in Ihre Anwendung integrieren und die Konvertierung des Bildes in DOC oder DOCX durchführen.

## Siehe auch

* [Generieren Sie PDF Dateien mit C# – .NET PDF API](https://blog.aspose.com/de/2020/12/02/create-pdf-files-using-csharp/)
* [Konvertieren Sie Word in Python in PDF](https://blog.aspose.com/de/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




