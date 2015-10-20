
# Character Encoding

**Purpose**

The character encoding used in the dataset.
This element is mandatory only if an encoding is used that is not based on UTF-8.

**Test method**

Grab the resource. Check the encoding. If the resource is not encoded based on UTF-8, validate if the appropriate encoding is provided in [CharEnc](#CharEnc)
Not applicable to services

**Reference(s)**	 

* [IR IOP](./README.md#ref_IR_IOP), Art 13 - 5

**Test type:** Automated

**Notes**

**Contextual XPath references**

The namespace prefixes used as described in [README.md](./README.md#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
<a name="CharEnc"></a> CharEnc | gmd:identificationInfo\gmd:MD_DataIdentification\gmd:characterSet\gmd:MD_CharacterSetCode@codeListValue
