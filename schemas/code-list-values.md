# Code list values

**Version**: 1

**Purpose**: Verify whether all attributes whose value type is a code list take the values set out therein

**Prerequisites**

**Test method**

When an attribute has a code list as its type, verify that the values comply with the definitions and include the values set out in Annex II of the regulation. To pass this tests that any instance of an attribute

* takes only values explicitly specified in the INSPIRE code list register when the code list‘s extensibility is 'none'.

Otherwise report [disallowedCodeListValue](#disallowedCodeListValue).

For the commonly used data types, the following properties have to be tested:
* [Nativeness (v3)](#Nativeness3) in GeographicalName. Valid values:
  * endonym
  * exonym
* [Nativeness (v4)](#Nativess4) in GeographicalName. Valid values:
  * http://inspire.ec.europa.eu/codelist/NativenessValue/endonym
  * http://inspire.ec.europa.eu/codelist/NativenessValue/exonym
* [NameStatus (v3)](#NameStatus3). Valid values:
  * official
  * standardised
  * historical
  * other
* [NameStatus (v4)](#NameStatus4) in GeographicalName. Valid values:
  * http://inspire.ec.europa.eu/codelist/NameStatusValue/historical
  * http://inspire.ec.europa.eu/codelist/NameStatusValue/official
  * http://inspire.ec.europa.eu/codelist/NameStatusValue/other
  * http://inspire.ec.europa.eu/codelist/NameStatusValue/standardised
* [GrammaticalGender (v3)](#GramGender3) in GeographicalName. Valid values:
  * common
  * feminine
  * masculine
  * neuter
* [GrammaticalGender (v4)](#GramGender4) in GeographicalName. Valid values:
  * http://inspire.ec.europa.eu/codelist/GrammaticalGenderValue/common
  * http://inspire.ec.europa.eu/codelist/GrammaticalGenderValue/feminine
  * http://inspire.ec.europa.eu/codelist/GrammaticalGenderValue/masculine
  * http://inspire.ec.europa.eu/codelist/GrammaticalGenderValue/neuter
* [GrammaticalNumber (v3)](#GramNumber3) in GeographicalName. Valid values:
  * dual
  * plural
  * singular
* [GrammaticalNumber (v4)](#GramNumber4) in GeographicalName. Valid values:
  * http://inspire.ec.europa.eu/codelist/GrammaticalNumberValue/dual
  * http://inspire.ec.europa.eu/codelist/GrammaticalNumberValue/plural
  * http://inspire.ec.europa.eu/codelist/GrammaticalNumberValue/singular
  
The following is not applicable here as no extensions are allowed. It is still included here as a reminder in case extensions will be allowed in the future:

Inspect the code list valued property elements. If a value is not one of the values listed above, review the code list definition to check that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule and that all extensions conform to the requirements. This is a manual test.
  
**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 4 (1)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 4 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 6 (1)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 6 (2)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 6 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#ref_TG_DS_tmpl) IR requirement Article 6 (4)

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
disallowedCodeListValue <a name="disallowedCodeListValue"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that is not one of the allowed values listed at $codelist. 

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
Nativeness (v3) <a name="Nativeness3"></a>   | //schema-element(gn3:GeographicalName)/gn3:nativeness/text()
Nativeness (v4) <a name="Nativeness4"></a>   | //schema-element(gn:GeographicalName)/gn:nativeness/@xlink:href
NameStatus (v3) <a name="NameStatus3"></a>   | //schema-element(gn3:GeographicalName)/gn3:nameStatus/text()
NameStatus (v4) <a name="NameStatus4"></a>   | //schema-element(gn:GeographicalName)/gn:nameStatus/@xlink:href
Grammatical Gender (v3) <a name="GramGender3"></a>   | //schema-element(gn3:GeographicalName)/gn3:grammaticalGender/text()
Grammatical Gender (v4) <a name="GramGender4"></a>   | //schema-element(gn:GeographicalName)/gn:grammaticalGender/@xlink:href
Grammatical Number (v3) <a name="GramNumber3"></a>   | //schema-element(gn3:GeographicalName)/gn3:grammaticalNumber/text()
Grammatical Number (v4) <a name="GramNumber4"></a>   | //schema-element(gn:GeographicalName)/gn:grammaticalNumber/@xlink:href
