# Project Metadata

Metadata is descriptive information about documents, datasets, images, and other material. Providing metadata enables discovery, accessibility, and usability of files contributed to an archive by providing standardized fields and terms to describe files. Furthermore, metadata provides context for non-textual materials like datasets or images that may not be usable without this additional information. Metadata commonly refers to a standardised set (a scheme or schema) of information that can be used to document, in a structured way, different aspects of data archiving at various levels.

Depending on the project, resource, or file, metadata may be either general or specific, but at minimum should provide the "who, what, when, where and how" information relating to a file or project. Information should be detailed enough that others are able to evaluate from the metadata whether they need the file or project. Common types of metadata include:
 
* General descriptive information about the contents of a file or project; 
* Information which places the project or file within a broader context;
* Administrative information tracking submission, access, and rights; and
* File or technical metadata identifying how the file was created, the program used, file size, and other detailed information.

The process and reasons for creating metadata are well-documented in a number of existing guidelines and by numerous organisations and repositories (e.g. @niso2004understanding, @day2006metadata, @ballegooie2006archival) but, put simply, metadata aims to make digital resources easily identifiable, retrievable and usable through the storage of descriptive and contextual information.

## Types of Metadata

For the purposes of these Guides metadata can be loosely grouped into a few categories (as described below). For the most part, these types of metadata are collected at a certain level (e.g. project or individual resource) but particular elements may be recorded for data from the general down to the specific file level. In addition, certain metadata standards may record elements of metadata that function at a number of levels (e.g. 'Author' may aid resource discovery as well as provide administrative information). The three categories relevant to archaeological projects are project-level metadata, resource-level metadata and file-level metadata.

__Project-Level Metadata__ (incorporating 'Descriptive' and 'Resource Discovery' metadata) is largely recorded at a broad level for an entire project/archive irrespective of the techniques used and covers elements such as period terms or dates, site and artefact keywords, project details, site codes and geographic location. Often, much of this information is included within documents in the archive (e.g., site reports).


*Descriptive or Resource Discovery Metadata* is designed to allow the comprehensive description and easy retrieval of datasets or documents, and is more about the project and its results. The [Dublin Core](https://www.dublincore.org/) standard is a good example of a metadata standard which incorporates a number of descriptive and resource discovery focussed elements.

__Resource-Level Metadata:__ Many archives, including the US-based tDAR archive, distinguish a middle tier of metadata elements relevant to the individual resources that make up an archival project. A resource, by this definition, may include one or multiple files, depending on the context. A simple example might be a PDF document, image, or access dataset. A more complex example might be a sensory data scan, a GIS shapefile, or even some databases where a single functional 'resource' consists of multiple files. 


The purpose of this metadata largely overlaps with the project level, with a descriptive or research discovery emphasis, but focuses on details that typically vary within the context of a larger project. These may include specific bibliographic citation fields, dates, locations, material types, or keyword-list elements that do not crosscut all resources in a project. In a sense, these metadata are more about the results reported in the individual resource rather than in the overarching project, and are documented primarily to aid discovery.

__File-Level Metadata__ (incorporating “Technical” and “Preservation” metadata) is typically very specific and applied, as the name implies, at the level of individual files. File-level metadata incorporates information on hardware and software along with validation methods such as checksums. In many cases, if the data is to be deposited in a digital archive, it is the archive itself that will generate much of this metadata. However, the data creator must often supply a number of elements, often during the process of data creation. By its nature, technical metadata is often very specific to the data type and will therefore be covered within the relevant chapters in these Guides.


A fourth broad category, __Administrative Metadata__, exists within all of the above and covers elements such as creation and acquisition as well as alteration and version control [@higgins2007what]. Included within this metadata is information concerning intellectual property rights. Such information can be recorded at a general level (e.g., ownership for an entire dataset may be held by one person or organisation) but should also be recorded for specific techniques or datasets where personnel or authors and intellectual property right holders differ.

In addition to the benefits of a structured schema, metadata at any level can be further enhanced through the use of specific, standardised word lists and thesauri. These are resources, such as the English Heritage [NMR Monument Type Thesaurus](https://heritage-standards.org.uk/fish-vocabularies/) or the MDA [Object Type thesaurus](https://heritage-standards.org.uk/fish-vocabularies/), which allow elements of metadata schema (e.g., The Dublin Core “Subject” element) to be completed in a controlled way, thereby increasing the usability and reliability of the metadata. Throughout these Guides, where specific metadata schema are indicated, suitable resources for qualifying elements will also be highlighted.

## Project- and Resource- Level Metadata

General Project- or Resource- level metadata, like a good library catalogue, allows users to quickly and easily identify available resources and connects them to those that they need. However, for this to work effectively, the metadata has to be implemented accurately and in a standard format. A commonly used format (and that used by the ADS) for project-level metadata is Dublin Core. The standard - which has both “simple” and “qualified” versions - consists of fifteen core elements (eighteen in the qualified version) that can provide a detailed overview of the project as a whole, including geographical coverage, temporal dates, methodology, monument and evidence types. Within tDAR, the basic Dublin Core metadata schema has been extended to include archaeology-specific fields as well as to include fields from the [Metadata Object Description Schema (MODS)](https://www.loc.gov/standards/mods/). At the early stages of a project, metadata often cannot be accurately compiled; however, project workers should familiarise themselves with the types of generic project-level metadata required. When depositing data with an archive, the depositor will often be expected to complete a project- or resource-level metadata record template, together with any relevant format-specific (e.g., geophysical survey) templates.

The example below (Table 1) forms the foundation of ADS project-level metadata and consists of the basic Dublin Core elements. In tDAR this set of metadata elements corresponds to information collected at both the overall project level and in many cases for the individual resources (e.g., Project Title loosely corresponds to a more general Title that may be used for individual documents or datasets at the resource level). It is also worth noting that tDAR metadata entry forms expand on this list to capture a variety of details that are grouped below (Table 2). More information on tDAR metadata is available in the [tDAR Data Dictionary](https://tdar-arch.atlassian.net/wiki/spaces/TDAR/pages/557072/Data+Dictionary).


```{list-table} ADS Project Metadata
:header-rows: 1
:name: ADS Project Metadata

* - Element
  - Description
* - __Project Title__
  - The title (and any alternatives) for the dataset.
* - __Description__
  - A brief summary of the main aims and objectives of the research project (or alternative process) from which the data collection arose together with a brief summary description of the content of the dataset.
* - __Subject__
  -  Keywords for the subject content of the dataset (qualified using e.g., the English Heritage NMR Monument Type Thesaurus or the MDA Object Type Thesaurus.
* - __Coverage__
  - This is both spatial and temporal coverage.<br>For spatial coverage it should include the current and contemporary name(s) of the country, region, county, town or village covered by the data collection and, where possible, a standardised reference such as the [Getty Thesaurus of Geographic Names](https://www.getty.edu/research/tools/vocabularies/tgn/) should be used. If names or administrative units were different during the time period covered by the data they should be recorded separately. Site coordinates can also be entered as a National grid reference in a number of different ways e.g., as a point (useful to describe a small project area via a central coordinate); as a line (e.g., at least 2 coordinates to represent the linear limits of the site); as a polygon (for a more complex site area, 3 or more coordinates are used to describe the boundaries). If applicable, the full postal code for the site can be included.<br>For temporal coverage it should include the dates/period covered by the dataset (using existing thesauri where possible such as the RCHME Period List).
* - __Creators__
  - Details of the creator(s), compiler(s), funding agencies, or other bodies or people intellectually responsible for the data collection. Information should include forename, surname, affiliation, address, phone, fax, email, or URL.
* - __Publisher__
  - Details about any organisation which has published this data.
* - __Contributors__
  - Other individuals or organisations who have contributed to the resource.
* - __Identifiers__
  - Project or reference numbers used to identify the dataset.
* - __Source__
  - Any important earlier work(s) from which this resource is derived.
* - __Dates__
  - Dates indicating when the dataset was created, when the archaeological project was carried out, processing dates, or computerisation dates as appropriate.
* - __Copyright__
  - The name of the copyright holder for the dataset. If the collection was created during work by an employee, the copyright holder will normally be the employer. If the material is covered by a specific copyright (e.g., Crown copyright) please indicate this.
* - __Relations__
  - If the data collection was derived in whole or in part from published or unpublished sources, whether printed or machine-readable, this element should include references to the original material, details of where the sources are held and how they are identified there (e.g., by accession number). If the collection is derived from other sources include an indication of whether the data represents a complete or partial transcription/copy and the methodology used for its digitisation. Also include full references to any publications about or based upon the data collection.
* - __Language__
  - Indication of which language(s) the dataset is in (e.g., English, French, Spanish).
* - __Resource Type__
  - Whether the dataset is best described as primary data, processed data, an interpretation of data, or a final report.
* - __Format__
  - The format the data is saved in (e.g., WordPerfect 5.1, HTML, AutoCAD).
```

Completed examples of this type of schema can be found in the [ADS Guidelines for Depositors](https://archaeologydataservice.ac.uk/help-guidance/instructions-for-depositors/collection-level-metadata/).


```{list-table} tDAR General Metadata
:header-rows: 1
:name: tDAR General Metadata

* - Element
  - Description
* - __Basic Information__
  - Basic metadata include association of a resource with a larger project, lifecycle status (e.g., draft, active, deleted), Language, Year Created, Abstract/Description and Physical Storage Location.
* - __Bibliographic Metadata__
  - Specific to documents, uses MODS metadata fields to describe resources.
* - __Resource Creators__
  - These fields are used to properly credit individuals and institutions for their contribution to the resource. “Role” refers to the individual’s main role for the resource (e.g., creator, editor, etc.).
* - __Resource Specific or Agency Identifiers__
  - Describes agency or project identifiers used (e.g., Smithsonian Trinomial, AZ State Museum—ASM—number).
* - __Investigation Type(s)__
  - Lists all investigation types relevant to the resource (e.g., Research Design, Site Monitoring, Data Recovery/Excavation).
* - __Site Description Information__
  - Includes Site Name, Site Type (controlled vocabulary), and keywords
* - __Material Type(s)__
  - Artifact types covered by the resource (e.g., Ceramic, Fauna, Metal, Dating Sample).
* - __Cultural Term(s)__
  - Includes Culture (e.g., PaleoIndian, Archaic) and user created values.
* - __Temporal Coverage__
  - Includes Temporal Terms (e.g., Pueblo IV), Coverage Dates, Date Type (e.g., Calendar, Radiocarbon), Start/End Years and Description (e.g., Calibrated, Range of ± N years).
* - __General Keyword(s)__
  - User created values to describe aspects of the resource not covered by other metadata.
* - __Spatial Terms__
  - Includes Geographic Terms (e.g., Death Valley), Coordinates
* - __Resource Provider__
  - The institution that authorized the resource to be archived and disseminated.
* - __Individual and Institutional Roles__
  - Name, Current Email Address, Institution and Role of those involved with the resource.
```

## File-Level Metadata

File-level metadata relates primarily to information required by an archive to preserve and disseminate files, but additionally, allows users to understand the nature of the files within a dataset and their reuse potential. File-level metadata is highly dependent on the type of data being recorded and the file type itself, but commonly includes notes on elements such as the software used in creating the file, lists of file names, relationships between files and so on.

Although the first edition of the ADS *Digital Archives from Excavation and Fieldwork: Guide to Good Practice* recommended that each file in a digital archive should have an associated metadata record, experience has demonstrated that this level of documentation is largely unnecessary. Dependant on the nature of the data, groups of files of the same format or sharing other characteristics can be documented by a single metadata record. It was recognised that the provision of file-level documentation places a large burden upon the creator and substantially increases the time—and hence the cost—necessary to construct the archive. Research has also shown that users of digital data are more likely to search for entire archaeological projects, or for particular categories of information, reducing the need for individual file metadata.

Alternately, the US-based tDAR metadata schema recognises that, for many kinds of records or resources that may be archived from an archaeological research project, it is worth the additional effort to maintain resource-level metadata records. For example, documents (e.g., site reports) or datasets generated from artefact-based analyses are well-served by metadata records tied to each individual resource. But, at the same time, it may not be necessary to maintain separate metadata for every file—for example, cases where two versions of a document (one complete for archival and research purposes, another redacted to protect sensitive content from unauthorised viewers), essentially the same resource, are stored in the digital archive. Also, some file types, such as images, are more efficiently handled with primarily project-level metadata similar to that advocated by ADS. 
File-level metadata is essential for discerning exactly what is in a dataset and how it can be used. It is recommended that, where data-specific guidelines are not suggested elsewhere in these Guides, the following elements be recorded as a bare minimum at a file level.

```{list-table} Generic minimum file-level metadata
:header-rows: 1
:name: Generic minimum file-level metadata

* - Element
  - Description
* - __File name__
  - The name of the file e.g., report.doc
* - __File format__
  - The file format e.g., PDF/A or Open Office Document
* - __Software used to create the files__
  - The software used to create the file e.g., Microsoft Word 2007
* - __Hardware used to create the files__
  - The hardware used to create the file, this is more significant when files are created directly by survey equipment such as laser scanners or GPS devices.
* - __Operating system used to create the files__
  - The operating system under which the file was made e.g., Windows XP or Mac OS X 10.5.
* - __Date of creation/last file update__
  - When the file was made or updated.
* - __Processing history or Lineage__
  - This element should be used to highlight relationships between files and whether a file is a source file or derived from another.
```

If deposited with an external archive, this information would generally be entered into the archive's internal file management system and used to plan future migration and validation strategies for the data. It is at this point that file-level metadata is enhanced by elements such as fixity values or [checksums](https://en.wikipedia.org/wiki/Checksum). These are "a form of redundancy check, a simple way to protect the integrity of data by detecting errors in data." The MD5 (Message-Digest algorithm 5) and the SHA (Secure Hash Algorithm) are widely used cryptographic hash functions, and applying these algorithms to a file produces an (almost certainly) unique hash or checksum value that provides a mechanism for validating and auditing data. An isolated checksum is of no use on its own. It has to be associated with a file, a location and a project as structured data. The schema below is an example of one structure that can be used to hold such file-level metadata.

```{list-table} File-level technical metadata
:header-rows: 1
:name: File-level technical metadata

* - Element
  - Description
* - UNIQUE_ID
  - Auto-generated unique ID e.g.,1234567
* - FILE_LOCATION
  - The file path i.e. directory and filename e.g., /adsdata/cottam_ba/jpg/fwking_plan.jpg
* - CHECKSUM_TYPE
  - The checksum algorithm used e.g., MD5, SHA-1, etc.
* - CHECKSUM_VALUE
  - The checksum value generated by algorithm e.g., 578cbb18f73a885988426797bcab8770
* - PROJECT_ID
  - A unique project ID e.g., ADS-123
* - GENERATED
  - Date the checksum was created e.g., 16-May-2006
* - GENERATED_BY
  - Person who created the checksum e.g., Doe, J
* - LAST_AUDITED
  - The date at which the file was last checked or verified e.g., 16-May-2007
```

In addition to more detailed fixity information, an archive (and possibly a data creator) will want to maintain a process history as part of archival practice. An example would be importing XYZ data into a GIS. Again, this can be recorded as simple structured data. The same structure can hold both file-level and batch processing information. The following example is based on AHDS practice.

```{list-table} File-level process metadata
:header-rows: 1
:name: File-level process metadata

* - Element
  - Description
* - PROCESS_ID
  - Auto-generated unique ID e.g.,1234567
* - PROJECT_ID
  - A unique project ID e.g., ADS-123
* - SOURCE_FORMAT
  - The format of the original file e.g., .txt
* - DESTINATION_FORMAT
  - The destination format e.g., .shp
* - PROCESS_AGENT
  - Who did the processing e.g., Doe, J.
* - PROCESS_COMMENTS
  - Comments relating to the process undertaken e.g., “referenced to WGS84'.
* - PROCESS_START_DATE
  - Date that the process started e.g., 17-May-2007
* - PROCESS_COMPLETION_DATE
  - Date process completed e.g., 17-May-2007
* - PROCESS_DESCRIPTION
  - A description of the process e.g., “Import of XYZ data into ArcView for analytical purposes and dissemination as research outcome'.
* - PROCESS_GUIDELINES
  - Any guidelines related to the process.
* - PROCESS_HARDWARE_USED
  - Hardware used to process the file e.g., Viglen Genie Intel Pentium 4
* - PROCESS_SOFTWARE_USED
  - Software used to process the file e.g., ESRI Arcview 9.1
* - PROCESS_INPUT
  - Full file path of the source file e.g., /adsdata/pro-453/xyz/file.xyz
* - PROCESS_OUTPUT
  - Full file path of the output file e.g., /adsdata/pro-453/shp/file.shp
* - PROCESS_RESULT
  - Comments on the result of the processing e.g., “Success”.
* - PROCESS_TYPE
  - Description of the process carried out e.g., “Conversion – dissemination.”
``` 

## Bibliography

van Ballegooie, M. and Duff, W. (2006) ‘Archival Metadata’ in S. Ross & M. Day (eds.) DCC Digital Curation Manual. http://www.dcc.ac.uk/resources/curation-reference-manual/completed-chapters/archival-metadata

Day, M (2005) ‘Metadata’ in S. Ross & M. Day (eds.) DCC Digital Curation Manual. http://www.dcc.ac.uk/resources/curation-reference-manual/completed-chapters/metadata

NISO (2004) Understanding Metadata. NISO Press. http://www.niso.org/standards/resources/UnderstandingMetadata.pdf