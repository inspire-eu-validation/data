# Temporal reference systems

**Version**: 1

**Purpose**: Verify that all references to temporal coordinate reference systems are using one of the http URIs approved for use in INSPIRE data sets.

**Prerequisites**

**Test method**

* Verify that all references to coordinate reference systems in the features use one of the approved http URIs, i.e. check that all references to coordinate reference systems in the [frame](#frame) XML attributes in the [features](#features) use the URI 'http://www.opengis.net/def/trs/ISO-8601/'. Otherwise report [unknownTRS](#unknownTRS). 

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/reference-systems/README#ref_TG_DS_tmpl) IR requirement Article 11 (1)

**Test type**: Automated

**Notes**

All values in the XML Schema date/time types are automatically in the required reference system.

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
unknownTRS <a name="unknownTRS"/>  |  XML document '$filename', $featureType '$gmlid': A temporal geometry uses an unexpected coordinate reference system '$trs'. Only 'http://www.opengis.net/def/trs/ISO-8601/' is allowed.

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-hy/3.1/hy-n-rs/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
frame <a name="frame"></a>   | $features//gml:TimeInstance/@frame \| $features//gml:TimeInstance/gml:timePosition/@frame \| $features//gml:TimePeriod/@frame \| $features//gml:TimePeriod/gml:beginPosition/@frame \| $features//gml:TimePeriod/gml:endPosition/@frame