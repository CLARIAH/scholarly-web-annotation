# Background for the Scholarly Web Annotation approach

[Scenarios](#scenarios) / [Use cases](#usecases) / [Requirements](#requirements) / [Ontology](#ontology) / [Data model](#datamodel) / [Challenges](#challenges) / [Workflow](#workflow)



## <a name="scenarios"></a>Scenarios

Scholarly annotation scenarios (forthcoming)

## <a name="usecases"></a>Use cases

Scholarly annotation scenarios (forthcoming)

## <a name="requirements"></a>Requirements

(Preliminary, more information will be added soon). 

To get a broader view of future requirements for querying and filtering annotations, the proposals of the [CLARIAH WP5 research pilots](http://www.clariah.nl/projecten/research-pilots) have been analysed and a rough estimate of their annotation tasks and querying requirements are listed below:

- [CrossEWT](http://www.clariah.nl/projecten/research-pilots/crossewt): historical development of eye-witness testimonies of WWII
  - manually annotate testimonies, use manual annotations to bootstrap automtatic recognition, extraction, annotation
  - query automatic annotations for manual verification
- [DReAM](http://www.clariah.nl/projecten/research-pilots/dream): cross-media analysis of trajectories of drugs and regulations
  - annotate mentions of drug components in broadcast media
  - query for annotations based on annotation bodies (types, values)
- [Me and Myself](http://www.clariah.nl/projecten/research-pilots/m-m): trace emergence of a genre based on analysis of cues related to genre conventions
  - annotation of oral and visual cues in video (bottom-up coding)
  - annotate video stream of TV broadcasts in combination with TV program guides
  - querying for free-form tags and batch-updating them with more controlled codes
  - querying codes in combination with resource metadata for analysis
- [MIMEHIST](http://www.clariah.nl/projecten/research-pilots/mimehist): annotate video stream of films in combination with film posters, photos and distribution data
  - querying annotations via bodies in combination with resource metadata 
  - querying annotations via creator, date and tags
- [NarDis](http://www.clariah.nl/projecten/research-pilots/nardis): analysing narrative constructing during exploratory search
  - exploring linked data collections, generating paths/trails of entities,  and generating narratives based on the relations between entities along the paths using annotations.
  - building trails of entities related to disruptive media events, annotate relations between entities, compare trails via annotations and entities
  - querying for annotations based on arbitrary sets of resources

## <a name="ontology"></a>The Scholarly Web Annotation Ontology

The Scholarly Web Annotation client uses RDFa reason about the page it is annotating. A page can use any Semantic Web ontology to describe itself, but for some specific scholarly goals, there is an annotation ontology that the client can use for special functionalities. 

The Scholarly Web Annotation Ontology (SWAO) extends the FRBRoo and CIDOC-CRM ontologies, so that scholars can differentiate between conceptual levels of the resources presented on a page and choose which level they want to annotate. E.g. it is possible to describe a resource both at the level of a work, or a specific manifestation or expression of it. For instance, when annotating a letter that is part of correspondence, scholars may want to annotate a phrase in the text to say something about the letter in general, or about some aspect of the specific transcription or translation.

The FRBRoo ontology is very extensive, and in many cases only a few of the concepts will be relevant, so we demonstrate how our SWA Ontology connects to some of the basic concepts of FRBRoo related to *Works*.

[Read more...](https://github.com/CLARIAH/scholarly-web-annotation-client/blob/master/docs/annotation_ontology.md)

## <a name="datamodel"></a>Data model

The Annotation client uses the W3C Web Annotation model as the basis for the annotations.

[Read more...](https://github.com/CLARIAH/scholarly-web-annotation-client/blob/master/docs/data_models.md)

## <a name="challenges"></a>Challenges

- [Handling permissions](https://clariah.github.io/scholarly-web-annotation-client/docs/discussion/handling-permissions.html): scholars want control over who has access to their annotations. Some annotations should remain private and only accessible to their creator, some should be shared with collaborators and some should be public, so that they can be referenced in publication or reused by others.

## <a name="workflow"></a>Workflow

(Forthcoming)



*(Last update: May 27, 2019)*