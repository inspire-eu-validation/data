# Temporal consistency

**Version**: 1

**Purpose**: Verify that the temporal validity of the real-world entity is consistent.

**Prerequisites**

n/a

**Test method**

* For all [features](#features) verify that either
 * [validFrom](#validFrom) or [validTo](#validTo) are missing or nil or
 * [validTo](#validTo) is not before the value of [validFrom](#validFrom).
* Otherwise report [endTooEarly](#endTooEarly).

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/data-consistency/README#ref_TG_DS_tmpl) IR requirement Article 10 (3)

**Test type**: Automated

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
endTooEarly <a name="endTooEarly"/>  |  XML document '$filename', $featureType '$gmlid': The validity of the real-world entity ends before it begins (property 'validTo': '$end', property 'validFrom': '$begin'). This is logically incorrect.

## Contextual XPath references

The namespace prefixes and variable references are specified in [README.md](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/data-consistency/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
validFrom <a name="validFrom"></a>   | $features/\*[local-name()='validFrom']
validTo <a name="validTo"></a>   | $features/\*[local-name()='validTo']
