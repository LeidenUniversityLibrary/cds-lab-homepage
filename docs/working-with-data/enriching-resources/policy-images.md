---
title: Policies for enriching images
status: draft
author: Ben Companjen
---

# Introduction

This document should guide people[^1] who want to enrich image-based materials such as photos, paintings and (scanned) texts with descriptive metadata, details, context, or what have you.

The policies in this document are (somewhat) concrete recommendations for implementing the guiding principles in the [Enrichment Policy Framework](policy-framework.md).
Both the framework and the policies in this document are based on the [Leiden University research data management policy framework](https://www.bibliotheek.universiteitleiden.nl/binaries/content/assets/ul2staff/reglementen/onderzoek/regeling-datamanagement-universiteit-leiden).

# Policies

## Use IIIF and the Web Annotation Framework if possible

The [International Image Interoperability Framework (IIIF)](https://iiif.io/) is a community-based set of standards for publishing, presenting, describing and annotating images on the Web. IIIF relies heavily on the [Web Annotation Framework](https://www.w3.org/TR/annotation-model/), a W3C standard for annotating Web resources.

### Create abstract resources to annotate

Use IIIF Canvases for pages/posters and annotate those instead of images. This is standard practice for IIIF-based resources.

### Don't copy if not necessary, always annotate the original

If you want to enrich images provided online by trustworthy institutions you don't need to copy the images.
It is okay to keep a backup copy, but connect enrichments to the originals to make them as useful as possible.
Other people may have annotated the same images, but only by referring to each image
using the same identifiers, can computers understand that all annotations are of
the same image.

### Add provenance to annotations

The Web Annotation Framework includes ways to attribute the creator(s) of each annotation,
the time the annotation was created/generated, and the time(s) the annotation was modified.
The tool(s) you use to annotate should help you keep track of your own work so that you can be credited for it, and held accountable.
Naturally, if you only make the annotations of others available, you should include
the identities of the original creators.

## Record provenance and licenses of source images

Explain how the set of images you selected for enrichment was created.
This helps people assess how complete your set is and how representative it is among all similar images.

If you have copies of images, keep the licence conditions and creator information (and all other relevant provenance) close and preferably linked to the images.
You need to cite and deposit your data and this will help determine if and how images can be shared.

## Store enrichments in a trustworthy data repository

If using IIIF and e.g. Mirador to create and save annotations, make sure the annotations are stored on a server that securely stores them and that creates backups. The server should store the provenance of each annotation too and if necessary, all versions of annotations.

## Identify, identify, identify

Make sure everything has identifiers, preferably persistent identifiers (PIDs).
You should use PIDs for images you annotate, and the server that stores your annotations should create PIDs for each (version of an) annotation.
This allows users to connect the right versions of annotations to the right versions of images and recreate the context of the annotation at the time of its creation.

!!! note
    The Web Annotation Model has another option to specify which representation of a
    resource was annotated: [Resource State](https://www.w3.org/TR/annotation-model/#states).

[^1]: Although we say people, the main audience is researchers.
