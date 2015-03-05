Terminology Service
=======

Overview
--------

For the access of hetrogenous terminological content from common platform we have developed a UTS (Unified Terminology Service) model using CTS2 (HL7 standard) and SKOS. We have CTS2 conceptual model over the SKOS model. Some of the properties were directly mapped over SKOS, but some properties of CTS2 were added as an extension of SKOS. The UTS model is shown in figure below

![alt tag](https://github.com/semr/neo4jena/raw/master/doc/image/sample.PNG)

Neo4Jena is a property graph model interface. It provides the mapping of RDF to property graph (Neo4J) using Jena API.  The main work focuses on how RDF triple is converted to Neo4j graph and vice versa. After the successful loading of RDF in graph we retrieve the data using SPARQL.  We made the following contributions:
* Firstly RDF triples (subject, predicate and object) are converted to Neo4j node and relationship. 
* After the conversion, it store triples in Neo4j graph.
* After the successful loading of RDF triples in graph Neo4Jena retrieve the data using SPARQL. For this neo4j nodes and relationship is converted to RDF triples (subject, predicate and object).
* Neo4Jena has full support of SPARQL 1.1.
