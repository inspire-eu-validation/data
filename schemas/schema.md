# Schema

**Version**: 1

**Purpose**: Verify whether each relevant element of the dataset under inspection carries a name specified in the target application schema.

**Prerequisites**

n/a

**Test method**

* Verify whether each relevant element of the source data set under inspection has been properly mapped to the INSPIRE application schemas. Inspect the documentation of the source data set and determine, if all relevant information has been mapped correctly to the INSPIRE application schema, i.e. that spatial object types, data types, attributes, association roles, code lists, and enumerations are mapped to the INSPIRE application schemas with the correct designation of mnemonic names.
* Inspect the XML Schema namespace of each feature element. If a namespace URI does not start with "http://inspire.ec.europa.eu/schemas/" or "urn:x-inspire:specification:gmlas:" it is not one of the approved INSPIRE application schema namespaces. Review the extension documentation for the identified namespaces to check that any extensions do not overlap with the spatial object types and associated data types and enumerations that are defined in Annexes II, III and IV of the Implementing Rule.

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 4 (1)

**Test type**: Manual

## Messages

n/a

## Contextual XPath references

n/a