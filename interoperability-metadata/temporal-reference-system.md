# Temporal Reference System

**Purpose**: Verify whether the temporal reference system(s) used in the data set have been created and published in the metadata for the data set, if the spatial data set contains temporal information that does not refer to the default temporal reference system.

**Prerequisites**

**Test method**

Inspect the spatial data set to determine whether it contains temporal information that does not refer to the Gregorian Calendar, the default temporal reference system.

If this is the case, inspect the data set metadata whether metadata describing the temporal reference system(s) has been created and published using the code property in [RS_Identifier](#rs). Note that currently no guidance exists regarding the identifiers for temporal reference systems.

**Reference(s)**	 

* [ISO 19108](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/README#ref_ISO_19108), 5.3.1
* [TG_DS_TMPL](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/README#ref_TG_DS_TMPL), TG requirements 4 and 5 

**Test type**: Manual

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/README#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
rs <a name="rs"></a>   | gmd:referenceSystemInfo/gmd:MD_ReferenceSystem/gmd:referenceSystemIdentifier/gmd:RS_Identifier/gmd:code/gco:CharacterString
