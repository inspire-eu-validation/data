# Spatial reference systems

**Version**: 1

**Purpose**: Verify that all references to spatial coordinate reference systems are using one of the http URIs approved for use in INSPIRE data sets.

**Prerequisites**

**Test method**

* Verify that all references to coordinate reference systems in the features ([srsName1](#srsName1)) use one of the approved [crsuris](#crsuris) listed in the INSPIRE coordinate reference systems register (https://inspire.ec.europa.eu/crs), otherwise report [unknownCRS1](#unknownCRS1). 
* Verify that all references to coordinate reference systems in the bounding box of the feature collection ([srsName2](#srsName2)) use one of the [crsuris](#crsuris) listed in the INSPIRE coordinate reference systems register (https://inspire.ec.europa.eu/crs). Otherwise report [unknownCRS2](#unknownCRS2).

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/reference-systems/README#ref_TG_DS_tmpl) IR requirement Section 1.2
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/reference-systems/README#ref_TG_DS_tmpl) IR requirement Section 1.3
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/reference-systems/README#ref_TG_DS_tmpl) IR requirement Section 1.5 (1)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/reference-systems/README#ref_TG_DS_tmpl) IR requirement Section 1.5 (2)
* TG Requirement 2 of all Data Specifications

**Test type**: Automated

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
unknownCRS1 <a name="unknownCRS1"/>  |  XML document '$filename', $featureType '$gmlid': A spatial geometry uses an unexpected coordinate reference system '$crs'. Please refer to the INSPIRE coordinate reference systems register (https://inspire.ec.europa.eu/crs) for the list of expected coordinate reference systems.
unknownCRS2 <a name="unknownCRS2"/>  |  XML document '$filename': The default coordinate reference system stated in the bounding box of the feature collection has an unexpected value '$crs'. Please refer to the INSPIRE coordinate reference systems register (https://inspire.ec.europa.eu/crs) for the list of expected coordinate reference systems.

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/reference-systems/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
srsName1 <a name="srsName1"></a>   | $features[.//@srsName[not(. = $crsuris)]]
srsName2 <a name="srsName2"></a>   | //wfs:boundedBy/\*/@srsName[not(. = $crsuris)] or //gml:boundedBy/\*/@srsName[not(. = $crsuris)]]
crsuris <a name="crsuris"></a>     | All valid HTTP URI identifiers are available in the INSPIRE coordinate reference systems register (https://inspire.ec.europa.eu/crs)
