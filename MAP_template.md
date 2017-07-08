---
title: Name of Model / Metadata Application Profile   
author: Name
contact: email / GH handle / other contact method for author / maintainer of this MAP
date: YYYY-MM-DD
profile:
  organization: Related Organization, if appropriate
  project: Related Project, if appropriate
  system or repository: the repository system where this MAP is expected to be used
  namespaces: involved namespaces. a few common ones are included for help getting started.
    dce:    http://purl.org/dc/elements/1.1/
    dct:    http://purl.org/dc/terms/
    edm:    http://www.europeana.eu/schemas/edm/
    fcr:    info:fedora/fedora-system:
    foaf:   http://xmlns.com/foaf/0.1/
    mrel:   http://id.loc.gov/vocabulary/relators/
    pcdm:   http://pcdm.org/models#Object
    premis: http://www.loc.gov/premis/rdf/v1#
    rdfs:   http://www.w3.org/2000/01/rdf-schema#
    sufia:  http://scholarsphere.psu.edu/ns#
    sweet:  http://sweet.jpl.nasa.gov/2.2/reprDataFormat.owl#
    works:  http://pcdm.org/works#
    xsd:    http://www.w3.org/2001/XMLSchema#
---

# Name of Model / Metadata Application Profile

## About

Describe here in a few sentences:
- what this model and metadata application profile is describing;
- the parts / pieces / object types involved ;
- an example of an instance of the object(s) involved ;
- any other details that help with comprehension.

## Use Cases

* List here any use cases that are driving this model & MAP. This helps relate end user functionality to underlying metadata work.

## Data Model
Include a diagram of the Model if appropriate or available.

## Metadata Application Profile

### `class name & hierarchy`
(e.g. `hydraworks:Work < pcdm:Object` or `pcdm:Collection`)

#### `Metadata Profile`
(e.g. you can separate out `Descriptive`, `Administrative`, etc. if that makes sense, or just include a general profile)

Fill out the following for fields that are asserted on instances of the given class. This should be all possible fields, not just required fields, following the expectations and scope of the given system this MAP applies to. Choose either the Basic Profile or the Extended profile based on your needs and abilities.

Basic profile:

| Field              | Predicate                   | Recommendation | Expected Value                        | Obligation |
| ------------------ | --------------------------- | -------------- | ------------------------------------- | ---------- |
| *title*            | `dct:title`                 | MUST           | `xsd:string`                          | {1}        |
| *creator*          | `dce:creator`               | SHOULD         | `xsd:string`                          | {0,n}      |

... (etc.)

Extended profile:

| Field | Predicate | Recommendation | Expected Value (Data Type) | Expected Value (Source) | Obligation | ActiveFedora Model | Solr Mapping(s) | Related Docs |
| ----- | --------- | -------------- | -------------------------- | ----------------------- | ---------- | ------------------ | --------------- | -------------|
| *date modified*  | `dct:modified`         | MUST           | `xsd:dateTime`             | n/a                                | {1}        | core_metadata.rb   |                 |              |

... (etc.)
