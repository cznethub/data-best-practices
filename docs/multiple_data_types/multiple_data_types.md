# Best Practices for Sharing Multiple Data Types Together

## Why would you want to share multiple types of data together?

Sometimes you need ways to group data of different types together so that they can be easily accessed or cited as one unit - e.g., all of the data used in a publication or all of the data for a particular site. There are a number of different options for doing this. This page provides some example scenarios (descriptions below) where grouping data may be required and examples of how this can be accomplished.

## Repositories for Sharing Multiple Data Types Together

The [HydroShare repository](http://hydroshare.org) provides the capability to upload multiple types of data to a single resource. Each resource in HydroShare can be shared, has a unique citation, and can be permanently published with the digital object identifier. HydroShare resources can have a folder/directory structure that allows you to easily organize and manage the contents of the resource. HydroShare also has a set of content types that provide value-added functionality for some data types. You can submit your data to HydroShare directly through the submission page for HydroShare in this Data Submission Portal.
If you need help with using HydroShare, visit the HydroShare help system at http://help.hydroshare.org.

The [Zenodo repository](http://zenodo.org) also provides the capability to upload multiple data types to a single resource. However, Zenodo does not currently support a folder/directory structure, so if you need folders to organize your data you will have to organize it how you want it on your machine, zip everything into a zip file, and then upload the zip file to Zenodo.

## Metadata for Describing Grouped Data

When you group data of different types together within a HydroShare or Zenodo resource, you are defining that grouping of data as a single “product”. You should provide metadata that describes that product, including a description of the contents of the resource and why the content was grouped together.  Because your resource may be organized using a folder/directory structure containing many files, you should strongly consider providing a readme file that describes the structure and content of the resource. If you place this readme file in the root directory of your HydroShare resource as “readme.md” or “readme.txt”, your readme file will be displayed on the landing page for your resource. Using “readme.md” allows you to use Markdown formatting in your readme file for things like section headers, bulleted/numbered lists, bold text, etc. Markdown formatting is displayed on the landing page in HydroShare.

## Formats for Sharing Grouped Data

Formats suggested for data grouped together into a single resource are the same as if those datasets were shared separately. See the other best practice documents for details.

## Organizing Data for Sharing

Organizing data for sharing requires several considerations that can be boiled down to questions about how to “chunk” the data into a set of resources in a repository and a set of files within those resources that are shared within prospective data users. Some of the important considerations include:

* **How do you want the data to be discovered and accessed?** Data discovery operates at the granularity of a resource (i.e., a HydroShare resource or a Zenodo resource). If you want two datasets to be separately discoverable with separate metadata, they should be shared in separate resources, each one having its own metadata description.
* **How do you want the data to be cited?** You should think of your data as research products that can be cited. Each resource in HydroShare and Zendodo has a separate citation and can be published with a digital object identifier (DOI). You may choose to organize data into a set of resources based on how you want them to be cited as products.
* **How will the data be used?** If you know investigators will want to use the data in a particular way, you may want to organize the data into a set of files that will make that easier – e.g., assembling all of the data required to reproduce a specific set of results into a single resource.
* **What is practical for managing the data?** If some of your content is dynamically updating (e.g., streaming sensor data) while other content is static, you will likely want to manage those datasets in separate resources.

## Scenarios for Sharing Multiple Data Types Together

### Scenario 1 - I need to share all of the data I used for a research publication to meet publisher requirements and to enhance the reproducibility of my work.

In this scenario, you may wish to group the set of data you used within a research publication together so that the data can be easily cited, accessed by readers of your paper, and potentially reused to reproduce your work.

**Option 1 - Put all of the data for the publication in one resource in HydroShare**

You can create a resource in HydroShare for the data associated with your publication. If you have multiple data types, you may choose to create a folder/directory structure within the resource for organizing your data (e.g., put geospatial data in a folder, time series data in a folder, etc.). Your HydroShare resource will have a single citation that you can add to the references section of your paper and cite in the text.

This option is useful if you want to have all of the data grouped together in one place with one citation. This option is also useful if you have code that goes with the data to perform analyses in your paper. For example, you may choose to include a Jupyter Notebook in your HydroShare resource that when launched into the CUAHSI Jupyter Hub server operates on the data in the resource to reproduce the results presented in the paper. This is easier to do if the data are all in one resource, but more advanced options are still available if you can’t put everything on one resource.

Example Hydroshare Resource associated with a publication with multiple content types:

Bastidas Pacheco, C. J., J. S. Horsburgh, J. Caraballo, N. Attallah (2021). Supporting data and tools for "An open source cyberinfrastructure for collecting, processing, storing and accessing high temporal resolution residential water use data", HydroShare, https://doi.org/10.4211/hs.aaa7246437144f2390411ef9f2f4ebd0

**Option 2 - Split the data into multiple resources in HydroShare**

In this option, you may have used multiple different datasets of different types in your publication, but there is no reason to put them in a single resource in HydroShare. In your paper, you will include each of the resources in your references section and cite them appropriately in the text of your paper.

This option is useful where you have multiple datasets that you may have used in your paper, but those datasets are more self-standing and may be reused and/or cited on their own. This option also maintains the discoverability of the different datasets as they will appear as separate products in searches.

Example paper that cites multiple HydroShare resources containing datasets that were used in the paper:

Mihalevich, B. A., Horsburgh, J. S., Melcher, A. A. (2017). High-frequency measurements reveal spatial and temporal patterns of dissolved organic matter in an urban water conveyance, Environmental Monitoring and Assessment, https://doi.org/10.1007/s10661-017-6310-y

**Option 3 - Create a “Collection” resource in HydroShare** 

Following Option 2, you may choose to create a Collection resource in HydroShare to group datasets together. Collection resources don’t store any content themselves, but rather store pointers to other HydroShare resources. So, if you’ve used multiple different HydroShare resources in your publication, you can create a collection resource to group them together. Just like other resources, Collection resources have a landing page and a citation so you can cite them if you choose.

Example collection resource in HydroShare:

Logan River Observatory (2021). Logan River Observatory Datasets, HydroShare, http://www.hydroshare.org/resource/def147fa06de4c67810586d45337b413

### Scenario 2 - I need a way to group data together for easier access and to preserve the context of my data collection.

Sometimes, you may want to group datasets together so that people can find them more easily, so that they can be accessed together and so that prospective data users can more easily understand the context of the data. Examples include grouping all of the data for a particular data collection site or all of the data for a particular project. This scenario is pretty similar to Scenario 1, with similar solutions (see above).

## Additional Best Practices for Sharing Multiple Data Types Together

The following recommendations are not meant to represent an exhaustive list but will provide relevant guidance. If you have specific questions about sharing multiple data types together, please feel free to contact us.

* **Use related resources metadata**: If the reason you are sharing multiple data types together is to group the data you used for a publication (or some similar use case), use the Related Resources metadata to provide a link to the paper. Best practice is to provide a full bibliographic citation for the paper or related resource if you can (e.g., author(s), year, title, journal, volume, issue, pages, URL-encoded DOI). You may also want to add references to other, related datasets or other resources on the Internet that are in some way related to the content you are sharing.
