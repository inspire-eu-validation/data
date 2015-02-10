
# Spatial Representation Type

**Purpose**	

The method used to spatially represent geographic information.

**Test method**	

Test if a spatialRepresentationType value is used from an appropriate codelist

'''
<gmd:spatialRepresentationType>
   <gmd:MD_SpatialRepresentationTypeCode codeList="http://schemas.opengis.net/iso/19139/20070417/resources/Codelist/gmxCodelists.xml" codeListValue="http://schemas.opengis.net/iso/19139/20070417/resources/Codelist/gmxCodelists.xml#vector"></gmd:MD_SpatialRepresentationTypeCode>
</gmd:spatialRepresentationType>
'''

The INSPIRE extentsion to iso19115 defines subclasses for MD_SpatialRepresentation, eg. MD_VectorSpatialRepresentation and MD_GridSpatialRepresentation. I'm not sure if this is relevant for this test.

**Reference(s)**	 

* [IR](./README.md#IR), Art 13 - 6

**Test type:** Automated

**Notes**

**Contextual XPath references**

The namespace prefixes used as described in [README.md](./README.md#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------

