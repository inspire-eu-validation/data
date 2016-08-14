# Conformance class: INSPIRE GML application schemas (DRAFT)

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3).

This conformance class examines GML documents against the requirements for the GML encoding for spatial data sets in INSPIRE. This only covers generic requirements that apply across application schemas. Requirements related to specific application schemas are part of conformance classes with a dependency on this conformance class. 

## Standardization target type

INSPIRE spatial data set encoded in GML

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the metadata record, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [INSPIRE Guidelines for the encoding of spatial data version 3.3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/D2.7_v3.3.pdf) | [INSPIRE GML encoding](http://inspire.ec.europa.eu/id/ats/data-encoding/3.3/inspire-gml) | n/a |

### Indirect dependencies

none

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
D2.7 <a name="ref_D2_7"></a>   | [INSPIRE Guidelines for the encoding of spatial data version 3.3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/D2.7_v3.3.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS Template](#ref_TG-DS_tmpl) |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Schema](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/schema)  | ready for review  | A.1.1 |
| [Schema validation](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/schema-validation)  | ready for review  | A.1.1, A.1.2, A.1.3, A.1.4, A.1.5, A.3.2, (A.6.1), A.8.1, A.9.5  |
| [GML model](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/gml-model)  | ready for review  | A.1.3, (A.6.1), A.9.5  |
| [Simple features](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/simple-features)  | ready for review  | A.1.7  |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
base           | http://inspire.ec.europa.eu/schemas/base/3.3
gml            | http://www.opengis.net/gml/3.2
wfs            | http://www.opengis.net/wfs/2.0
xsi            | http://www.w3.org/2001/XMLSchema-instance
xlink          | http://www.w3.org/1999/xlink
xml            | http://www.w3.org/XML/1998/namespace
hy-n           | http://inspire.ec.europa.eu/schemas/hy-n/3.0 or http://inspire.ec.europa.eu/schemas/hy-n/4.0
hy-p           | http://inspire.ec.europa.eu/schemas/hy-p/3.0 or http://inspire.ec.europa.eu/schemas/hy-p/4.0
