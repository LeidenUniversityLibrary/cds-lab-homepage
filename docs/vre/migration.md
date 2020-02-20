---
title: Migrating or exporting data from a VRE
status: draft
---

This page describes the general process of moving data out of SharePoint
and into a data model and data format that can be used in different
contexts. In general, these converted data can be readily stored in a
data archive.

If you have a SharePoint VRE and would like to export your data, please
[contact the Centre for Digital Scholarship][cds] for information.

[cds]: https://www.library.universiteitleiden.nl/research-and-publishing/centre-for-digital-scholarship

# Data modelling

Unless you only used the VRE for sharing files that are read and edited
outside the VRE, you probably have information that is managed directly
in SharePoint. The data model explains what the information is about.

Some projects already started with a highly structured data model, other
projects need more help to reshape their data into models that are more
interoperable with existing datasets.

In many cases, we will meet several times
to discuss what your data describe and how data points are interrelated.

# Find models to map to

For your data to be understandable to other researchers (or anyone else,
really), it helps to "speak the same language", i.e. use common data models.
Many people have already created data models to describe for example books,
people, architecture and art, genes, et cetera.
However, not everyone describes every item in the same
way, so you may need to extend or adapt an existing data model.

There are too many possible models to list here, so we only link to some
databases that provide overviews of existing models:

- [Linked Open Vocabularies (LOV)](https://lov.linkeddata.es/dataset/lov/) indexes ontologies and RDF Schemas
- [FAIRsharing](https://fairsharing.org/) collects standards, databases and policies

# Iteratively create mapping(s) and test their correctness

Use SharePoint's legacy XML export or REST API with Atom XML to get the data.

Transform the data to the target model using, for example, XSLT or [RML].
Do not try to create a complete mapping in one go, but start simple and
improve one step at a time.

[RML]: https://rml.io/

# Perform the migration

When you are happy with the results of your mapping and transformation testing,
do it once more for all data and add metadata about the dataset, including its provenance.
This is the data that you will publish, archive or maybe continue working on using
other tools.

# Archive the data

See the [Research Data Services catalogue][rds] for information on data archives.

[rds]: https://digitalscholarship.nl/rds/
