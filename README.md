# netcdf-ld

netCDF-LD is an approach for constructing Linked Data descriptions using the metadata and structures found in netCDF files. Linked Data is a set of practices to allow structured data to be published so that it can be interlinked on the web and support semantic queries. It uses the W3 Resource Description Framework (RDF) to express the information and relationships.

netCDF-LD enhances netCDF metadata, enabling information found in netCDF files to be linked with published conventions and controlled vocabularies used to express the content.


## The problem

netCDF is a data format commonly used for array and gridded data in environmental applications, particularly climatology and oceanography, and recently in the geosciences. netCDF files typically use “community conventions” within the file to encode details relevant for users of the data, e.g. Climate & Forecast (CF) Metadata Conventions and the Attribute Convention for Data Discovery (ACDD). While these conventions allow the detailed definitions to be delegated to a common place, the links to the definitions are indirect, and not generally known to users outside the communities, so the definitions cannot be immediately used for discovery, integration and understanding. 


Furthermore, the existing conventions (CF, ACDD) do not cover all possible applications, nor should they try to. Other relevant vocabularies and schemas exist, are maintained by various institutions and communities, and have their own lifecycle and usage. We need a mechanism that allows different vocabularies and schemas to play nicely together, so that data authors can combine conventions without a confusing and possibly conflicting mix of namings and interpretations.


## Why netCDF-LD 

* Provides a view of definitions of nearly every part of my netCDF file by following the URIs in the generated RDF triples.
* Provides tools and support for enhancing discoverability and access of netCDF data from data repositories.
* Provides views of netCDF metadata that can be linked with other netCDF metadata and related information on the Web.


## More about the netCDF-LD solution

The netCDF-LD working group is currently working on a candidate specification using existing netCDF files that are encoded using CF and ACDD conventions as test cases.
 
The current activity features two parts: 1) A way to scan existing netCDF files that use CF and ACDD and generate RDF statements. 2) A way to specify other vocabularies and schemas so that RDF statements can be generated linking the data to many metadata systems.

We are currently working on a set of conventions to define prefixes and aliases and rules for their use that allow URIs to be layered over existing netCDF file metadata, providing Linked Data views on the file contents.

The project landing page is found [here](https://binary-array-ld.github.io/netcdf-ld/).

netCDF-LD is being developed by the a working group consisting of members of CSIRO, UK Met Office, NOAA, NCI, Geoscience Australia and others. The working group is contributing to a stream of activity under the [Advancing netCDF-CF for the Geoscience Community](https://www.earthcube.org/content/advancing-netcdf-cf-geoscience-community) (or see the [Github repo wiki](https://github.com/Unidata/EC-netCDF-CF/wiki)). Participation is open. There is a set of relevant Github repositories and is the main collaboration site for this work.


### Credits

(Alphabetical order) Jim Biard (NOAA), Nicholas Car (GA), [Simon Cox (CSIRO)](https://github.com/dr-shorthair), Ethan Davis (UCAR), Kelsey Druken (NCI), Mark Hedley (UK Met. Office), Alex Ip (GA), Adam Leadbetter (Marine Inst.), [Jonathan Yu (CSIRO)](https://github.com/jyucsiro)

We also acknowledge contributions from: Stefano Nativi, and Aaron Sweeney.