# Spatial Representation Type

**Purpose**: Verify that the identifier(s) of the spatial representation type(s) used in the data set have been created, taken from the list of allowed values and published in the metadata for the data set.

**Prerequisites**

**Test method**

Inspect the data set metadata whether metadata describing the spatial representation type(s) have been created and published in [spatialRepresentationType](#spatialRepresentationType).

Verify that each value is one of the [valid values](#validvalues).

**Reference(s)**	 

* [TG_DS_TMPL](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/README#ref_TG_DS_TMPL), TG requirements 4 and 5 

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/README#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
<a name="spatialRepresentationType"></a> spatialRepresentationType | gmd:identificationInfo/gmd:MD_DataIdentification/gmd:spatialRepresentationType/gmd:MD_SpatialRepresentationTypeCode/@codeListValue
<a name="validvalues"></a> valid values | doc(http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/gmxCodelists.xml)//gmx:CodeListDictionary[@gml:id='MD_SpatialRepresentationTypeCode']//gml:identifier/text()
