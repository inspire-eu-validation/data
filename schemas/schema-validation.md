# Validation against declared schema

**Version**: 1

**Purpose**: Verify that all XML documents validate against the XML schema(s) declared in the schemaLocation attribute.

**Prerequisites**

**Test method**

* Verify for each XML document that in the root element a [schemaLocation](#schemaLocation) attribute is provided. Otherwise report [noSchemaLocation](#noSchemaLocation)
* Validate each document against the schema(s) specified in the xsi:schemaLocation attribute using strict XML schema validation. Otherwise report [invalidSchema](#invalidSchema).

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 3
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 4 (2)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 4 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 5 (2)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 5 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 6 (5)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 9 (1)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) TG requirement 1
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) TG requirement 6

**Test type**: Automated

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
noSchemaLocation <a name="noSchemaLocation"/>  |  XML document '$filename':  The root element does not have an xsi:schemaLocation attribute. The document cannot be validated.
invalidSchema <a name="invalidSchema"/>  |  XML document '$filename':  The document is not valid. The XML parser has identified the following issues: $issues

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
schemaLocation <a name="schemaLocation"></a>   | /*[@xsi:schemaLocation]
