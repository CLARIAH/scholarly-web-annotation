# CLARIAH Scholarly Web Annotation (SWA) development

Based on research of scholarly needs, CLARIAH is developing an annotation client and server that will enable scholars to annotate different sources available via the Web, and to store their annotations in CLARIAH. We also work on developing different viewers for annotations of different media types (text, video, images, mixed media) -More information about the viewers will be added soon.

The main developers of the SWA client and server are  [Marijn Koolen](http://marijnkoolen.com/#/) (KNAW Humanities Cluster (HuC)), [Jaap Blom](https://www.clariah.nl/over/wie-is-wie/wp5/jaap-blom) (The Netherlands Institute for Sound and Vision).

## SWA Client

The Scholarly Web Annotation (SWA) client is a Javascript annotation client for RDFa enriched web resources based on the W3C Web Annotation standard. This client is developed by the [Netherlands Institute for Sound and Vision](http://labs.beeldengeluid.nl/) and [Huygens ING](https://www.huygens.knaw.nl/?lang=en) for the research infrastructure project [CLARIAH](https://www.clariah.nl/en/). It is being developed in tandem with the Scholarly Web Annotation Server.

[See the Scholarly Web Annotation Client website and repository in Github](https://clariah.github.io/scholarly-web-annotation-client/)

## SWA Server

Python server for scholarly web annotations. An experimental Python Flask RESTplus server based on the W3C Web Annotation standard, that implements both the [WA data model](https://www.w3.org/TR/annotation-model/) and the [WA protocol](https://www.w3.org/TR/annotation-protocol/). It is developed in tandem with the [Scholarly Web Annotation Client](https://github.com/CLARIAH/scholarly-web-annotation-client) and will eventually be replaced by a proper annotation server.

The server uses [Elasticsearch](https://www.elastic.co/products/elasticsearch) for storage and retrieval of annotations. When running the SWA server, make sure you have a running Elasticsearch instance. Configuration of the Elasticsearch server is done in `settings.py`. This repository contains a file `settings-example.py` that shows how to configure the connection to Elasticsearch. Rename or copy this to `settings.py` to make sure the SWA server can read the configuration file.

[See the Scholarly Web Annotation Server repository in Github](https://github.com/marijnkoolen/scholarly-web-annotation-server).

## Video annotation interoperability expert group (VAINT)

Besides developing the CLARIAH SWA client, server and viewers, see also more implementation-related information about the video annotation interoperability expert group (VAINT) in their [Github repository](https://github.com/CLARIAH/video-annotation-interoperability).



*(Last update: May 27, 2019)*