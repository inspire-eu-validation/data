# Version consistency

**Version**: 1

**Purpose**: Verify that the information about a spatial object is consistent over time.

**Prerequisites**

**Test method**

Automated assertions:

* Verify that all endLifespanVersion values are from the allowed range.
  * For all [features](#features) verify that either
    * [beginLifespanVersion](#beginLifespanVersion) or [endLifespanVersion](#endLifespanVersion) are missing or nil or
    * [endLifespanVersion](#endLifespanVersion) is not before the value of [beginLifespanVersion](#beginLifespanVersion).
  * Otherwise report [endTooEarly](#endTooEarly).

Manual assertions:

* Verify that identifiers are persistent for a spatial object, i.e. inspect the documentation of the spatial data set and verify that rules for identifiers are specified in a way that the identifiers (namespace and localId) do not change during the life-cycle of a spatial object. If older versions of the data set are available compare the features and verify that the namespace and localId part of the INSPIRE identifiers have not changed between the versions.
* Verify that the type of a spatial object is unchanged for different versions, i.e. inspect the documentation of the spatial data set and verify that rules for the mapping to the INSPIRE application schema are specified in a way that the spatial object type do not change during its life-cycle. If older versions of the data set are available compare the features and verify that the types of the features has not changed between the versions.

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/data-consistency/README#ref_TG_DS_tmpl) IR requirement Article 9 (2)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/data-consistency/README#ref_TG_DS_tmpl) IR requirement Article 10 (3)

**Test type**: Automated/Manual

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
endTooEarly <a name="endTooEarly"/>  |  XML document '$filename', $featureType '$gmlid': The lifespan of the feature ends before it begins (property 'endLifespanVersion': '$end', property 'beginLifespanVersion': '$begin'). This is logically incorrect.

## Contextual XPath references

The namespace prefixes and variable references are specified in [README.md](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/data-consistency/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
beginLifespanVersion <a name="beginLifespanVersion"></a>   | $features/\*[local-name()='beginLifespanVersion']
endLifespanVersion <a name="endLifespanVersion"></a>   | $features/\*[local-name()='endLifespanVersion']
