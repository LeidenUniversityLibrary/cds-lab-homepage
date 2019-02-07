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

## Links between objects and enrichments

Define object bounds and types of enrichments. Objects may consist of various components, like high-resolution master image(s), thumbnail(s) and transcriptions of the text in the object.

Model enrichments as annotations

## Annotations are research data

All policies for research data also apply to annotations, and hence to enrichments as well.

Enrichments should (thus) be FAIR.
Use standards for annotations, like the Web Annotation Framework.

# Considerations

## Data formats for annotations

- RDF
    - CSV + CSV metadata
    - JSON-LD
    - Turtle
- Nanopublications

## Bodies of annotations

Annotations can have one or more bodies, or none (for specific motivations). If there are multiple bodies, they are usually related, but *how* they are related may vary.

- external, can be anything
    - full resources
    - fragments of resources
- embedded
    - TextualBody
        - HTML fragment
        - plain text


## Storage and access

- Linked Data
    - URIs resolve to descriptions
    - access one object at a time
- Linked Data Fragments / Triple Pattern Fragments
- SPARQL endpoint
- RDF dumps in a TDR

## Correctness

Annotations are RDF graphs and can include authorship information about the external body, but what if this doesn't match the metadata of the external body? The Web Annotation Model specifies that the external body's metadata is the canonical source.

## Access control

Who can add, edit and delete annotations? How do you authenticate and authorise users?

## Copyright and content policies

What kind of content may be added in annotations? How will you monitor whether users adhere to this? What do you do in case of violations of copyright laws or content policies? Who decides what is allowed and who makes the final decision in case of a dispute over contents of annotations?

# Aspecten in het advies

Hebben we eenzelfde beeld van waar onze collecties uit bestaan? Komen de modellen voor boeken, AV-objecten een beetje overeen?

soorten objecten

bij gedigitaliseerde objecten: links met analoge originelen

Modellen voor objecten en collecties,

Collectieobjecten en entiteiten gelinkt aan, maar buiten de collectie (mensen, concepten, etc.)

Toegangsmanieren: bulkdownload, API's, geen toegang maar code naar data brengen

Opslag voor verrijkingen

"Ondersteunde" modellen voor verrijkingen en diensten voor zulke verrijkingen

Tijdspad, stappen, pilots

# Andere initiatieven

[Collections as Data](https://collectionsasdata.github.io/)

FAIR – UvA-idee "FAIR Collections"

NDE, DERA

UBL-KB-pilot IIIF

See Zotero collection "Collection Enrichment"

OAIS object model, PROV model.