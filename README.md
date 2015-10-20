ats-interoperability-metadata
=============================

Abstract Test Suite for additional metadata elements included in INSPIRE Implementing Rules on the Interoperability of Spatial Datasets and Services (Commission Regulation (EU) No 1089/2010) and in the Data Specifications Technical Guidelines for the Annex I-III spatial data themes.

*Note*: This ATS is in Ready for review stage, none of the tests have an official INSPIRE MIG approval.

## External document references

| Abbreviation | Document name                       |
| ------------ | ----------------------------------- |
| IR IOP <a name="ref_IR_IOP"><a/> | [COMMISSION REGULATION (EU) No 1089/2010 of 23 November 2010 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards interoperability of spatial data sets and services](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=OJ:L:2010:323:FULL&from=EN)
| IR IOP AMD <a name="ref_IR_IOP_AMD"></a> | [COMMISSION REGULATION (EU) No 1253/2013 of 21 October 2013 amending Regulation (EU) No 1089/2010 implementing Directive 2007/2/EC as regards interoperability of spatial data sets and services](http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=OJ:L:2013:331:0001:0267:EN:PDF)
| TG DS TMPL <a name="ref_TG_DS_TMPL"></a> | [INSPIRE Data Specifications Template, version 3.0](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)
| ISO 19108 <a name="ref_ISO_19108"></a> | [ISO/DIS 19108 Geographic information - Temporal schema](http://www.iso.org/iso/catalogue_detail.htm?csnumber=26013)

## Tests

This Conformance Class contains the following tests:

| Identifier                                                        | Origin | Mechanical | Status   |
| ----------------------------------------------------------------- | ------ | ---------- | -------- |
| [A.01.IR13.1.crs](A.01.IR13.1.crs.md)                             | [IR IOP](#ref_IR_IOP)     |  Yes          | Ready for review    |  
| [A.02.IR13.2.trs](A.02.IR13.2.trs.md)                             | [IR IOP](#ref_IR_IOP)     |  No          | Ready for review    |  
| [A.03.IR13.3.enc](A.03.IR13.3.enc.md)                             | [IR IOP](#ref_IR_IOP)     |  Partial          | Ready for review    |  
| [A.04.IR13.4.topo](A.04.IR13.4.topo.md)                           | [IR IOP](#ref_IR_IOP)     |  Partial          | Ready for review    |  
| [A.05.IR13.5.char.enc](A.05.IR13.5.char.enc.md)                   | [IR IOP](#ref_IR_IOP)     |  Yes          | Ready for review    |  
| [A.06.IR13.6.spat.rep](A.06.IR13.6.spat.rep.md)                   | [IR IOP AMD](#ref_IR_IOP_AMD)  | Yes           | Ready for review    |  

## Open issues

* Test scope: Should the tests just check if the required metadata elements are correctly given, or that they also match the features of reported data sets?
* These test cover recommendations, not requirements. These recommendations are listed in [TG DS TMPL](#ref_TG_DS_TMPL), section 8 "Dataset-level metadata", and thus included in each of the INSPIRE Data Specification documents.

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix   | Namespace
-------- | -------------------------------------------------
gmd      | http://www.isotc211.org/2005/gmd
wfs      | http://www.opengis.net/wfs/2.0
