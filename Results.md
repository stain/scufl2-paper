# Results

## SCUFL2 Workflow Bundle

* A ZIP file that contains several files that together define the workflow to execute
  * One file per (nested) workflow
  * Workflow Bundle document that ties together
    * "Main workflow" and "Preferred profile"
* Profiles for choosing implementation activity and configurations
  * Separate file per profile
  * Separate file per configuration 
    * Can be shared across profiles 
* JSON-LD based configurations - flexible for each activity
* XML schemas for workflow structure files
  * structured XML that can be validated
  * ..also parseable as RDF/XML
* Everything has a URI
  * Unique UUID-based identifier pr workflow version
  * Declared relative within ZIP - but can be made absolute
  * Annotation target for any workflow object
  * [URI service](http://guess.taverna.org.uk/) - minimally describe any worfklow component
 

## SCUFL2 API

* Java API for programmatically loading, saving and creating SCUFL2 Workflow Bundles
* Each workflow element is a Java bean
* Support for load/save different formats, scufl1, t2flow, wfbundle, [wfdesc](https://github.com/apache/incubator-taverna-language/tree/master/taverna-scufl2-wfdesc), [shiwa-iwir](https://github.com/stain/scufl2-iwir)

## wfdesc

* Abstract workflow language that only deals with the pipeline
* Easier to query 
* Hooks for annotation on a Research Object level
* Hooks for describing provenance of workflow run
* Same identifiers as in SCUFL2
* Not complete enough for execution - no control logic or iteration
* Inspiration for Commons workflow language

## Common Workflow Language

* Work in progress
* Definition for executable workflow language across bioinformatics workflow systems.
* Specifies how to invoke command line tools
* Dataflow-driven

## RO Bundle

* Evolution from UCF container to RO bundle
  * Details how to describe metadata, provenance and annotations 
* Formal specification: https://w3id.org/bundle
  * To be proposed as an RFC
* A wfbundle is also a ro bundle
  * how to store annotations

### Databundle

Workflow results can be stored as a [DataBundle](https://github.com/apache/incubator-taverna-language/tree/master/taverna-databundle) - extension of robundle.

Used for provenance of workflow runs -
https://github.com/taverna/taverna-prov#structure-of-exported-provenance

Databundle contains a wfbundle

TODO: Can a wfbundle contain/also be a databundle for example input/output/run?

