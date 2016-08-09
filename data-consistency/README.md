# Conformance class: Data consistency (DRAFT)

Conformance class for the requirements related to the consistency of the data.

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "INSPIRE GML application schemas".

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

none

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS Template](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/data-consistency/README#ref_TG_DS_tmpl) | [INSPIRE GML application schemas](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas) | INSPIRE spatial data set encoded in GML | n/a |
 
## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-HY](#ref_TG_DS_HY)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Version consistency](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/data-consistency/versions)  | ready for review  | A.3.1, A.3.2, A.3.3 |
| [Temporal consistency](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/data-consistency/temporal)  | ready for review  | A.3.4  |

Note: Additional data consistency test cases will be defined per data theme, where needed.

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
gml            | http://www.opengis.net/gml/3.2
hy-n           | http://inspire.ec.europa.eu/schemas/hy-n/3.0 or http://inspire.ec.europa.eu/schemas/hy-n/4.0
hy-p           | http://inspire.ec.europa.eu/schemas/hy-p/3.0 or http://inspire.ec.europa.eu/schemas/hy-p/4.0

The following variables are used to refer to the corresponding Xpath expressions in all test descriptions:

Variable       | Value
-------------- | -------------------------------------------------
$features      |  //schema-element(hy-n:HydroNode) \| //schema-element(hy-n:WatercourseLink) \| //schema-element(hy-n:WatercourseLinkSequence) \| //schema-element(hy-n:WatercourseSeparatedCrossing) \| //schema-element(hy-p:Watercourse) \| //schema-element(hy-p:StandingWater) \| //schema-element(hy-p:Wetland) \| //schema-element(hy-p:GlacierSnowfield) \| //schema-element(hy-p:Shore) \| //schema-element(hy-p:DrainageBasin) \| //schema-element(hy-p:RiverBasin) \| //schema-element(hy-p:LandWaterBoundary) \| //schema-element(hy-p:Embankment) \| //schema-element(hy-p:Ford) \| //schema-element(hy-p:Lock) \| //schema-element(hy-p:Sluice) \| //schema-element(hy-p:DamOrWeir) \| //schema-element(hy-p:ShorelineConstruction) \| //schema-element(hy-p:Crossing) \| //schema-element(hy-p:SpringOrSeep) \| //schema-element(hy-p:VanishingPoint) \| //schema-element(hy-p:Rapids) \| //schema-element(hy-p:Falls)
