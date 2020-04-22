---
title: Generic guidance for enrichment projects
---

Are you interested in 'doing something' with digital artefacts from (cultural) heritage institutions?
Do you want to collect, describe, annotate or present them in a certain way, as part of your research
or for any other purpose?
Then this guide may be for you.

This guide aims to help researchers *plan* and *execute* projects that include any or all of the above activities.
It is (being) written by the Centre for Digital Scholarship, who help researchers at Leiden University
use digital data, manage research data and publish in Open Access. We consider enriching objects to be
both *working with digital data* and *creating and managing research data*.

The guide covers:

- definitions of (digital) objects and enriching objects
- goals of enriching objects
- sources of objects to enrich
- what kinds of enrichments exist
- where to store your enrichments and how to share them

This document can be used as a reference for (research) projects in which (digital) objects are collected, described, annotated and presented.
If you intend to perform these activities, you are reusing and creating data.
Especially when you data you want to use come from cultural heritage collections, we say you are *enriching* the objects.
Doing this properly can save you and others lots of effort and it will definitely make your research better.
It is not meant as a template for projects that you fill out like a form,
but you should be able to use it as inspiration for writing your project proposal.

For any questions, please get in touch with the [Centre for Digital Scholarship][cds].

[cds]: https://www.library.universiteitleiden.nl/about-us/centre-for-digital-scholarship

# Definitions of terms

## What are digital objects?

Digital objects are artefacts in our digital collections. They may be digital representations of 'analog' objects or born-digital materials. The digital objects that are subject to these policies are the ones that Libraries have taken custodianship over.

## What is 'enriching digital objects'?

Enriching a digital object means putting the object in context(s) by adding information or linking to related information or objects to provide more value to the object's users.

Enriching an object, depending on your goals, could include:

- providing a description of the object's contents so that it can be better indexed or understood
- providing a link to a similar object
- provide provenance analysis
- transcribe text in images

# Goals of enrichment

As with any project, you should first understand the goals of the project in which you want to enrich objects.
Think about:

- What research questions are you trying to answer?
- How is enriching objects helping you to answer your questions?

Intuitively, you need to enrich objects because the objects themselves and existing descriptions
do not give you the information that helps you answer your research questions.

!!! example
    If you want to know how often a cat appears in photos in a specific collection,
    but the metadata describing the photographs do not mention whether a cat is
    present, you may want to collect this data. To help others with similar questions
    and to show off your work, you could enrich the photographs by adding *cat* or
    *no cat* as annotations. If you create these annotations in a standardised, digital
    way, a script can then easily tally the number of photographs
    with and without cats.

Will you be working with a few example objects or are you trying to generalise by working with a large set of objects?

Who else might be interested in the results of your enrichment activities?
What other projects have inspired you to try this?

# Sources: objects to enrich

What is your source material? Where will you get it? Who owns the rights to the source materials?

Objects may be textual, visual, audible or of a different nature – or of a combination of 'natures'. The type(s) of your source materials will influence the way you work with them, starting with how you retrieve them.

If the objects you want to collect and enrich are available online, published by trustworthy archives or libraries, accessible via persistent identifiers and stable and open protocols, there is no need to create copies on your own computer. Copying such objects may even make your research harder, as you have to pay for the extra storage, manage backups[^1], find a way to share 'your' copies with colleagues and make sure your enrichments can be linked to the originals.

[^1]: You should already have a way of managing backups of everything important on your computer. Ask your IT department for help with this.

It is a different story when the originals are not digitised, only available within the holding institution, or don't have persistent identifiers. Maybe for security or privacy you can only work with them offline, with strict access controls for everything related to the objects – including enrichments. This will not be covered in this guide.

In some cases it is okay to create digital representations of objects yourself and use those in the project. Note that you may need approval from the owner or holding institute. Also, you will also need to describe the representations, keep links to the originals through identifiers and arrange for storage.
Creating representations of objects should be done in a very consistent manner, following best practices for the specific types of objects and the goals of the project.  

# Models for objects and enrichments

Depending on the type of objects you are using, different kinds of enrichments can be used. The way you refer to (fragments of) objects varies as well.
What are the parts to each of your objects? Files, metadata files, database rows?

What do you want to do with your objects? Add descriptions of the whole object, or parts of the object? Do you want to link to other objects in the same collection, or link to external objects or concepts?
What are the parts to each of your enrichments? A collection name, general description, tags, contextual information? Do you put them in a Word document, HTML files, a spreadsheet, a database, an annotation service?

# System components and procedures

To perform the actual enrichment, you will need a method – tools (e.g. software) that help you create and
store enrichments and procedures for working with the tools.
In the past, perhaps you would take structured notes on index cards and share (copies of) the cards with researchers that you know.
Nowadays, you may want to select parts of an image and fill a few fields in a form right next to the image and
allow non-expert *citizen scientists* to help you (with automatic validation of their input).
Your goals, sources and models all influence how the system should be configured and what procedures you need to have in place.

Keep in mind that systems and system components need maintenance and usually cost money.
This may mean that systems or components that you use during the project are not necessarily
available (let alone maintained) after the project, unless you can afford keeping them available
using other funds and/or organisational infrastructure.
You should always ensure that any enrichments you create in your project can be used outside
the system(s) you use to create them.

## Procedures

- collecting sources not available online
- basic description of sources
- creating enrichments
- grouping enrichments in versioned datasets
- updating enrichments
- authorising users (researchers, non-experts)
- training humans
- training machines
- discussing enrichments
- validating enrichments
- presenting enrichments

## System components

- Content Management System
    - authentication and authorisation of users
    - publication of sources with basic descriptions
    - publication of tutorials
- annotation tool(s)
- machine learning tool(s)
- data conversion tools
- data import tools
- data management / archiving system

# Storage and publication

As mentioned above, you should ensure your data is stored safely to prevent loss and unauthorised access and changes. See [Data protection](https://www.library.universiteitleiden.nl/research-and-publishing/datamanagement/data-protection) for some pointers.

Ideally your enrichments are available via standard interfaces and protocols as soon as possible after their creation (and possibly validation).
Even better is when they are available for the long term with *persistent identifiers*
that resolve to the latest location when the data of your enrichment are relocated to other computers.

You should archive your enrichments in a research data archive at least once,
at the end of the project, or when the enrichments are finished.
This ensures that nothing is lost, even if the system is shut down at the end of the project.
It also allows you to cite the data as a dataset in your own publications.
