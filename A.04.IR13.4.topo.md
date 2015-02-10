
# Topological Consistency

**Purpose**	

Correctness of the explicitly encoded topological characteristics of the data set as described by the scope.
This element is mandatory only if the data set includes types from the Generic Network Model and does not assure centreline topology (connectivity of centrelines) for the network.

**Test method**	

First check if validation is required. This test would be facilitated if the types that are described in the metadata are added to the metadata. In the curent situation to know which types are described the test should go into the WFS (or Atom) capabilities to find the names of advertised [FeatureType](#FeatureType). It should then match any of those names to a predefined list of types from the Generic Network Model.

Test if data of the type assures centreline topology.

If the element is mandatory, it should be available else the test fails.



If required, check if the appropriate topological consistency is provided in [topo](#topo)

**Reference(s)**	 

* [IR](./README.md#IR), Art 13 - 4

**Test type:** Automated

**Notes**

**Contextual XPath references**

The namespace prefixes used as described in [README.md](./README.md#namespaces).

Abbreviation                                   |  XPath expression (relative to gmd:MD_Metadata)
-----------------------------------------------| -------------------------------------------------------------------------
FeatureType <a name="FeatureType"></a>   | WFS_Capabilities/FeatureTypeList/FeatureType