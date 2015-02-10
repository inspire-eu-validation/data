
# Spatial Representation Type

**Purpose**	

The method used to spatially represent geographic information.

**Test method**	

Test if a spatialRepresentationType value is used from an appropriate codelist. The values of MD_SpatialRepresentationTypeCode in the scope of the INSPIRE Directive are: vector, grid or tin.

Grab the recource and check the spatial representation. Validate if it matches the advertised representation.

'''
<gmd:spatialRepresentationType>
   <gmd:MD_SpatialRepresentationTypeCode codeList="http://schemas.opengis.net/iso/19139/20070417/resources/Codelist/gmxCodelists.xml" codeListValue="http://schemas.opengis.net/iso/19139/20070417/resources/Codelist/gmxCodelists.xml#vector"></gmd:MD_SpatialRepresentationTypeCode>
</gmd:spatialRepresentationType>
'''

**Reference(s)**	 

* [IR-M2](./README.md#IR-M2), Art 13 - 6

**Test type:** Automated

**Notes**

**Contextual XPath references**

The namespace prefixes used as described in [README.md](./README.md#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
Value | gmd:identificationInfo\gmd:MD_DataIdentification\gmd:spatialRepresentationType\gmd:MD_SpatialRepresentationTypeCode@codeListValue
