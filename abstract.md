Authors: Stian Soiland-Reyes, David Withers, Alan R Williams, Donal Fellows, Carole Goble


This article describes the workflow language of 
[Apache Taverna](http://taverna.incubator.apache.org/) \cite{Wolstencroft_2013},
in particular focusing on its workflow language _SCUFL2_ and the abstract semantic
workflow model _wfdesc_. 

The [SCUFL2 API](https://github.com/taverna/taverna-scufl2/) \cite{3721cfa2-edd7-43f1-825a-6b5044f0d0db}
allows construction and inspection of Taverna 3
workflows from independent applications, but also enables translation
from/to different abstract and concrete third-party workflow formats
([SHIWA](http://www.shiwa-workflow.eu/) IWIR,
[MG-RAST](http://blog.metagenomics.anl.gov/) AWE) and the [Common Workflow Language](https://github.com/common-workflow-language/common-workflow-language)

This includes the general semantic model
[wfdesc](http://purl.org/wf4ever/model#wfdesc)
which we have created within the
[Wf4Ever project](http://www.wf4ever-project.org/) \cite{Hettne_2014}
for the purpose of workflow preservation and annotation.
wfdesc is easily combined with W3C PROV-based
[workflow provenance](http://purl.org/wf4ever/model#wfprov),
and is also used by the digital
preservation project [SCAPE](http://www.scape-project.eu/)
to find and compose semantically
described Workflow Components from the [myExperiment workflow
repository](http://www.myexperiment.org/).