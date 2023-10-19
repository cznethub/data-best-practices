# Best Practices for Sharing Geospatial Data

## What are geospatial data?

Geospatial data are related to a specific location on the Earth’s surface. Geospatial data typically combine location information with attribute information (data or information about the locations). Geospatial data may have a time component and typically conform to one of several well known geospatial data models for vectors (e.g., shapefiles, feature classes, KML/KMZ, etc.), rasters (e.g., land cover, digital elevation data, aerial imagery, etc.), and other geographic information (e.g., LiDAR point clouds). Geospatial data may also include locations with horizontal (e.g., latitude/longitude) and vertical (i.e., elevation) coordinates.

## Repositories for Sharing Geospatial Data

We recommend sharing geographic feature, geographic raster, and multidimensional space time (NetCDF) geospatial data in the [HydroShare repository](http://hydroshare.org). You can submit your data to HydroShare directly through the submission page for HydroShare in this Data Submission Portal. If you need help with using HydroShare, visit the [HydroShare help system](http://help.hydroshare.org). You can also learn about the geographic feature, geographic raster, and multidimensional NetCDF Content Types in HydroShare at [https://help.hydroshare.org/hydroshare-resources/content-types/](https://help.hydroshare.org/hydroshare-resources/content-types/).

For high resolution topography data (i.e., LIDAR data), we recommend using the [OpenTopography repository](https://opentopography.org/). OpenTopography facilitates community access to high-resolution, Earth science-oriented topography data along with related tools and resources. See OpenTopography’s information on contributing data at [https://opentopography.org/data/contribute](https://opentopography.org/data/contribute).

If you feel that your geospatial data are not a good fit for the HydroShare repository, you can also deposit your data in the [Zenodo repository](http://zenodo.org).

## Metadata for Describing Geospatial Data

The geospatial data community has a long history of standards development for geospatial metadata. For example, see the Federal Geographic Data Committee’s (FGDC) geospatial metadata standards and guidelines at [https://www.fgdc.gov/metadata/geospatial-metadata-standards]( https://www.fgdc.gov/metadata/geospatial-metadata-standards). Metadata describing geospatial datasets usually conform to one of these existing standards. Generalized data repositories like HydroShare and Zenodo use high level metadata to describe resources (e.g., HydroShare uses the standard elements from the Dublin Core metadata standard) for the purposes of data cataloging and discovery and do not have many of the specific metadata elements needed to sufficiently describe geospatial data. You should think of the high-level metadata used by a repository like HydroShare as the metadata required to find and access the data, whereas the more detailed metadata required for a prospective user to understand the data and decide how and/or whether it can be used for a particular purpose should be included in a separate metadata file that is uploaded with the data. Given this, we strongly recommend that you include a metadata file with each geospatial dataset that describes at minimum:

* The spatial reference system used by your geospatial data
* Definition of the data set entities and attributes - i.e., what are the features in your dataset and what are their attributes, including units
* Methods/manipulations/transformations/processing – include processing, methods, tools used, transformations applied, normalization, etc. that were used to format data layers for analysis. Also describe specific software used.

For resource-level metadata in HydroShare or Zenodo (the metadata that will support discovering your geospatial data), we recommend creating titles, abstracts, keywords, and other high level metadata that will help prospective data users discover your resource. Be brief but descriptive with your title, and include useful information in your abstract. Choose keywords that you think people who may be interested in your data will use to search for it, which may include place names, observed variables, topics, etc. Keep in mind that the more detailed geospatial metadata you provide as part of the resource’s content files will not be indexed for discovery purposes. Users will be able to download the file and use the metadata to help them interpret your data, but it will not help them find your data, which is why the resource-level metadata is so important.

## Formats for Sharing Geospatial Data

While we recommend the formats below for geospatial data, we recognize that there may be instances where you may want/need to use other formats. While HydroShare provides value-added functionality for the known formats listed above, the repository also accepts data in any format. Similarly, Zenodo is format agnostic.

### Geographic Feature Datasets

For geographic feature datasets (points, lines, or polygons), we recommend using the ESRI shapefile format. The shapefile format is a mostly open format that can be used with many different geographic information system (GIS) software programs. When you upload a shapefile, HydroShare has some value-added functionality that will automatically extract some metadata and display it on the resource landing page. For public resources, HydroShare will also build an Open Geospatial Consortium (OGC)-compliant web map service using a HydroShare-linked GeoServer. A link to this service will appear on the landing page for the resource and can be used to load your feature data into any GIS client that knows how to access web map services.  Learn more about how HydroShare handles geographic feature data: [https://help.hydroshare.org/hydroshare-resources/content-types/geographic-feature/](https://help.hydroshare.org/hydroshare-resources/content-types/geographic-feature/).

Two additional good options for geographic feature data include simple comma separated values (.csv) files that can be used to store location data (e.g., x, y, and z coordinates), or Keyhole Markup Language (.kml or .kmz) files that can be used with Google Earth, Google Maps, and some other GIS software programs. You can share both CSV and KML/KMZ data in HydroShare, but you will not get the value-added functionality described above for shapefiles. These formats are also compatible with Zenodo and other repositories.

### Geographic Raster Datasets

For geographic raster datasets (regularly spaced gridded data) we recommend using the GeoTIFF format. GeoTIFF is an open data format for encoding raster data within a TIFF file. Georeferencing information for the raster dataset can be embedded within the dataset. When you upload a GeoTIFF file, HydroShare will automatically extract some metadata and display it on the resource landing page. For public resources, HydroShare will also build an OGC compliant web map service using a HydroShare-linked GeoServer. A link to this service will appear on the landing page for the resource and can be used to load your feature data into any GIS client that knows how to access web map services. Learn more about how HydroShare handles geographic raster data: [https://help.hydroshare.org/hydroshare-resources/content-types/geographic-raster/](https://help.hydroshare.org/hydroshare-resources/content-types/geographic-raster/).

An additional raster format you may consider is the ASCII grid format. The ASCII format it text-based, which may make file sizes larger and processing slower. However, the ASCII grid format is open, cross platform compatible, and can be used in non-geospatial software programs like R or Python (although there are packages for R and Python for working with many geospatial data formats).

### Multidimensional Space Time Datasets

For multidimensional space time datasets (e.g., data that include three spatial dimensions (e.g., x, y, and z), a time dimension, and other user-defined dimensions), we recommend using the Network Common Data Form (NetCDF) format. Learn more about how HydroShare handles multidimensional data - [https://help.hydroshare.org/hydroshare-resources/content-types/multidimensional/](https://help.hydroshare.org/hydroshare-resources/content-types/multidimensional/).

Some multidimensional data can be very large. HydroShare has a practical limit for uploading files through its web user interface of 1-2 GB per file. There are options for getting larger files into HydroShare – see the HydroShare help at [https://help.hydroshare.org/creating-and-managing-resources/uploading-large-files-into-hydroshare/](https://help.hydroshare.org/creating-and-managing-resources/uploading-large-files-into-hydroshare/). If you have a large volume of data to share (that will exceed your HydroShare user quota) or you have very large files (> 2 GB) to share, we recommend that you contact a member of the CZ Hub team to consider the best options for sharing.

### Other Geospatial Data

If you need to upload high resolution topography data to OpenTopography, consult their tutorial [https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/CommunityDataspaceTutorial.pdf](https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/CommunityDataspaceTutorial.pdf) and metadata template [https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/MetaDataTemplate.docx](https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/MetaDataTemplate.docx). OpenTopography accepts high resolution topography data derived from both LiDAR and photogrammetry. According to their tutorial, OpenTopography accepts point clouds in LAS or LAZ format, with LAZ being preferred because of their reduced size. They accept rasters in IMG and TIF format with the coordinate system inofrmation included in the file header. Extended metadata to describe data submitted to OpenTopography must be uploaded in PDF format. OpenTopography has a 10GB size limit on a single submission. Datasets larger than this can be broken into multiple submissions.

## Organizing Data for Sharing

Organizing data for sharing requires several considerations that can be boiled down to questions about how to “chunk” the data into a set of resources in a repository and a set of files within those resources that are shared within prospective data users. Some of the important considerations include:

* **How do you want the data to be discovered and accessed?** Data discovery operates at the granularity of a resource (i.e., a HydroShare resource or a Zenodo resource). If you want two datasets to be separately discoverable with separate metadata, they should be shared in separate resources, each one having its own metadata description.
* **How do you want the data to be cited?** You should think of your data as research products that can be cited. Each resource in HydroShare and Zendodo has a separate citation and can be published with a digital object identifier (DOI). You may choose to organize data into a set of resources based on how you want them to be cited as products.
* **How will the data be used?** If you know investigators will want to use the data in a particular way, you may want to organize the data into a set of files that will make that easier – e.g., assembling all of the data required to reproduce a specific set of results into a single resource.
* **What is practical for managing the data?** If some of your content is dynamically updating (e.g., streaming sensor data) while other content is static, you will likely want to manage those datasets in separate resources.

## Additional Best Practices for Geospatial Data

The following recommendations are not meant to represent an exhaustive list but will provide relevant guidance. If you have specific questions about your geospatial data, please feel free to contact us.

* **Choose a consistent geospatial metadata standard**: Choose a consistent geospatial metadata standard for all of your geospatial data. Make sure that you submit supplemental geospatial metadata files with your data to the repository.
* **Choose a consistent spatial reference system**: Don’t count on the ability of your GIS software to do projection on the fly. Users of your data may be accessing subsets or all of your data and may or may not have access to the software you used to produce the data. A consistent spatial reference system makes it easier for people to use your data.
* **Share your data using open data formats**: Use the open data formats suggested above or another open data format to share your final data products. While you may need to use specific software and/or data formats for your analyses, it is common for potential data users to not have access to expensive, proprietary software. Using open formats that can be opened using a variety of GIS software to share the inputs and outputs of your analyses will enable the greatest access to the data and facilitate reuse.
