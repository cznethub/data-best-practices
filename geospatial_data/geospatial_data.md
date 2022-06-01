# Best Practices for Sharing Geospatial Data

## What are geospatial data?

Geospatial data are related to a specific location on the Earth’s surface. Geospatial data typically combine location information with attribute information (data or information about the locations). Geospatial data may have a time component and typically conform to one of several well known geospatial data models for vectors, rasters, and other geographic information.

## Repositories for Sharing Geospatial Data

We recommend depositing geographic feature, geographic raster, and multidimensional space time (NetCDF) geospatial data in the [HydroShare repository](http://hydroshare.org). You can submit your data to HydroShare directly through the submission page for HydroShare in this Data Submission Portal. If you need help with using HydroShare, visit the [HydroShare help system](http://help.hydroshare.org). You can also learn about the geographic feature, geographic raster, and multidimensional NetCDF Content Types in HydroShare at [https://help.hydroshare.org/hydroshare-resources/content-types/](https://help.hydroshare.org/hydroshare-resources/content-types/).

For high resolution topography data (i.e., LIDAR data), we recommend using the [OpenTopography repository](https://opentopography.org/). OpenTopography facilitates community access to high-resolution, Earth science-oriented topography data along with related tools and resources. See OpenTopography’s information on contributing data at [https://opentopography.org/data/contribute](https://opentopography.org/data/contribute).

If you feel that your geospatial data are not a good fit for the HydroShare repository, you can also deposit your data in the [Zenodo repository](http://zenodo.org).

## Metadata for Describing Geospatial Data

The geospatial data community has a long history of standards development for geospatial metadata. Metadata describing geospatial datasets usually conform to one of these existing standards. Generalized data repositories like HydroShare and Zenodo use high level metadata to describe resources (e.g., HydroShare uses the standard elements from the Dublin Core metadata standard) for the purposes of data cataloging and discovery and do not have many of the specific metadata elements needed to sufficiently describe geospatial data. Given this, we strongly recommend that you include a metadata file with each geospatial dataset that describes at minimum:

* The spatial reference system used by your geospatial data
* Definition of the data set entities and attributes - i.e., what are the features in your dataset and what are their attributes, including units

For resource-level metadata in HydroShare or Zenodo, we recommend creating titles, abstracts, keywords, and other high level metadata that will help prospective data users discover your resource. The more detailed geospatial metadata you provide as part of the resource’s content files can be used by data users to interpret the data.

## Formats for Sharing Geospatial Data

**Geographic Feature Datasets**: For geographic feature datasets (points, lines, or polygons), we recommend using the ESRI shapefile format. The shapefile format is a mostly open format that can be used with many different geographic information system (GIS) software programs. When you upload a shapefile, HydroShare will automatically extract some metadata and display it on the resource landing page. For public resources, HydroShare will also build a web map service using a HydroShare-linked GeoServer. A link to this service will appear on the landing page for the resource and can be used to load your feature data into any GIS client that knows how to access web map services.  Learn more about how HydroShare handles geographic feature data: [https://help.hydroshare.org/hydroshare-resources/content-types/geographic-feature/](https://help.hydroshare.org/hydroshare-resources/content-types/geographic-feature/).

**Geographic Raster Datasets**: For geographic raster datasets (regularly spaced gridded data) we recommend using the GeoTIFF format. GeoTIFF is an open data format for encoding raster data within a TIFF file. Georeferencing information for the raster dataset can be embedded within the dataset. When you upload a GeoTIFF file, HydroShare will automatically extract some metadata and display it on the resource landing page. For public resources, HydroShare will also build a web map service using a HydroShare-linked GeoServer. A link to this service will appear on the landing page for the resource and can be used to load your feature data into any GIS client that knows how to access web map services. Learn more about how HydroShare handles geographic raster data: [https://help.hydroshare.org/hydroshare-resources/content-types/geographic-raster/](https://help.hydroshare.org/hydroshare-resources/content-types/geographic-raster/).

**Multidimensional Space Time Datasets**: For multidimensional space time datasets (e.g., data that include three spatial dimensions (e.g., x, y, and z), a time dimension, and other user-defined dimensions), we recommend using the Network Common Data Form (NetCDF) format. Learn more about how HydroShare handles multidimensional data - [https://help.hydroshare.org/hydroshare-resources/content-types/multidimensional/](https://help.hydroshare.org/hydroshare-resources/content-types/multidimensional/).

** Other Geospatial Data** : If you need to upload high resolution topography data to OpenTopography, consult their tutorial [https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/CommunityDataspaceTutorial.pdf](https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/CommunityDataspaceTutorial.pdf) and metadata template [https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/MetaDataTemplate.docx](https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/MetaDataTemplate.docx).

While we recommend the above formats for geospatial data, we recognize that there may be instances where you may want/need to use other formats. While HydroShare provides value-added functionality for the known formats listed above, the repository also accepts data in any format. Similarly, Zenodo is format agnostic.

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
* **Use open data formats**: Use the open data formats suggested above or another open data format. It is common for potential data users to not have access to expensive, proprietary software. Use formats that can be opened using a variety of GIS software.
