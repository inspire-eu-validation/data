# Topological Consistency

**Purpose**

Verify whether metadata about the topological consistency of the data set has been created and published in the metadata for the data set, if the spatial data set includes types from the Generic Network Model and does not assure centreline topology (connectivity of centrelines) for the network.

**Prerequisites**

* [A.00.validate](A.00.validate.md)

**Test method**

Inspect the spatial data set to determine whether it includes instances of types from the Generic Network Model and does not assure centreline topology (connectivity of centrelines) for the network.

If this is the case, inspect the data set metadata whether metadata describing the topological consistency has been created and published in [TopologicalConsistency](#topo).

**Reference(s)**	 

* [IR IOP](./README.md#ref_IR_IOP), Art 13 (4)
* [TG_DS_TMPL](./README.md#ref_TG_DS_TMPL), 8.2

**Test type:** Manual

**Notes**

**Contextual XPath references**

The namespace prefixes used as described in [README.md](./README.md#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
TopologicalConsistency <a name="topo></a>	| gmd:dataQualityInfo/gmd:DQ_DataQuality/gmd:report/DQ_TopologicalConsistency/result/DQ_QuantitativeResult/value
