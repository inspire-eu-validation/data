
# Coordinate Reference System

**Purpose**	

Description of the coordinate reference system(s) used in the data set.

**Test method**	

It is suggested the code attribute in [RS_Identifier](#rs) is inserted as qualified url, eg. 

```
<gmd:code>
   <gco:CharacterString>http://www.opengis.net/def/crs/EPSG/0/4326</gco:CharacterString>
</gmd:code>
```

Other attributes can be available in [RS_Identifier](#rs) like gmd:authority, gmd:codeSpace, gmd:version

If the resource is available to download, the test can grab the file and validate the coordinate 
reference system against the advertised system.

**Reference(s)**	 

* [IR](./README.md#IR), Art 13 - 1

**Test type:** Automated

**Notes**

**Contextual XPath references**

The namespace prefixes used as described in [README.md](./README.md#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
rs <a name="rs"></a>   | gmd:referenceSystemInfo/gmd:MD_ReferenceSystem/gmd:referenceSystemIdentifier/gmd:RS_Identifier
