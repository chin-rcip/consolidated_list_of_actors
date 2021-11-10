---
layout: page
permalink: /en/project-description
title: Project Description
sidebar: project-desc
---

## Description

### Context

The CLA would be a consolidated list of persons or groups of national, historical, or cultural significance *themself* or who have *produced something* that is of national historical, or cultural significance.

The list would be established by extracting relevant data from a series of relevant sources, reconciling this data and making it available as a controlled vocabulary to which contributors can submit new entries (which would be vetted by CHIN based on a series of criteria). 

The provenance of the information listed would be referenced (i.e. where the information was extracted from, or who submitted it) so that its credibility can be assessed by the user.  

The CLA would be available under a CC0 license.

#### Relevance

It would be possible to develop discipline-specific vocabularies (e.g. list of artists, list of architects), but these would:

* Only useful to a handful of stakeholders who have collections solely centered around this discipline (e.g. galleries, architecture center), as opposed to being useful to the sector as a whole (with most institutions having encyclopedic data in some capacity); 
* Have to be developed directly with a single expert institution for each discipline (since mediating between institutions is not part of CHIN’s mandate), thus servicing single institutions rather than the sector as a whole; 
* Rely on legal agreements with stakeholders rather than reuse of factual data already openly available (thus making the burden of maintenance much higher on CHIN, especially at the beginning of the project). 

The absence of a controlled list of actors in Canada is detrimental to their visibility on the web (most notably in major databases such as ULAN or Wikidata, but also in search engine results such as Google). It is also a disservice to Canadian heritage institutions that cannot rely on a standardized list of actors to manage their data (either for cleaning and management purposes, or for cross-institutional use of information). 

#### Benefits

On the contrary, a sector-wide controlled list supports the development of cross-institutional tools that can be mobilized by practitioners regardless of their disciplinary focus, a need that has been mentioned by several stakeholders. This would: 

* Offer a historical portrait of collection practices in Canada when it comes to actors; 
* Establish grounds for representation statistics in the future, once more complete data is available; 
* Be indexed in Google (if developed accordingly), which would contribute to the visibility and reusability of the CLA’s contents; 
* Support the direct adding, updating, querying and use of data by tools and applications (through an API), , contributing to greater visibility of the actors for the general public as well as heritage practitioners.

In addition, should an LOD component be developed as part of the list, it would:

* Facilitate the management of data by offering an interoperable standard for cleaning and reconciling;
* Enhance the visibility of Canadian actors and productions on other international platforms such as ULAN, Wikidata, or ISNI by linking the CLA content with theirs.

These advantages would be most visible in potential uses of the CLA as part of tools and services such as: 

* An integrated feature in content management systems so that the list can be directly used by practitioners;
* An open source data cleaning tool based on the list; 
* An Open Refine extension or service to facilitate heritage data reconciliation; 
* Various statistical and visual analysis tools and services (e.g. how collecting has grown throughout the years in Canada, actors repartition by type across years, etc.);
* A direct access to the database through a SPARQL endpoint and/or API, thus facilitating further research on actors through complex queries.

#### Challenges

Despite the benefits of such a list, it also entails challenges in terms of governance and relationship with stakeholders: 

* The eventual deployment of an entirely new list would require significant resources for the:
   * consultation of relevant communities (heritage, Indigenous, LGBTQIA+, etc.) to ensure adequate representation; 
   * development of agreements with relevant software providers; 
   * development of a communication plan and outreach strategy  to ensure use by practitioners; 
   * allocation of sustained resources for the maintenance of the CLA. 
* CHIN would have three options when it comes to prior lists: 
   * Subsume any priorlist under the CLA (which risks displeasing the owners); 
   * Maintain two parallel lists should the ownersnot want to be a contributor to the list (which risks confusing users in general as to the right list to use); 
   * Release maintenance of any prior listto the ownerswho would hopefully contribute to the CLA nonetheless (which also risks confusing users in general as to the right list to use). 
* Like all heritage datasets, the CLA would contain data whose publication would be sensitive for social or legal reasons. This applies to information that is personal or subject to collective intellectual property (e.g. Indigenous data). Significant resources will thus be necessary to:
   * Identify problematic or sensitive data;
   * Shadow said data until necessary verifications have been made as to whether it can be published or not; 
   * Secure agreements with relevant parties (rights holders, data owners) in view of publication. 
* Because of the consolidated nature of the CLA, CHIN will have to adjudicate the credibility and precedence of information. This imposes a revision of CHIN’s business model from an organization that hosts data to an organization who would have:
   * authority, in some capacity, over data; 
   * responsibility for the maintenance of its contents up to date (through regular enhancements, analysis and potential review of the list’s structure, etc.).
* Because of the precedent the CLA would establish, there might be an expectation from the heritage community that CHIN develop other needed vocabularies (which might be doable and useful, but is not considered at the moment). 

### Anticipated Development

#### Controlled List

As a first step, a prototype of a consolidated list of actors could be done based on a subset of actors data extracted from available datasets. 
Potential sources could include: 

* [Artefacts Canada](https://app.pch.gc.ca/application/artefacts_hum/indice_index.app?lang=en); 
* [Artists in Canada](https://app.pch.gc.ca/application/aac-aic/recherche_base-search_basic.app?lang=en);
* [Dictionary of Canadian Biography](http://www.biographi.ca/en/index.php); 
* [Données Québec](https://www.donneesquebec.ca/recherche/dataset?groups=societe-culture&q=&sort=metadata_created+desc&extras_organisation_principale=); 
* Getty’s [Union List of Artists](http://www.getty.edu/research/tools/vocabularies/ulan/);
* [ISNI](https://isni.org/);
* [VIAF](http://viaf.org/);
* [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page).

Other lists of relevant actors in Canada are available (controlled or not) and could provide data for the CLA. This would have to be investigated further. 

Other current partners could also be involved in the prototype provided agreements on the subject are made. 

In a subsequent pilot project data could either be obtained through agreements, or extracted provided it is available online. There would thus be two types of data retrieval processes: 

* Contribution agreements through which relevant providers submit their datasets for parsing, reconciling and entry into the CLA; 
* Direct extraction from open datasets or APIs. 

Up until this point, no LOD would be involved and the controlled list could be maintained as a “flat” standard (and deployed as such). At this point: 

* Use in CMSs would still be possible pending agreements, although the likelihood of misuse would be higher due to the lack of URIs. 
* Statistical analysis and visualization tools would still be possible, given that a CLA ID would be assigned to each unique actor, to which other external IDs (ULAN, WD, etc.) would be reconciled.
* Canadian collections’ actors presence in international systems would remain low due to a lack of technological automation when it comes to commonly used platforms (e.g. ISNI, ULAN, Wikidata). 

#### LOD Controlled List

A second phase of the project could focus on the creation of URIs (or reuse from other sources such as ULAN if relevant) and mapping to the DOPHEDA Target Model for actors listed in the CLA, and the submission of entries into counterparts’ systems. This could not be done prior to the establishment of a sustainable and robust semantic environment at CHIN (so that once the URIs are created, they are a trusted resource to use). This phase would likely take the following forms: 

* Agreements with CMSs so that the list is available for use by practitioners; 
* Development of an API for direct query of the CLA; 
* Submission of the entries to internationally used standards such as ULAN and Wikidata (either in the context of batch submissions, or through bilateral agreements). 

At this point: 

* CMSs could embed the CLA through the use of API. 
* Statistical analysis and visualizations mobilizing several datasets would be facilitated and tools could be developed to support these.
* Canadian collections’ actors presence in international systems would increase due to the facilitated submission of  entries to and interlinking with relevant platforms (e.g. ISNI, ULAN, Wikidata). 

### Definitions

* Consolidated list: A file containing a list of the names of persons or groups of significance recorded by institutions in Canada. A consolidated list is: 
	* based on the aggregation of the data gathered from various sources; 
	* vetted and organized by a central agency (likely CHIN) in charge or maintenance; 
	* reconciled to ensure all entries are unique and relevant. 
* Actor: Person or group of national, historical, or cultural significance *themself* or who has *produced something* that is of national, historical, or cultural significance. 
* “In Canada”: Determining who qualifies as being part of a list of actors “in Canada” will be one of the trickiest parts of the CLA as many persons and groups relevant to institutions in Canada might not be considered or consider themselves Canadians. Even though this will have to be further investigated, the following criteria can be used as a preliminary basis:
   * related to objects held in heritage collections in Canada;
   * born in what is now considered Canada;
   * identify as Canadian. 

### Statistics about Actors

Analysis of several relevant datasets such as AiC, AC, ISNI, ULAN, Wikidata:

* How many Canadian actors in ULAN and WD?
   * ULAN: 4477 (with Canadian nationality)
   * WD: 87,873
* Are there any Canadian institutions contributing to ULAN or WD? If so, who are they?
	* ULAN: one institution contributing to 2551 entities (Canadian Centre for Architecture)
	* WD: Top 5 Institutions/databases having properties ID and number of entities [link to query](ULAN: one institution contributing to 2551 entities (Canadian Centre for Architecture)
WD: Top 5 Institutions/databases having properties ID and number of entities (link to query)
Canadiana Name Authority ID: 30670
Cinémathèque québécoise person ID: 22205
BAnQ author ID: 11176
Library of PArliament of Canada person ID: 5129
Dictionary of Canadian Biography ID: 5125
)
		* Canadiana Name Authority ID: 30670
		* Cinémathèque québécoise person ID: 22205
		* BAnQ author ID: 11176
		* Library of PArliament of Canada person ID: 5129
		* Dictionary of Canadian Biography ID: 5125


## Roadmap

1. Necessary Research
   1. Infrastructure (e.g. technological components such as server or cloud; structural components such as a tabular database or  centralized ecosystem). 
   2. Governance models and processes
   3. Policy Models
   4. Legal and Rights Issues
   5. Model alignment (e.g. schema.org for indexing?)
   6. Choose Peripheral vocabularies (i.e. for occupations)
   7. Integration of the CLA in selected museum tools (e.g. CMS)
2. Extract relevant data from AC, AiC, ULAN, WD, ISNI, etc. 
3. Consolidate 
   1. Reconcile, enhance, and clean data
   2. Assign IDs
   3. Translate if necessary
4. Mapping to model(s)
5. Publication interface development
6. R&D Enhancements (Complimentary Projects)
   1. Necessary Research
   2. Develop/select model (actors?)
   3. Mapping to model 
   4. Peripheral vocabularies mapping (if not done in first phase blue)
   5. Adapt interface 
   6. Create SPARQL endpoint
   7. Tool development (in LOD or not; stats, graphs, API, etc.) 
   8. Conquer the world!

### Pipeline

A final high-level pipeline could be anticipated to take the following form (a dynamic version including anticipated tasks is available here): 

<iframe frameborder="0" style="width:100%;height:500px;" src="https://viewer.diagrams.net/?tags=%7B%7D&target=blank&highlight=0000ff&edit=_blank&layers=1&nav=1#G1Qf5BsLsiWgaiWp9HeeZQKLteokK7LBHf"></iframe>

## Resources

### Starting Requirements

The following would be needed before starting work on a prototype of a flat list (i.e. a tabular and/or JSON file that can be downloaded and searched): 

* Governance structure for the project, which would at least have to address: 
   * Authorization and/or confirmation that data extraction and/or publication can be done (especially in the case of more sensitive data);
   * Guidelines on the handling of sensitive data (identifying, shadowing);
   * CHIN’s authority and responsibilities with regards to the CLA data; 
   * Agreements from relevant rights and stakes holders. 
* Server with testing and deployment infrastructure and services off the PCH ecosystem;
* Research and decision making on a number of features, including: 
   * Would the CLA eventually be developed in LOD (if so, development might be impacted in the first stage of the project); 
   * Would the CLA be indexed on Google or not (and, if so, would it be using schema.org or other models)?
   * What languages would the CLA support? How would language precedence be established and on what grounds?
   * What other vocabularies will be used for peripheral information (e.g. occupation, place of birth)?
   * What hierarchical structure will be used (e.g. flat, relational)?
* Roadmap to completion and maintenance, including workflows and responsibilities assignments throughout the project: 
   * A non-LOD CLA would likely involve R&D work to extract the list from available sources and reconcile data, but further maintenance and updates would not involve R&D work; 
   * People in charge of maintenance would have to become familiar with GitHub or other web platforms to enable a deployment (or there would have to be a clear workflow and agreement as to updating, maybe at first); 
   * Conservation plan. 

### Development Requirements

The following would be needed before starting work on any research and development component (LOD enhancement to the flat file, tools, statistical analysis and visualizations): 

* Testing and development environment in parallel to the deployment one;
* Research and decision making on a number of features, including: 
   * What tools and features should be developed?
   * If there is a semantic component, what views would be offered?
   * What statistics or visualizations would be deemed relevant?
* Roadmap to completion and maintenance, including workflows and responsibilities assignments throughout the project: 
   * Governance model adapted to LOD; 
   * Infrastructure and services for SPARQL endpoint and API; 
   * Further development of the CLA, in LOD or not, would: : 
      * impact the work of the maintenance team who would likely have to become familiar with GitHub; 
      * require model alignment (and, if doing LOD, likely the testing of the Actors model);
      * necessitate specific software, tools, or agreements depending on the project. 
   * Conservation plan. 

### Sustainability Requirements

The following would be needed for deployment and maintenance of the CLA: 

* Dedicated production and maintenance infrastructure and site; 
* Staff assigned to maintenance both in terms of structure and contents; 
* Official governance model; 
* Long-term agreements with rights and stakes holders as well as relevant software providers;
* Official conservation plan.



