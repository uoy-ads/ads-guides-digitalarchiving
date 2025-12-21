# The Project Archive: Storage and Dissemination

This chapter aims to outline some of the main requirements and issues of the long-term storage and dissemination of archaeological documents, datasets, and other resources. It is assumed throughout these Guides that the majority of data creators will ultimately aim to deposit materials with a suitable digital archive or repository. Regardless, a number of factors are useful to consider when evaluating an archive, building an archive, or preparing for a project. Some of these factors are storage, backup, bandwidth, access and large or complex data, such as the result of sensory data scans.

Depending on the lifecycle of data, resources and even archives, planning for storage, backup, and dissemination may be simple, and may include a computer, a set of external hard-drives, or backup media. As any aspect of the lifecycle may grow over time or through complexity of data collected, some of these issues become more intricate. For projects that span more than a few years, hardware replacement and migration costs should be considered as well. Furthermore, larger projects will require additional infrastructure to ensure appropriate storage, backup, and dissemination. Over time, storage is comparatively cheap and its cost may be considered negligible over a 20-year period.

For projects with significant amounts of data, network infrastructure may also be important; like archives, data transfer (for backups, dissemination, or storage) will become a factor in the ability of a project to succeed. In certain cases, the use of physical media and the calculation of checksums when transferring files, especially large data files, may be useful to ensure the speed and accuracy of transfer.

## A Brief Overview of “Big Data”

The concept of “Big Data” in archaeology is typified by file formats that have exceptionally large file sizes and, in particular, the technologies associated with their storage and delivery. The generation and use of such data is increasing in certain fields of archaeological and cultural resource management activity—for example, in maritime archaeology and surveying, laser scanning, LIDAR, computer visualisation and other scientific research applications. There is, however, little understanding of the implications for cost and good practice in data preservation, dissemination, reuse and access. This lack of understanding is potentially exacerbated by the proprietary formats often used by new research technologies now commonplace in archaeology and cultural resource management.

A project examining [Big Data](https://archaeologydataservice.ac.uk/about/projects/big-data/) was carried out by the ADS in 2005-6 as the result of a lack of guidance about Big Data technologies for the archaeological community. Existing archival guidance previously did not cover such technologies, and the final Big Data report and Formats Review made significant progress towards suggesting solutions to current problems. This chapter aims to cover, within the context of general data retention and dissemination, some of the issues highlighted in the report. However, readers are also advised to consult the project documents for a wider discussion and context for Big Data. In addition, this chapter will not detail recommendations for specific data types, as these have been incorporated within the relevant technique-specific chapters (e.g., Marine Remote Sensing or Laser Scanning). The original Big Data report did, however, note that much can be learned from non-archaeological organisations that have long-running experience of these technologies and, where possible, such examples will be highlighted within this chapter.

## Storage, Backup and Data Curation

On the surface, the physical storage of most datasets is largely unproblematic with terabyte external hard drives cheaply and widely available. Many archival organizations, however, invest heavily in backing up data (both internally and externally). For example, the ADS subscribes to the University of York backup service, which uses Legato Networker and an Adic Scalar Tape Library and also maintains copies of data in the UK Data Archive (UKDA). As highlighted in the previous chapter on [Planning for the Creation of Digital Data|CreateData_1-0], a basic strategy for storing a project dataset could be as simple as the use of high-capacity hard drives with copies stored offsite in a fairly inert environment and synchronised on a regular basis with the master data. Such a strategy should be supported, as previously outlined, by other procedures to ensure reliable version control and protection from viruses and other sources of data corruption. Problems in the physical storage of data are, however, relative and should be examined within the context of the resources available to the organization storing the datasets. The threshold of what is problematic, either because it is large in terms of file numbers or size, is generally much lower within Archaeology than in other sectors, such as the Earth Sciences, which have more resources and are accustomed to working with such data. Currently, tens of gigabytes are probably problematic for archaeologists in terms of accessibility and long-term storage (availability), but expectations are becoming larger in terms of both storage availability and datasets in use.

__Hardware and Data Refreshment__

It should be noted that “storage” covers not only the size of the media on which data is stored and backed up, but also encompasses the ongoing periodic process of data refreshment (the movement of datasets to new hardware or software environments). While the cost of physical storage continues to decrease, that of refreshment and long term curation - key factors in continuing to make data accessible and available - does not. In addition, in order to take advantage of technological advances and decreasing costs in certain areas, archives have to periodically upgrade systems or parts thereof.

The cost of physical disc storage and backup media, such as tape, decreases rapidly. Analysis of past and current trends suggest that, beyond a five-year period, the cost of a gigabyte will have decreased so much as to be considered a zero-cost object [@gilheany]. However, the capital cost of the systems associated with such storage can be substantial, as can ongoing maintenance, backup and insurance costs. From experience, the cost of refreshment for a given resource partially decreases with time as archival systems become more sophisticated and a given archive becomes an increasingly smaller part (presuming archival growth) of periodic refreshment. This gradual decrease in the cost of refreshing a given resource is, however, partially offset by the increasing cost in human resources (i.e. increasing wages) that, between refreshments, is required for the ongoing proactive management and administration of the archive or repository.

As an example, in its 10-year history the ADS has now moved to its third generation of equipment, essentially operating on a five-year upgrade cycle. This is expensive in terms of both the new equipment and also with regard to the staff time required to implement setup and migration from the old system. The long-term cost of storage is often difficult to conceptualize but, based on this example of a five-year cycle, a dataset maintained for 100 years would go through 20 refreshments. There is no reason why certain digital datasets should not be maintained for such a period considering that many of our most valued paper archives are of considerable antiquity.

The test of time suggests that so far, the one-time 50p (ca. 63 cents) per megabyte charge in the current ADS policy is near the mark for an earlier archival tradition. Recent developments, however, in systems upgrades suggests that this charge can be reduced significantly. This “per megabyte” charge is shorthand for what has been described above, and might be better described as “ongoing management and refreshment.” The following is simplistic but attempts to represent more accurately the current situation of lifecycle management and its associated retention and discard policies.

```{list-table}
:header-rows: 1

* - Retention period
  - Cost for refreshment
* - 5 years
  - R + E
* - 10 years
  - R - DR + E - DE
* - 15 years
  - R - 2DR + E - 2DE
* - 20 years
  - R - 3DR + E - 3DE
* - 25 years
  - R - 4DR + E - 4DE
```

Where R = refreshment cost 
<br>DR = decreasing cost of refreshment 
<br>E = cost of physical equipment 
<br>DE = decreasing cost of equipment


As an example, if R = 9p, DR = 3p, E = 4p and DE = 1p (all pence per megabyte charges are for example purposes only—they could equally be thought of as cent per megabyte charges) then:

```{list-table}
:header-rows: 1

* - Retention period
  - Cost for refreshment (pence)
  - Cumulative total (pence)
* - 5 years
  - 9 + 4 = 13
  - 13
* - 10 years
  - 9 - 3 + 4 - 1 = 9
  - 22
* - 15 years
  - 9 - 6 + 4 - 2 = 5
  - 27
* - 20 years
  - 9 - 9 + 4 - 3 = 4
  - 28
* - ongoing
  - 
  - 30
```

The above one-time costs suggest that preservation costs become negligible after 20 years. This is, to a degree, a product of the simplicity of the model as, clearly, there will be ongoing costs of refreshment, management and administration of a resource based on retention policy. Thus a one-time charge of 30p (ca. 38 cents) per megabyte would cover ongoing preservation beyond 20 years. ADS policy is currently based on the assumption that “best efforts” will be used to preserve all data deposited with ADS in perpetuity (i.e. following the 20-year cost model above). However, in some cases it is possible that funding agencies may no longer require preservation beyond a specified period, which might be subject to review at regular intervals. A number of possible reasons to discard a dataset exist, including that only a specified period of preservation was required, that it has been superseded or included in another resource, that it is no longer considered to have value or that there is no practical way to continue its preservation.

__Hardware and Refreshment Issues Specific to “Big Data”__

So long as data are finalised in a suitable archival package (suitable file formats, sufficient documentation and metadata), archiving Big Data should be no more consuming of human resources than archiving any other data. It takes much more time to move these files because of their physical size, for example, when ingesting data from delivery media into an archival environment. Similarly, confirming the success of a transfer through generating fixity or checksum values is a much longer process because each byte in a file is referenced. However, both of these processes can be run as background or automated tasks, thereby potentially reducing the “human cost.” By definition, the physical storage requirements of Big Data are greater than a more conventional dataset. However, Big Data archives would fit comfortably within a charging policy where storage fees are assessed by the megabyte and ingest costs are based on the number of files comprising a resource.

## Data Dissemination

As with the transfer of data between creator and archive, the dissemination of datasets to a wider audience is often seen as problematic. This is particularly the case for Big Data. User preference is for online access to files, and this is typically not problematic for archival organizations that are often part of high-bandwidth systems and thus capable of making resources available. However, in the case of Big Data it is dangerous to assume that users have access to high-bandwidth connections, or that these capabilities are globally uniform. For this reason, many archives restrict or scale file download sizes so users don't unwittingly affect their networks. On occasion, larger files are made available for download by special arrangement (e.g., via http or ftp download) for users known to have suitable connections.

While large datasets consisting of numerous small to medium files are a minor problem for archives to host and users to download, single large files - raw point cloud data from laser scanning, detailed satellite imagery or bathymetric data, for example - present a more complex issue. Single smaller files, even on slow Internet connections, can be downloaded individually so that a user can assess their content and relevance. In contrast, larger files require more time to download and thus place a greater draw on resources for both the user and the archive. Larger files are often also difficult to “summarise,” or allow the user to know what the file contains prior to download and, in many cases, it may not be the entire file that the user requires.

__Networks__

In terms of simply providing stable access to a large file and reducing load at both ends, a variety of network technologies were investigated as part of the Big Data Project including popular peer-to-peer methods such as [BitTorrent](https://www.bittorrent.com/). It was concluded that, although such a method could support a distributed archiving model, the reuse of data (especially Big Data) is likely to be an occasional and limited activity within a small community. The consequence of this pattern is that limited downloads - and thus peers - would create little, if any, improvement in download speed or reliability. High-speed “Point of Access” (PoA) optical networks such as the JANET Lightpath service were also considered but the cost of implementation (several thousand pounds) prevented this proceeding further. These examples illustrate some of the difficulties presented by Big Data in terms of allowing online access to users. 

__Web Services and Grid Computing__

Web Services and Grid Computing techniques both provide a more flexible approach to disseminating data but also increase cost to the archive. Web Services such the [National Geoscience Data Centre GeoIndex](bgs.ac.uk/services/ngdc/home.html) and the British Atmospheric Data Centre Data Extractor Tool allow users to navigate datasets online and to define and extract subsets of data. In addition, other web services and grid-based applications, such as [NERC Earth Observation Data Centre](https://archaeologydataservice.ac.uk/archives/view/btrar_ahrb_2005/) contain tools that allow users to skip the download stage altogether. Instead, users can process data in various ways or to other formats online, without the need to download the whole dataset. Such services obviously have a huge potential to improve the issues of previewing data and download capabilities (and even user access to software) but provision of these tools places a greater cost on the archive.

__Physical Media__

Currently, the most consistent way of disseminating very large datasets is by request on portable media such as DVDs (for smaller sizes) and external hard drives (for anything larger). As noted already, one-terabyte portable hard drives are relatively cheap and available and can be supplied as well as returned.

Acquiring large files is likely to be expensive in one way or another, whether due to occupation of bandwidth or to costs for preparing media. Clearly, potential users need to be able ascertain the relevance of available data to their work. Traditionally, this has been accomplished through extensive online descriptive metadata catalogues such as the National Oceonography Centre SeaDOG database, which act as pointers to data holders from which the user can negotiate data download. The use of “tasters” such as thumbnail images or movie clips is also a well-established decision support mechanism. 

Big data suggests some more unusual mechanisms such as fly-throughs and point cloud models; for example, the point cloud models produced by the Big Data case study [“Breaking through Rock Art Recording'](https://archaeologydataservice.ac.uk/archives/view/btrar_ahrb_2005/). These are generally project outcomes and tend to use decimated datasets, but they will inform on the relevance of the associated raw data. 

## Bibliography

Gilheany, S. (nd) The Decline of Magnetic Disk Storage Cost Over the Next 25 Years. White paper.