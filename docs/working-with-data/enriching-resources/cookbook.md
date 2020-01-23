---
title: Enrichments cookbook
author: Ben Companjen
date: 2019-03-13
---

This cookbook contains recipes for enrichment of digital objects.
It is never finished and non-normative, and will have lots of links to examples elsewhere.
However, it is the intention of the Centre for Digital Scholarship to provide good examples and not to create a comprehensive list of every project ever undertaken.

# Example enrichments

## Identify people in images

!!! warning
    Mind the rules for working with personal data.

Here are two ways of identifying people in images. Assuming that the abstract representation of the image is more stable and versatile than individual images, annotating the canvas is preferred.

### Annotate (part of) the Canvas (preferred)

1. Create a [Canvas][] for the image, if it doesn't exist yet.
2. Annotate the part (i.e. fragment) of the Canvas with a Web Annotation with the `identifying` motivation and the URI of the person as the body.

### Annotate (part of) the image directly

1. Annotate the part (i.e. fragment) of the image with a Web Annotation with the `identifying` motivation and the URI of the person as the body.

## Classify objects in images

When you cannot or do not want to identify specific objects, but do want to say what *kind of object* they are, you can link an object *class* to (part of) an image.

!!! warning
    Understand the ethics of classifying real-world objects, including (especially) people or peoples and objects involved in disputes.

Annotate the part (i.e. fragment) of the Canvas or image with a Web Annotation with the `classifying` motivation and the URI of the object as the body URI.

## Link an image to its original

If you believe an image is derived from another image, you can link them in the following way: (TODO)

# Example workflows

## Record tags for items in a spreadsheet

When you want to assign a single tag to each item, put the identifier for the item the first column and the tag in the second.

When you want to assign one or more tags to each item, you can either:

- add a row for each combination of item and tag
- concatenate the tags in the second column, separated by a comma, semicolon or other character that is never part of the tag

!!! note
    Spreadsheets allow data entry in very flexible ways. However, for reusability you should stick to keeping your data in a rectangular table.
