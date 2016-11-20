# netcdf-ld

netCDF-LD is an approach for constructing Linked Data descriptions using the metadata and structures found in netCDF files. Linked Data is a method of publishing structured data on the web so that it can be interlinked and become more useful through semantic queries. It uses the W3 Resource Description Framework (RDF) standard to express the information and relationships.

netCDF-LD enhances netCDF metadata, enabling information found in netCDF files to be linked with published conventions and controlled vocabularies used to express the content.


## The problem

NetCDF is commonly used in environmental applications from climatology to oceanography, and more recently in the geosciences. NetCDF files often adopt conventions to encode certain information relevant for users of the data, e.g. Climate & Forecast (CF) Metadata Conventions and the Attribute Convention for Data Discovery (ACDD). Data encoded using conventions like CF and ACDD contain much useful metadata that could be leveraged to provide enhanced discovery, integration and understanding using Semantic Web technologies, but right now the information is locked away in individual files.


Conventions like CF and ACDD are not sufficient to cover all possible vocabularies and schemas for data stored in netCDF files, nor should they try to be. Other relevant vocabularies and schemas exist, are maintained by various institutions and communities, and have their own lifecycle and usage. Without a mechanism that allows different vocabularies and schemas to play nicely together, data authors are often forced to choose between conventions or end up presenting users with a confusing and possibly conflicting mix of namings and interpretations.

## Why netCDF-LD 

* Provides a view of definitions of nearly every part of my netCDF file by following the URIs in the generated RDF triples.
* Provides tools and support for enhancing discoverability and access of netCDF data from data repositories.
* Provides views of netCDF metadata that can be linked with other netCDF metadata and related information on the Web.


## More about netCDF-LD netCDF-LD solution

The netCDF-LD working group is currently working on a candidate specification using existing netCDF files that are encoded using CF and ACDD conventions as test cases.
 
The current activity features two parts: 1) A way to scan existing netCDF files that use CF and ACDD and generate RDF statements. 2) A way to specify other vocabularies and schemas so that RDF statements can be generated linking the data to many metadata systems.

We are currently working on a set of conventions to define prefixes and aliases and rules for their use that allow URIs to be layered over existing netCDF file metadata, providing Linked Data views on the file contents.
