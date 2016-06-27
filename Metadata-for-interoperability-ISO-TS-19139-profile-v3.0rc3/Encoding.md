# Encoding

**Purpose**

Verify that the encoding (i.e., the description of the computer language construct that specifies the representation of data objects in a record, file, message, storage device or transmission channel) used in the data set have been created and published in the metadata for the data set.

**Prerequisites**

* [Schema validation](Schema validation.md)

**Test method**

Inspect the data set metadata whether metadata describing the encoding has been created and published using the code property in [distributionFormat](#distributionFormat).

Verify that the properties [name](#name), [version](#version) and [specification](#specification) are all provided.

**Reference(s)**

* [TG_DS_TMPL](./README.md#ref_TG_DS_TMPL), TG requirements 4 and 5 

**Test type:** Automated

**Notes**

**Contextual XPath references**

The namespace prefixes used as described in [README.md](./README.md#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
distributionFormat <a name="distributionFormat"></a>   | gmd:distributionInfo/gmd:MD_Distribution/gmd:distributionFormat
name <a name="name"></a>   | gmd:distributionInfo/gmd:MD_Distribution/gmd:distributionFormat/gmd:MD_Format/gmd:name/gco:CharacterString
version <a name="version"></a>   | gmd:distributionInfo/gmd:MD_Distribution/gmd:distributionFormat/gmd:MD_Format/gmd:version/gco:CharacterString
specification <a name="specification"></a>   | gmd:distributionInfo/gmd:MD_Distribution/gmd:distributionFormat/gmd:MD_Format/gmd:specification/gco:CharacterString
