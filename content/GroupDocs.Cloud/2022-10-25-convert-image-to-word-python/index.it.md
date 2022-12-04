---
title: "Converti immagine in Word in Python"
seoTitle: "Converti immagine in Word in Python | Python PNG, JPG, BMP GIF in Word | Assumere"
description: "Usa Python Word API per convertire le immagini in Word in Python. Converti una singola immagine o più immagini in una parola in Python."
date: Mon, 25 Oct 2022 05:00:00 +0000
draft: false
url: /it/words/convert-image-to-word-python/
author: "Usman Aziz"
summary: "In alcuni casi, devi convertire una singola immagine o più immagini in un documento Word. Per eseguire questa operazione a livello di codice, questo articolo mostra come convertire le immagini in Word DOC DOCX in Python."
tags: ['convert image to word in python', 'convert png to word in python', 'convert jpg to word in python']
categories: ['Aspose.Words Product Family']
---

{{< figure align=center src="images/image-to-word-python.png" alt="Converti immagine in Word in Python">}}

I formati MS Word [DOC][1] e [DOCX][9] sono ampiamente utilizzati per creare documenti RTF. Puoi formattare il testo e inserire vari elementi nei documenti di Word come le immagini. In alcuni casi, devi convertire una singola immagine o più immagini in un documento Word. Per eseguire questa operazione a livello di codice, questo articolo mostra come convertire le immagini in Word DOC DOCX in Python.

* [Libreria del convertitore da immagine a Word Python](#Library-to-Convert-Image-to-Word)
* [Converti un'immagine in Word DOC in Python](#Convert-an-Image-to-Word)
* [Converti più immagini in DOCX in Python](#Convert-Multiple-Images-to-Word)

## Libreria del convertitore da immagini a Word Python - Download gratuito {#Library-to-Convert-Image-to-Word}

Per la conversione da immagine a Word DOC/DOCX, utilizzeremo [Aspose.Words for Python][3]. È una libreria ricca di funzionalità per lavorare con documenti Word inclusi DOC, DOCX, ecc. La libreria ha un convertitore integrato per la conversione avanti e indietro di documenti Word. Puoi installare la libreria da [PyPI][4] usando il seguente comando pip.

```
> pip install aspose-words
```

## Converti un'immagine in Word DOC in Python {#Convert-an-Image-to-Word}

Di seguito sono riportati i passaggi per convertire un'immagine in un Word DOC in Python.

* Innanzitutto, crea un nuovo documento utilizzando la classe Document.
* Quindi, crea un oggetto DocumentBuilder e inizializzalo con l'oggetto Document.
* Inserisci l'immagine nel documento utilizzando il metodo DocumentBuilder.insert_image(fileName).
* Infine, salva il documento di Word usando il metodo Document.save(fileName).

L'esempio di codice seguente mostra come convertire un'immagine PNG in DOC in Python.

```
import aspose.words as aw

# Crea un nuovo documento
doc = aw.Document()

# Crea un generatore di documenti
builder = aw.DocumentBuilder(doc)

# Inserisci l'immagine nel documento
builder.insert_image("logo.png")

# Salva come DOC
doc.save("image-to-word.doc")
```

## Converti più immagini in Word in Python {#Convert-Multiple-Images-to-Word}

Nella sezione precedente, abbiamo convertito solo una singola immagine in un documento Word. Tuttavia, in alcuni casi, potrebbe essere necessario convertire più di un'immagine alla volta. Di seguito sono riportati i passaggi per convertire più immagini in un Word DOCX in Python.

* Innanzitutto, crea un nuovo documento utilizzando la classe Document.
* Quindi, crea un oggetto DocumentBuilder e inizializzalo con l'oggetto Document.
* Ottieni l'elenco dei file di immagine dalla cartella desiderata.
* Scorri l'elenco dei file di immagine e inserisci ogni immagine nel documento utilizzando il metodo DocumentBuilder.insert_image(fileName).
* Infine, salva il documento di Word usando il metodo Document.save(fileName).

L'esempio di codice seguente mostra la conversione di più immagini in Word DOCX in Python.

```
import aspose.words as aw
import os

# Directory delle immagini
dir = "D:\\images\\"

# Crea un nuovo documento
doc = aw.Document()

# Crea un generatore di documenti
builder = aw.DocumentBuilder(doc)

# Scorri le immagini nella cartella
for imageFile in os.listdir(dir):
    # Inserisci l'immagine nel documento
    builder.insert_image(os.path.join(dir, imageFile))

# Salva come DOCX
doc.save("images-to-word.docx")
```

## Convertitore da immagine a DOC Python - Ottieni una licenza gratuita {#Get-a-Free-License}

Puoi convertire le immagini in formati Word senza limitazioni di valutazione [ottenendo una licenza temporanea gratuita][5].

## Convertitore da immagine Python a DOCX - Ulteriori informazioni

Puoi esplorare di più su Aspose.Words for Python usando [documentazione][6]. In caso di domande, non esitare a farcelo sapere tramite il nostro [forum][7].

## Conclusione

In questo articolo, hai imparato come convertire un'immagine in un documento Word in Python. Abbiamo anche dimostrato come convertire più immagini in un documento Word DOC/DOCX a livello di codice. Puoi facilmente integrare gli esempi di codice forniti nella tua applicazione ed eseguire la conversione dell'immagine in DOC o DOCX.

## Guarda anche

* [Genera file PDF utilizzando C# – .NET PDF API](https://blog.aspose.com/it/2020/12/02/create-pdf-files-using-csharp/)
* [Converti Word in PDF in Python](https://blog.aspose.com/it/2021/10/27/convert-word-to-pdf-in-python/)


[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/image/png/
[3]: https://products.aspose.com/words/python-net/
[4]: https://pypi.org/project/aspose-words/
[5]: https://purchase.aspose.com/temporary-license/
[6]: https://docs.aspose.com/words/python-net/
[7]: https://forum.aspose.com/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/word-processing/docx/




