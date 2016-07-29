# Character Encoding

**Purpose**: Verify that the identifier(s) of the character encoding(s) used in the data set have been created and published in the metadata for the data set. This element is mandatory only if an encoding is used that is not based on UTF-8.

**Prerequisites**

**Test method**

For each value of [Character Encoding](#CharEnc) in the data set metadata, test that the value is one of the [valid character encodings](#CharEnc).

**Reference(s)**	 

* [TG_DS_TMPL](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/README#ref_TG_DS_TMPL), TG requirements 4 and 5 

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/README#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
<a name="CharEnc"></a> Character Encoding | gmd:identificationInfo/gmd:MD_DataIdentification/gmd:characterSet/gmd:MD_CharacterSetCode/@codeListValue
<a name="ValidCharEnc"></a> valid character encodings | doc(http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml)//gmx:ML_CodeListDictionary[@gml:id='MD_CharacterSetCode']//gml:identifier/text()
