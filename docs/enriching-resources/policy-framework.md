---
title: "Enriching Digital Objects: a Policy Framework"
---

**THIS IS A VERY ROUGH DRAFT; IT MAY NEVER BE ACTUAL POLICY.**

See the [definitions of objects and enriching](index.md#definitions-of-terms) before reading on.

# Principles 

- annotations are research data
- annotations enrich objects by adding or linking to information
    - privacy of annotators
    - ethical processing of annotation objects
    - secure access to annotations
    - preservation of annotations

# Laws and regulations

- GDPR
- Copyright

# Policies

Existing policy: [Digitaal Erfgoed Referentiearchitectuur (DERA)](https://www.netwerkdigitaalerfgoed.nl/wp-content/uploads/2018/11/181107-DERA2.0_def.pdf)

## Links between objects and enrichments

Define object bounds and types of enrichments. Objects may consist of various components, like high-resolution master image(s), thumbnail(s) and transcriptions of the text in the object.

Model enrichments as annotations directly or use an annotation to make discovering more complex external descriptions of the resource easier.
The latter use of annotations may be useful when an enrichment is more than a single connection between two objects.

## Annotations are research data

All policies for research data also apply to annotations, and hence to enrichments as well.

Enrichments should (thus) be FAIR.
Use standards for annotations, like the [Web Annotation Model](https://www.w3.org/TR/annotation-model/).

# Considerations

## Data formats for annotations

- RDF
    - CSV + CSV metadata
    - JSON-LD
    - Turtle
    - RDFa
- Nanopublications
- other data formats
    - Hypothes.is JSON
    - brat stand-off format
    - TEI
    - [VGG Image Annotator](https://gitlab.com/vgg/via) format (JSON or CSV)

## Bodies of annotations

Annotations can have one or more bodies, or none (for specific motivations). If there are multiple bodies, they are usually related, but *how* they are related may vary.

- external, can be anything
    - full resources
    - fragments of resources
- embedded
    - TextualBody
        - HTML fragment
        - plain text

### Example: TEI file as external body

When you transcribe text from manuscripts, you may want to use the TEI guidelines and markup.
You can refer to (fragments of) external TEI files as the body of annotations.

### Example: HTML file as external body

Many documents on the Web are available in HTML format. You can refer to (fragments of) HTML files as the body of annotations.

## Motivation and purpose of annotations

In the Web Annotation Model, motivation and purpose are used to present a reason for the annotation, thereby also explaining the nature of the relationship between the target and the body of the annotation.

!!! note
    The motivations and purposes defined by the Web Annotation Model are useful, but deliberately generic. They can be specialised, though any terms created for special purposes should get persistent identifiers and clear explanations for their use.

## Storage and access

- Linked Data
    - URIs resolve to descriptions
    - access one object at a time
- Linked Data Fragments / Triple Pattern Fragments
- SPARQL endpoint
- RDF dumps in a TDR

## Informing the object holder

When annotations are not stored by the provider (holder) of the annotated object, they may be informed about the annotations. Some providers may provide instructions for informing them.

## Correctness

Annotations are RDF graphs and can include authorship information about the external body, but what if this doesn't match the metadata of the external body? The Web Annotation Model specifies that the external body's metadata is the canonical source.

## Access control

Who can add, edit and delete annotations? How do you authenticate and authorise users?

## Copyright and content policies

What kind of content may be added in annotations? How will you monitor whether users adhere to this? What do you do in case of violations of copyright laws or content policies? Who decides what is allowed and who makes the final decision in case of a dispute over contents of annotations?

