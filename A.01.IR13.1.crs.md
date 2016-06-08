# Coordinate Reference System

**Purpose**

Verify that the identifier(s) of the coordinate reference system(s) used in the data set have been created and published in the metadata for the data set.

**Prerequisites**

* [A.00.validate](A.00.validate.md)

**Test method**

Inspect the data set metadata whether metadata describing the coordinate reference system(s) have been created and published using the code property in [RS_Identifier](#rs).

Verify that the value is a http URI and includes one of the values from table 2 in [TG_DS_TMPL](./README.md#ref_TG_DS_TMPL).

Example:

```
<gmd:code>
   <gco:CharacterString>http://www.opengis.net/def/crs/EPSG/0/4258</gco:CharacterString>
</gmd:code>
```

**Reference(s)**

* [IR IOP](./README.md#ref_IR_IOP), Art 13 (1)
* [TG_DS_TMPL](./README.md#ref_TG_DS_TMPL), TG requirements 2, 4 and 5 

**Test type:** Automated

**Notes**

Other attributes may be available in [RS_Identifier](#rs) like gmd:authority, gmd:codeSpace, gmd:version.

**Contextual XPath references**

The namespace prefixes used as described in [README.md](./README.md#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
rs <a name="rs"></a>   | gmd:referenceSystemInfo/gmd:MD_ReferenceSystem/gmd:referenceSystemIdentifier/gmd:RS_Identifier/gmd:code/gco:CharacterString
