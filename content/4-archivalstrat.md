---
authors:
  - name: Kieron Niven
    orcid: https://orcid.org/0000-0002-0537-9238
    affiliations: Archaeology Data Service
  - name: Adam Brin
    affiliations: Centre for Digital Antiquity
---

# Archival Strategies

## Overview

Although it is easy to ignore issues of digital archaeological data preservation until the near-completion of a project, it is critical to consider aspects of preservation strategy throughout a project’s lifecycle. Depending on the preservation strategy selected, different resources may need to be identified to ensure preservation and access beyond the life of the project. Regardless of the preservation strategy chosen, it is critical that data be properly documented to ensure future usability. Documentation should catalog all of the contextual information necessary to use the materials in the future, including translations of codes and abbreviations, as well as descriptions of how data were captured.

The three most common preservation strategies are technology preservation, emulation, and migration. Each of these maintains different requirements for what may need to be archived and documented. Specific hardware descriptions, software version numbers, license keys and copies, as well as documentation of processes for saving and exporting files or using software are important candidates for archival. While it may require more work on ingest, both Digital Antiquity and ADS rely on the migration model for digital preservation. Both groups believe that this model creates less work and need for infrastructure in the long term, because serious preservation issues are identified and resolved at ingest. At that point, both the original and a preservation format of the file are archived. 

When selecting an archive, it is important to evaluate the archival policies and procedures of possible repositories. An important part of this process is to ensure that the policies of a potential repository cover preservation, access, backups, migrations, disaster recovery and sustainability. 

## The Digital Lifecycle

Preservation of digital data by data migration — the strategy advocated by these Guides — together with the OAIS model (which provides a structure for this strategy, see the relevant appendix on [The Open Archival Information System](OAIS) places an emphasis on the ongoing management and administration of a digital resource and an object lifecycle.

A common element in many preservation policies, the concept of a digital object lifecycle has been around for some time. At the 2006 conference *The LIFE Project: Bringing digital preservation to life* Neil Beagrie gave a paper entitled, "Life cycle modelling: the background" [@beagrie2006lifecycle], in which he discussed the evolution of lifecycle management from its beginnings in publications such as the Terotechnology Handbook [@hmso1978tetrotechnology], which considered lifecycle costing and the idea of "total cost of ownership" for physical objects. Subsequently, during the 1990s, the AHDS, the British Library and others built on this approach for digital assets. Beagrie noted how the early involvement of the JISC and the AHDS with project proposals, through the provision of guidance and advice, helped to reduce costs downstream. One manifestation of this early involvement was the publication of a number of AHDS Guides to Good Practice.

By 1998, lifecycle frameworks for managing digital resources had become well-defined. This is evident, for example, in Beagrie and Dan Greenstein’s "A Strategic Policy Framework for Creating and Preserving Digital Collections" [@beagrie1998strategic], and the subsequent development of this framework into a cost model by Tony Hendley in a British Library Research and Innovation Report (106) [@hendley1998comparison]. The LIFE Project final report provides a more recent and detailed methodology for calculating “the long-term costs and future requirements of the preservation of digital assets" [@mcleod2006lifecycle]. In addition, the [Digital Curation Centre's Curation Lifecycle Model](https://www.dcc.ac.uk/guidance/curation-lifecycle-model) provides a concise overview of how an object lifecycle can function and how elements continually feed back into the processes of preservation and reuse.

Although simplified, the generally recognised categories of the lifecycle of digital assets are:
* Data Creation
* Documentation and Metadata
* Acquisition and Selection (retention or disposal)
* Preservation and Management
* Access and Use/Reuse

These categories provide the framework for the subsequent introductory sections of the Guides. Although there is a logical structure to these elements, the Guides initially outline the core preservation and management strategies (this section). The proceeding introductory sections examine how data preservation methods can be simplified and made more effective through planning at the data and archive creation stages. The final introductory sections focus on data dissemination, access and use, particularly in the context of large datasets and rights management.

## The Three Main Preservation Strategies

At its simplest level, the preservation of digital files can be broken down into two key elements: first, the continued storage of data in an accessible and robust format, and second, the creation and maintenance of documentation (metadata) that allows the preserved data to be understood. Digital archiving strategies do not, and should not, rely simply on the physical preservation of a single disk, tape, or CD-ROM. The preservation of digital data, regardless of subject area or content, is generally approached via one of three main strategies:

* __Technology Preservation__
* __Emulation__
* __Migration__

Although archives commonly use all three strategies, these Guides recommend that a __migration__-based approach be adopted for the preservation of archaeological digital data. Such an approach relies on the continual migration of information from older hardware and software to newer systems. Conversely, in a __technology preservation__ strategy, the data is maintained unchanged along with the technology (hardware and/or software) upon which it depends. @rothenberg1999avoiding, Section 6.3 raises a number of problems associated with such a reliance on “computer museums,” namely that technology will inevitably fail over time, while maintenance and replacement simultaneously become increasingly difficult and costly. In the context of many archaeological projects, it is likely that substantial amounts of very specific software and hardware would need to be documented and preserved. The complete conservation of obsolete hardware and software systems, as part of technology preservation, is a costly and high-risk strategy that can be seen as unjustifiable unless data cannot be migrated and are of substantial international importance.

An __emulation__ strategy attempts to avoid some of the pitfalls of technology preservation through the emulation of older hardware or software systems in newer ones. This is technically challenging, expensive, and becomes increasingly difficult as current technology becomes ever more remote from the original systems employed. Emulation is therefore not recommended for archaeological archives.

Rothenberg, however, favours emulation as an alternative preservation strategy, which has particular relevance where the look, feel, and behaviour of a data resource are important. Critiques of emulation include that it is still in its infancy in terms of development, that it is likely to be more costly than the implementation of a migration strategy, that there are likely to be software copyright issues, and that the original software and hardware are rarely documented to a high enough level to allow subsequent emulation. An interesting and confusing development came about during the CAMiLEON project, which developed a strategy called "Migration on Request". This is, in fact, emulation with a tool being built to process the original byte stream of a digital object on request. An interesting case study in emulation was the decision to move an interactive video, created by the BBC (1986) to celebrate the 900th anniversary of the Domesday Book, away from its dependence on outmoded media and computer hardware [@darlington2003domesday]. Numbers of experts were approached, including the CAMiLEON project team, who “argued that the slight faults in images as displayed from the original analogue discs were a part of that experience, and should not be cleaned up.” However, the National Archive “wanted to preserve the data with the highest quality available consistent with longevity,” and hence opted for migration. Other projects that examine the possibility of emulation as a digital preservation strategy, such as KEEP, continue to emerge.

### Preservation by Migration

A migration-based preservation strategy is focused on the practice of moving data to software-independent formats (normalisation) and subsequently migrating that data through successive technical infrastructures over time (refreshment). There is, without doubt, a preference within the archival community that, where possible, data should be migrated to a small set of stable file formats and, where possible, that this process be openly documented. This not only reduces the potential number of refreshments that the data have to undergo, but also allows migration processes to be carried out easily across large datasets. As stated above, it is recommended that digital archiving in archaeology should employ the policies and procedures of controlled data migration. There are four main activities required for successful digital archiving with this strategy:

* Data Refreshment
* Data Migration
* Data Documentation
* Data Management Tools

### Data Refreshment

Data refreshment is the act of copying information from one medium to the next as the original medium nears the end of its reliable life span. Research into the life span of both magnetic and optical media has been conducted, with the overwhelming conclusion being that digital media are far more likely to become unreadable as a result of changing technology than they are through physical media degradation. Although magnetic media can be safe for 5-10 years, and optical media may survive for more than 30, the preferred technology changes much more quickly. For example, 10 years ago many archaeologists collected information on 3" Amstrad disks. These disks are completely unreadable by PC machines, and cannot be accessed unless a surviving Amstrad computer can be networked or has a peripheral such as a 3.5" disk drive. Even then, as Amstrads use a different operating system to PCs, the data must be exported in a standard format such as ASCII text. On the other hand, if archaeologists had refreshed their data from 3-inch Amstrad diskettes to 5.25" disks and then onto 3.5" disks, these digital data would still be accessible and safe.

The architecture of hardware changes rapidly, but not as rapidly as software. Data created or gathered in a proprietary software format is hostage to the long-term viability of that brand and of its parent company. These cannot be assured. Certain types of files have been earmarked as industry standard formats, while in other cases there may be open formats available that, while losing some of the original versatility, may nonetheless allow reconstruction or importation into other updated software types.

### Data Migration

Data migration is even more important than data refreshment for successful digital archiving. Migration is the act of copying digital information from one format or structure into another that can be read by current versions of software. One example is the migration of data between different Computer-Aided Design (CAD) packages. However, even though CAD packages allow data to be exported in a “standard” format (DXF), in fact many programmes create such DXF files in unique ways that may not be readable to other packages. The unwary can find that, without careful migration, much of the original information is lost when creating a new file. Many migration programmes incorporate a process of format normalization: files are migrated to common, stable formats and then, when necessary, through successive versions of the format. An ideal is to normalise files to open-standard and preferably text-based formats (e.g. XML or ASCII), although this is not always an option, as with images. In such cases, version and format migration is practiced, and files in these formats are also subject to periodic refreshment.

It is also essential to monitor ongoing research and development into good digital preservation strategies, and not to assume that the same formats are always the safest. Digital preservation requires active intervention and constant vigilance. If this cannot be provided locally, it is best to contact a professional digital archiving service.
A strict regime of validating all files and their documentation must be followed during the migration process. Original media should be retained until the validation process is 100% complete since it may be necessary to return to the original file if any aspect of the data could not be successfully and safely migrated.

## Data Documentation

In order for a digital archivist to migrate digital information successfully, it is necessary to understand the structure of the data and how different parts relate to one another. Data migration thus relies on the third activity: data documentation.

Documentation is essential for both the preservation and reuse of all dataset types. While abbreviations and shorthand used in the data might be understood by their creator, there is no guarantee that these will make sense to someone reusing the data several years later. Worse still, in a large archive, a file describing contexts or small finds may relate to only one of several possible excavations. For these reasons, it is necessary to document the codes or abbreviations used in the data together with any standards that have been followed or thesauri or word lists that have been used. In addition, it is often useful to provide an accurate (if brief) description of each file, explaining how different files fit together. Software often incorporates the option to generate documentation during the creation of files (e.g., field descriptions in databases), though these options can vary in their depth and relevance. The type of documentation required will also depend on the type of data; for example, the documentation for a text file may be quite straightforward, while that for a GIS or database may be quite intensive. Data documentation, at the file or data type level, is dealt with in more detail in the relevant chapters within these Guides.

No digital archivist can successfully preserve data that are not fully documented, because at every step of data migration information can be lost. This leaves archivists with two options: migrating data from one format and then double-checking each entry manually, or requiring thorough documentation of the data at the time of archiving so migrations can be carefully planned and tested in advance.

## Data Management Tools

As already noted, digital data needs to be regularly refreshed and migrated. Digital files that are stored on a local network or are in current use should move naturally into a localised back-up strategy as alterations take place. Digital files that are stored in a deep storage facility (a preferred archival strategy for long-term preservation, whereby files are stored in a remote and specialised repository) require active intervention for appropriate updating and version control to take place.

Digital archives need to be actively managed. Use of Electronic Document Management (EDM) systems is recommended; these are data management tools, usually in database form. The system employed should flag dates and will ideally automatically inform the archive manager when files need attention (backing up, migration, refreshment).

## Archival Policies

Organisations responsible for the long-term preservation and management of digital data should have well-documented archival strategies and procedures in place. Documentation can range from generic to quite specific policy statements, for example, the series of Preservation Handbooks produced by the UK's Arts and Humanities Data Service (AHDS) and its subject-specific data centres, including the ADS. Other national and international organisations providing useful documentation on strategies and procedures include the [UK Data Archive (UKDA)](https://www.data-archive.ac.uk/), the [British Library](https://www.bl.uk/about), the [Library of Congress](https://www.loc.gov/preservation/digital/), the [National Library of Australia](https://webarchive.nla.gov.au/tep/10691), the [United Kingdom Hydrographic Office (UKHO](https://www.gov.uk/government/organisations/uk-hydrographic-office), NASA’s [National Space Science Data Center (NSSDC)](https://www.nasa.gov/nssdc/), the [Electronic Resource Preservation and Access Network (ERPANET)](https://www.erpanet.org/), [The Digital Preservation Coalition (DPC)](https://www.dpconline.org/) and the [Digital Curation Centre (DCC)](https://www.dcc.ac.uk/). Whilst often organisationally specific, some generic themes emerge from the available information, including the creation of the International Organization for Standardization (ISO) standard Open Archival Information System (OAIS) (see [Appendix 1|App_OAIS]) and the increasing prevalence of Lifecycle Management as an archival strategy.

Recent developments have seen a move toward certifying data repositories and providing assurance that data remains accessible in the future. The publication of a certification document, “Trustworthy Repositories Audit & Certification (TRAC): Criteria and Checklist,” by the US-based Research Libraries Group (RLG), the Center for Research Libraries (CRL) and the National Archives and Records Administration (NARA), aims to provide a checklist for identifying repositories capable of reliably managing digital collections. The audit checklist is closely tied to the OAIS reference model in terms of its conceptual framework and terminology. It considers organisational suitability, repository workflows, user communities and the usability of data, plus the underlying technical infrastructure of a repository, including security. All of these areas must be openly documented. Organisations that can demonstrate that they meet the criteria within the checklist will be identified as Trusted Digital Repositories. The CRL is currently undertaking a project to test the RLG-NARA metrics through actual audits of subject digital archives and one archiving system, and has published an audit report on the assessment of Portico.

The [Data Seal of Approval](https://www.coretrustseal.org/about/history/data-seal-of-approval-synopsis-2008-2018/) aims to provide a similar quality assessment to that of the TRAC system, although with a slightly simpler structure based on sixteen guidelines and focused on three groups of stakeholders (producer, consumer and archive). Again, as with TRAC, the aim is to "guarantee the durability of the data concerned, but also to promote the goal of durable archiving in general". In general, the archival community is actively seeking to become compliant with the OAIS reference model through the process of certification. However, it should be noted that such audit checklists are a very recent development 
and, for the time being, a state of trust needs to exist between creator and archive.

## Bibliography

Beagrie, N. and D. Greenstein (1998) *A Strategic Policy Framework for Creating and Preserving Digital Collections*.

Darlington, J., Finney, A. & Pearce, A. (2003) 'Domesday Redux: The rescue of the BBC Domesday Project videodiscs'. *Ariadne* 36. http://www.ariadne.ac.uk/issue36/tna/

Terotechnology Handbook (1978) HMSO.

Rothenberg, J. (1999) *Avoiding Technological Quicksand: Finding a Viable Technical Foundation for Digital Preservation*.