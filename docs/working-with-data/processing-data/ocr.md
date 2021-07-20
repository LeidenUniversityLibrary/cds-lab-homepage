---
title: Optical character recognition (OCR)
status: draft
---

Recognise print text in images with any of these tools.

# ABBYY FineReader

ABBYY FineReader is considered very good for OCR in many languages.
However, it is not cheap.

# Adobe Acrobat

Adobe Acrobat has OCR capabilities for PDFs.
However, not all languages are supported (e.g. Arabic).

# Tesseract

Tesseract is open source and free to use.
It has support for many languages, can be (re)trained for other languages
and achieves good results.
It requires a little knowledge of the command line and
supports only a limited number of image formats for inputs.

# OCRmyPDF

For PDFs without a text layer, [OCRmyPDF] is a very useful toolkit.
It is a command-line tool that uses Tesseract under the hood,
as well as various preprocessing tools to straighten (deskew) the text lines
and removing noise – if you want it to.

[OCRmyPDF]: https://ocrmypdf.readthedocs.io/

# Kraken / Ocropy

Kraken and Ocropy are related OCR applications, as they build on one another.
They are both open source and free to use.
Kraken is relatively easy to train.
Instead of full pages, Kraken recognises text in single lines.

# Calamari

Calamari is also open source and free to use.
