Target: [Int. J. on Software Tools for Technology Transfer -
Special Section on Scientific Workflows](http://www.cs.stir.ac.uk/~kjt/research/sttt-workflows.html)

# Introduction

This article desribes the next
major version of our [Taverna workflow system](http://www.taverna.org./uk/), 
in particular focusing on its workflow language SCUFL2 and the abstract semantic
workflow model wfdesc.

The [SCUFL2 API](https://github.com/taverna/taverna-scufl2/) 
allows construction and inspection of Taverna 3
workflows from independent applications, but also enables translation
from/to different abstract and concrete third-party workflow formats
(SHIWA [8] IWIR, MG-RAST [9] AWE).

This includes the general semantic model wfdesc [3] which we have
created within the Wf4Ever project [4] for the purpose of workflow
preservation and annotation. wfdesc is easily combined with W3C
PROV-based workflow provenance [5], and is also used by the digital
preservation project SCAPE [6] to find and compose semantically
described Workflow Components from the myExperiment [7] workflow
repository.




[3] http://purl.org/wf4ever/model#wfdesc
[4] http://www.wf4ever-project.org/
[5] http://purl.org/wf4ever/model#wfprov
[6] http://www.scape-project.eu/
[7] http://www.myexperiment.org/
[8] http://www.shiwa-workflow.eu/
[9] http://blog.metagenomics.anl.gov/