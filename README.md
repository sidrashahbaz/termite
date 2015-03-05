Terminology Service
=======

Overview
--------

For the access of hetrogenous terminological content from common platform we have developed a UTS (Unified Terminology Service) model using CTS2 (HL7 standard) and SKOS. We have CTS2 conceptual model over the SKOS model. Some of the properties were directly mapped over SKOS, but some properties of CTS2 were added as an extension of SKOS. The following table shows the mapping of CTS2 over SKOS:

| **CTS2**        | **SKOS**                      |     
|-----------------|-------------------------------|
CodeSystem | ConceptScheme
Concept | Concept
ValueSet | Collection
DesignationType | prefLabel,altLabel,hiddenLabel
Designation | literal
Description | note
CodeSystemEntityVersionAssociation | semanticRelation
CodeSystemEnity | rdfs:resource
ConceptValueSetMemberShip | member
AssociationType | mappingRelation,related,broader,broaderTransitive,narrower,narrowerTransitive
Name | rdfs:label

The UTS model as an extension of SKOS is shown in figure below

![uts](https://cloud.githubusercontent.com/assets/4283040/6510893/d9ff30a8-c38a-11e4-8db2-e3d103b0e375.jpg)
