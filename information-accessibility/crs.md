# CRS

**Version**: 1

**Purpose**: Verify that referenced coordinate reference systems can be accessed.

**Prerequisites**

**Test method**

* Verify that any coordinate reference system is publicly accessible via HTTP, i.e. inspect links to coordinate reference systems. Verify that a HTTP GET request to the URI of each unique link ([srsName1](#srsName1), [srsName2](#srsName2), [frame](#frame)) retrieves a document. Otherwise report [brokenLink](#brokenLink).

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/information-accessibility/README#ref_TG_DS_tmpl) IR requirement Section 1.3.4
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/information-accessibility/README#ref_TG_DS_tmpl) IR requirement Section 1.5.1
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/information-accessibility/README#ref_TG_DS_tmpl) IR requirement Section 1.5.2

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': A spatial or temporal geometry uses an unexpected coordinate reference system with identifier '$rsid' that cannot be retrieved. Every URI must be a HTTP URI in a CRS register that when retrieved with HTTP GET returns a definition of the reference system.

## Contextual XPath references

The namespace prefixes and variable references are specified in [README.md](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/information-accessibility/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
frame <a name="frame"></a>   | $features//gml:TimeInstance/@frame \| $features//gml:TimeInstance/gml:timePosition/@frame \| $features//gml:TimePeriod/@frame \| $features//gml:TimePeriod/gml:beginPosition/@frame \| $features//gml:TimePeriod/gml:endPosition/@frame
srsName1 <a name="srsName1"></a>   | $features//@srsName
srsName2 <a name="srsName2"></a>   | //wfs:boundedBy/\*/@srsName or //gml:boundedBy/\*/@srsName
