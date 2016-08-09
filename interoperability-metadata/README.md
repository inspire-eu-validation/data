# Conformance class: Metadata for interoperability

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3).

## Standardization target type

ISO 19115/19119 metadata record

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the metadata record, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [INSPIRE Metadata Implementing Rules: Technical Guidelines based on EN ISO 19115 and EN ISO 19119](#ref_TG_MD) | [XML encoding](http://inspire.ec.europa.eu/id/ats/metadata/1.3/iso-19115-19119) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [INSPIRE Metadata Implementing Rules: Technical Guidelines based on EN ISO 19115 and EN ISO 19119](#ref_TG_MD) | [XML encoding](http://inspire.ec.europa.eu/id/ats/metadata/1.3/xml-encoding) | XML document (MD_Metadata) |  `encoding` = `ISO/TS 19139` or `CSW ISO AP 1.0.0` |

## External document references

| Abbreviation | Document name                       |
| ------------ | ----------------------------------- |
| IR IOP <a name="ref_IR_IOP"><a/> | [COMMISSION REGULATION (EU) No 1089/2010 of 23 November 2010 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards interoperability of spatial data sets and services](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=OJ:L:2010:323:FULL&from=EN)
| IR IOP AMD <a name="ref_IR_IOP_AMD"></a> | [COMMISSION REGULATION (EU) No 1253/2013 of 21 October 2013 amending Regulation (EU) No 1089/2010 implementing Directive 2007/2/EC as regards interoperability of spatial data sets and services](http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=OJ:L:2013:331:0001:0267:EN:PDF)
| TG DS TMPL <a name="ref_TG_DS_TMPL"></a> | [INSPIRE Data Specifications Template, version 3.0rc3](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)
| ISO 19108 <a name="ref_ISO_19108"></a> | [ISO 19108 Geographic information - Temporal schema](http://www.iso.org/iso/catalogue_detail.htm?csnumber=26013)

## Tests

This Conformance Class contains the following tests:

| Identifier                                                        | Origin | Automated | Status   |
| ----------------------------------------------------------------- | ------ | ---------- | -------- |
| [Coordinate Reference System](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/coordinate-reference-system)     | [IR IOP](#ref_IR_IOP), [TG DS TMPL](#ref_TG_DS_IMPL)     |  Yes          | Ready for review    |
| [Temporal Reference System](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/temporal-reference-system)         | [IR IOP](#ref_IR_IOP), [TG DS TMPL](#ref_TG_DS_IMPL)     |  No          | Ready for review    |  
| [Encoding](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/encoding)                             				| [IR IOP](#ref_IR_IOP), [TG DS TMPL](#ref_TG_DS_IMPL)     |  Yes          | Ready for review    |
| [Topological Consistency](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/topological-consistency)             | [IR IOP](#ref_IR_IOP), [TG DS TMPL](#ref_TG_DS_IMPL)     |  No          | Ready for review    |
| [Character Encoding](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/character-encoding)                   	| [IR IOP](#ref_IR_IOP), [TG DS TMPL](#ref_TG_DS_IMPL)     |  Yes          | Ready for review    |  
| [Spatial Representation Type](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/spatial-representation-type)     | [IR IOP AMD](#ref_IR_IOP_AMD), [TG DS TMPL](#ref_TG_DS_IMPL)  | Yes           | Ready for review    |  

## Open issues

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix   | Namespace
-------- | -------------------------------------------------
gmx      | http://www.isotc211.org/2005/gmx
gmd      | http://www.isotc211.org/2005/gmd
gco      | http://www.isotc211.org/2005/gco
gml      | http://www.opengis.net/gml/3.2
