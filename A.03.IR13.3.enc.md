
# Encoding

**Purpose**	

Description of the computer language construct(s) specifying the representation of data objects in a record, file, message, storage device or transmission channel.

**Test method**	

The formats and versions of the distributions should be advertised in [distributionFormat](#distributionFormat), eg.

<gmd:distributionFormat>
  <gmd:MD_Format>
    <gmd:name>
      <gco:CharacterString>GML</gco:CharacterString>
    </gmd:name>
    <gmd:version>
      <gco:CharacterString>3.2.1</gco:CharacterString>
    </gmd:version>
  </gmd:MD_Format>
</gmd:distributionFormat>

iso19115 doesn't provide a mechanism to match certain [distributionFormat](#gmd:distributionFormat) to certain [onLine](#onLine) / [offLine](#offLine), so if multiple multiple [onLine](#onLine) elements are provided this test might not be machine testable. 

The test can grab each of the [onLine](#onLine). If the [onLine](#onLine) is of type WMS, WFS, SOS, WCS or Atom, this call will return a capabilities document advertising the available output formats. If the [onLine](#onLine) links to some other type of resource, the format may be deduced from the downloaded resource. The list of advertised distributionFormats should match with the available formats.

Note that a certain distributionFormat might be available as [offLine](#offLine) only.
 
The result of this test will be "success" or "non-machine-testable".

**Reference(s)**	 

* [IR](./README.md#IR), Art 13 - 3

**Test type:** Automated/Manual

**Notes**

**Contextual XPath references**

The namespace prefixes used as described in [README.md](./README.md#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
distributionFormat <a name="distributionFormat"></a>   | gmd:distributionInfo/gmd:MD_Distribution/gmd:distributionFormat
onLine <a name="onLine"></a>   | gmd:distributionInfo/gmd:MD_Distribution/gmd:transferOptions/gmd:MD_DigitalTransferOptions/gmd:onLine
offLine <a name="onLine"></a>   | gmd:distributionInfo/gmd:MD_Distribution/gmd:transferOptions/gmd:MD_DigitalTransferOptions/gmd:offLine