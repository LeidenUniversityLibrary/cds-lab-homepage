---
title: Policies for enriching audio-visual materials
status: draft
date: 2019-03-06
author: Ben Companjen
---

# Introduction

This document should guide people who want to enrich audio(visual) materials such as videos, films, podcasts with descriptive metadata, details, context, or what have you.

The policies in this document are (somewhat) concrete recommendations for implementing the guiding principles in the [Enrichment Policy Framework](policy-framework.md). Both the framework and the policies in this document are based on the [Leiden University research data management policy framework](https://www.bibliotheek.universiteitleiden.nl/binaries/content/assets/ul2staff/reglementen/onderzoek/regeling-datamanagement-universiteit-leiden).

# Policies

## Use IIIF and the Web Annotation Framework if possible

The [International Image Interoperability Framework (IIIF)](https://iiif.io/) is a community-based set of standards for publishing, presenting, describing and annotating images on the Web – and AV resources as well, as of Presentation API 3.0. IIIF relies heavily on the [Web Annotation Framework](https://www.w3.org/TR/annotation-model/), a W3C standard for annotating Web resources.

### Create abstract resources to annotate

Use IIIF Canvases for pages/posters and annotate those instead of AV resources themselves. This is standard practice for IIIF-based resources.

### Don't copy if not necessary, always annotate the original

If you want to enrich AV resources provided online by trustworthy institutions you don't need to copy the resources. It is okay to keep a backup copy, but connect enrichments to the originals to make them as useful as possible.

### Add provenance to annotations

The Web Annotation Framework includes ways to attribute the creator(s) of each annotation, the time the annotation was created/generated, and the time(s) the annotation was modified. The tool(s) you use to annotate should help you keep track of your own work so that you can be credited for it, and held accountable.

## Keep provenance and licenses of source resources

Explain how the set of resources you selected for enrichment was created. This helps people assess how complete your set is and how representative it is among all similar resources.

If you have copies of resources, keep the licence conditions and creator information (and all other relevant provenance) close and preferably linked to the resources. You need to cite and deposit your data and this will help determine if and how resources can be shared.

## Store enrichments in a trustworthy data repository

If using IIIF and e.g. (some annotation editor for AV resources) to create and save annotations, make sure the annotations are stored on a server that securely stores them and that creates backups. The server should store the provenance of each annotation too and if necessary, all versions of annotations.

## Identify, identify, identify

Make sure everything has identifiers, preferably persistent identifiers (PIDs).
You should use PIDs for AV resources you annotate, and the server that stores your annotations should create PIDs for each (version of an) annotation.
This allows users to connect the right versions of annotations to the right versions of resources and recreate the context of the annotation at the time of its creation.

# Projects and Tools

[CLARIAH video annotation interoperability](https://github.com/CLARIAH/video-annotation-interoperability): discussion around Web Annotations for videos.

[Semantic Annotation Tool](http://mediaecology.dartmouth.edu/wp/projects/technology/the-semantic-annotation-tool): front-end ([Waldorf.js](https://github.com/colejd/Waldorf)) and back-end ([Statler](https://github.com/VEMILab/Statler)) that work with HTML5, JavaScript and Web Annotations.

[ELAN](https://tla.mpi.nl/tools/tla-tools/elan/): offline annotator that creates EAF files and various other annotation formats and connects to online knowledge bases for data categories (like CLARIN).

[VIAN](https://filmcolors.org/2018/03/08/vian/): not generally available yet.