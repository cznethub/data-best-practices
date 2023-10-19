# Best Practices for Sharing and Publishing CZNet Data

The CZ Hub Team has developed a Data Submission Portal (https://contribute.criticalzone.org) to meet the needs of the CZ Collaborative Network (CZNet). The Data Submission Portal provides guidance regarding which data repositories into which products should be deposited and also provides functionality that allows submission of data to the appropriate repository through the Portal. We recommend that all data and research products be submitted to the appropriate repository through the Portal, where possible. We provide the following additional guidance for submitting data for sharing and publication.

## Content of this General Best Practice Document

* [How to Contact Us](#how-to-contact-us)
* [Which repository should I use?](#which-repository-should-i-use)
* [General Guidance for all CZNet Data and Research Products to be Submitted](#general-guidance-for-all-cznet-data-and-research-products-to-be-submitted)
* [Specific Guidance for CZNet Data and Research Products](#specific-guidance-for-cznet-data-and-research-products)
* [Construct a Descriptive Title for Your Data Product](#construct-a-descriptive-title-for-your-data-product)
* [Create a Descriptive Abstract for your Data Product](#create-a-descriptive-abstract-for-your-data-product)
* [Select Keywords for your Data Product](#select-keywords-for-your-data-product)
* [Provide Author Information](#provide-author-information)
* [Provide Spatial and Temporal Coverage Information](#provide-spatial-and-temporal-coverage-information)
* [Provide Funding Agency Information](#provide-funding-agency-information)
* [Use Common Quality Control/Data Levels](#use-common-quality-controldata-levels)
* [Use Consistent Missing Data Labels](#use-consistent-missing-data-labels-nodata-values)
* [Linking Datasets with Publications](#linking-datasets-with-publications)
* [Potentially Useful Data Management Resources](#potentally-useful-data-management-resources)


## How to Contact Us

If you need help with data management or have questions about the guidance provided here, you can contact us in a number of ways.

### Join Us in the CZNet Slack Workspace

The CZNet Slack workspace was established to foster communication between the thematic clusters and with the CZNet Hub team. If you haven’t joined the CZNet Slack workspace, we encourage you to join us there. There are specific channels set up within the workspace for topical discussions. If you would like to join the CZNet Slack workspace, please email us at [help@cuahsi.org](mailto:help@cuahsi.org).

### Contact Us Directly via Email

For specific questions about CZNet data management, please contact us at [help@cuahsi.org](mailto:help@cuahsi.org). Be sure to include “CZNet” in the subject line of the email you send. We will route these emails to the person(s) who we think can best answer your questions.

## Which Repository Should I Use?

Our initial focus in developing the CZ Hub Data Submission Portal and for this data publication guidance is on the repositories listed below. We anticipate adding support for additional repositories via the Data Submission Portal as resources allow us to add them. If the supported repositories listed below will not meet your needs, choose a trusted repository that follows international best practices by offering:

1. A public landing page for your dataset/research product.
2. A unique identifier, which may be a digital object identifier (DOI), and a **persistent URL (the URL does not change)** for accessing the landing page for your dataset/product.
3. A formal citation for your dataset/product.

You can find directories of data repositories at [https://www.re3data.org](https://www.re3data.org) and [https://fairsharing.org](https://fairsharing.org).

We provide the general guidance with regard to supported repositories below, but we are happy to discuss any questions you may have and make more specific recommendations:

1. [HydroShare](http://www.hydroshare.org): A general purpose repository for submitting water-science related datasets and models. Submit datasets, models, and other research products that are water-related. This includes time series of hydrologic observations, time series of data from weather stations, geospatial datasets, etc. HydroShare is flexible and allows upload of files having any format. HydroShare also includes a linked JupyterHub server if you wish to upload executable Jupyter Notebooks using Python or R with your content. For information about how to submit to HydroShare, you can access HydroShare’s help system at [https://help.hydroshare.org](https://help.hydroshare.org).
2. [EarthChem](http://www.earthchem.org): A repository for submitting data derived from material samples such as soil, sediment, pore water, or rock specimens; cores; and other physical objects. Primary focus is on geochemical, geochronological, petrological, and mineralogical data. EarthChem strongly recommends use of data submission templates available on the EarthChem web site ([https://earthchem.org/ecl/templates/](https://earthchem.org/ecl/templates/)) that provide guidance for properly documenting data quality and provenance. Though data can be contributed to the EarthChem Library in a wide range of formats ([https://ecl.earthchem.org/fileformat.php](https://ecl.earthchem.org/fileformat.php)), it always needs to be documented with relevant information regarding the analytical data quality. Submission guidelines for EarthChem can be accessed at [https://www.earthchem.org/ecl/submission-guidelines/](https://www.earthchem.org/ecl/submission-guidelines/). For help, go to [https://earthchem.org/resources/support/earthchem-library-documentation/](https://earthchem.org/resources/support/earthchem-library-documentation/) or write to [info@earthchem.org](mailto:info@earthchem.org). Regardless of whether you submit directly to the EarthChem Library or you submit to the EarthChem Library through the CZNet Data Submission Portal, you shoud review and use the templates and guidance for your data files linked here.
3. [Zenodo](http://www.zenodo.org): A catch-all repository that may be an appropriate place to upload content that is not appropriate for the other repositories. Zenodo does not limit what you can upload and is not domain specific. For more information about Zenodo and submitting data, see [https://zenodo.org/record/787445](https://zenodo.org/record/787445).
4. [SESAR](https://www.geosamples.org): A sample registry that catalogs sample metadata, sample images, and other information to make samples more discoverable, accessible, and reusable. SESAR allows you to get an IGSN for your samples, a globally unique identifier that is essential for unambiguously citing samples in datasets and publications ([https://www.igsn.org](https://www.igsn.org)). Use SESAR to submit metadata about your samples and obtain IGSN Global Sample Numbers. Resources for researchers can be accessed at [https://www.geosamples.org/resources/researchers](https://www.geosamples.org/resources/researchers), and tutorials and FAQs can be accessed at [https://www.geosamples.org/resources/help](https://www.geosamples.org/resources/help).
5. [OpenTopography](https://opentopography.org): A repository that facilitates community access to high-resolution, Earth science-oriented, topography data and related tools and resources. Submit high resolution topography data acquired with lidar and other technologies. A tutorial describing how to submit data to OpenTopography can be accessed at: [https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/CommunityDataspaceTutorial.pdf](https://cloud.sdsc.edu/v1/AUTH_opentopography/www/docs/CommunityDataspaceTutorial.pdf).

If you choose to submit your data or research products to a repository other than the ones listed above, we will still need to know about those submissions. Please register these datasets with the CZNet Data Submission Portal.

Please see our specific guidance for CZNet data and research products below for information on what to do if you submit to a different repository.

## General Guidance for all CZNet Data and Research Products to be Submitted

We offer the following general guidelines for submitting your data and other research products. For a full overview, [click here](https://criticalzone.org/uploads/publications/Data-Products-Guide-CZhub.pdf).

1. **Use the Best Practices and Templates Described in this Repository**: Please follow the specific best practices, data formats, and templates described in this repository.
2. **Start assembling your data now**: We recommend that you begin thinking about which products (e.g., data, images, samples, code) you will generate. Assemble and document them as early as possible after generating them (it will save you time later), and register them within one of the above repositories. You need not wait until your data are ready for formal publication. HydroShare, EarthChem, and Zenodo all offer the ability to upload private content, allowing you to capture and store your data safely while your research and publication process is ongoing. Then share and publish when you are ready. Register your samples online in SESAR.
3. **Create a descriptive title for your data product**: Put some thought into the title of your dataset. See the guidance in the section below about how to construct a descriptive title for your dataset.
4. **Tag your data with appropriate metadata**: Use the repository’s submission form and templates to enter descriptive metadata for your products. Metadata should include information needed to discover and cite your products, but also additional information required to interpret your content (e.g., procedures used to collect or analyze samples or observations).
5. **Use common, open, and accepted data formats**: We know that the data you are creating are diverse and that there is not always specific guidance for how to organize your data and which file formats to use. We have provided some links to general data management resources in the section at the end of this document. If you have questions about what to do, please contact us.
6. **Include a “readme” file**: A readme file can include detailed information about the structure or content of your data or research product. It can also be used to describe how to perform specific analyses to make your research results more reproducible. If you upload a "readme.txt" or "readme.md" file to your resource in HydroShare, it will be displayed on the landing page for your resource. Using "readme.md" allows you to use markdown formatting in your readme file that will be rendered on the landing page for the resource.

We have included links to additional documentation that may assist you in preparing your datasets and research products for sharing and publication. We are always happy to discuss specific questions you may have.

## Specific Guidance for CZNet Data and Research Products

The CZ Hub Team is providing a coordinated view of all CZNet data/research products submitted to reputable data repositories via the CZnet Cataloging and Discovery system [https://discover.criticalzone.org](https://discover.criticalzone.org). We are using specific information from the metadata of the resources you submit to find and catalog resources submitted to the different repositories (see below). If the information we request below is missing, we may not be able to find your submitted resource and include it in the CZNet metadata index and discovery tools - or, your resource may not respond to the different search and filtering tools we have provided.

**NOTE**: The CZNet Data Submission Portal guides you to provide the following information to be entered for all datasets and products submitted through the Portal. However, we know that some may choose to submit directly to a repository without using the Data Submission Portal, so it is important to specify this information regardless of how or when you submit your data.

To accomplish this, we ask that you do the following, regardless of which repository you deposit your data in:

1. Tag your dataset/product with the subject keyword “CZNet”.
2. Tag your dataset/product with a subject keyword that is unique to your Thematic Cluster project. Use this keyword consistently for all products you share.
3. Ensure that you enter funding information, including funding agency (National Science Foundation), award number, and, if possible given the metadata elements available, award title. See the additional recommendations below for funding agency information.
4. Make sure that your dataset is publicly available. HydroShare, EarthChem, and Zenodo enable private content. We may not be able to discover and catalog your datasets/products until you have made them publicly available.

### Guidance for HydroShare, EarthChem, and Zenodo

We will be using “community” and “group” functionality within the different repositories to help group and present data from the cluster projects. When you submit to HydroShare, EarthChem, or Zenodo, we ask that you associate your dataset/product with an appropriate Group or Community, depending on which repository you submit to:

* **HydroShare** - share your dataset/product with your Cluster’s HydroShare Group. We have created a HydroShare “Group” for each thematic cluster project. You can share your HydroShare resource with your Group by clicking on the “Manage Access” button on the resource’s landing page and giving view or edit access to your cluster’s group. This can be done at any time after you create your resource in HydroShare.
* **EarthChem** - associate your dataset/product with the “Critical Zone” community within EarthChem. See [https://earthchem.org/communities/cznet/](https://earthchem.org/communities/cznet/)
* **Zenodo** - associate your dataset/product with the “Critical Zone Data and Research Products” community ([https://www.zenodo.org/communities/czdata/](https://www.zenodo.org/communities/czdata/)). When you create a new upload, search for “czdata” or “Critical Zone Data and Research Products” to find the correct community.

### Guidance for Data/Products Submitted to Other Repositories

We know that our list of supported repositories may not meet the needs of all of the CZNet cluster projects for all of the different types of data products. If you choose to submit your data/product(s) to a repository other than the ones in our list of supported repositories, we will be unable to discover and catalog those products unless you tell us about them. Please make sure that you register these data products with the CZNet Data Submission Portal. 

## Construct a Descriptive Title for Your Data Product

One of the most important metadata elements for your data product is the title. This piece of information is cataloged to enable discovery of your data product, and it is also included in the citation for your dataset. Anyone who uses your data product will cite your data using the title you construct. Consider the following suggestions when constructing a title for your data product:

* Make your title brief, but descriptive of the contents of the dataset. Since data products are first class research products - consider giving your data product a title that is similar to the type of title you construct for your journal papers.

> Example: Seasonal changes in organic matter composition and nutrients in coastal urban canals of Miami-Date County, Florida

* You may want to include a geographic area, site name or code, or an indication that the data product is affiliated with your thematic cluster project in the title.

> Example: Air temperature data for Dead Run watershed, Baltimore County, MD, USA

* Consider including brief information about the content of your data product in the title.

> Example: Watershed boundaries, hydrography, stream gage locations, and impervious surface area shapefiles for Pennypack Creek watershed in Bucks, Montgomery and Philadelphia Counties, PA, USA

* Avoid including acronyms in your title.
* Avoid including special characters (e.g., "&", "+", "%", or characters that are reserved for programming languages) in your title.
* Avoid including metadata in your title that belongs in other metadata fields. Try not to overload your title by concatenating a bunch of information into a cryptic title that nobody will understand.
* If your data product is specifically tied to a journal publication (i.e., it contains the exact data used in that publication), consider titling your data product similar to "Supporting data for X" where "X" is the title of the related publication. If you anticipate that your data product will be used by multiple journal publications, a more generic title would be better.

>Example: Supporting data and tools for "Impact of data temporal resolution on quantifying residential end uses of water"

## Create a Descriptive Abstract for your Data Product

The Abstract for your data product is important as it's likely the first (and perhaps last) piece of information a prospective user of your data will read before making a determination of whether they want to spend any more time evaluating or accessing your dataset. In general, you should approach writing the abstract for your data product in the same way you would approach writing the abstract for a journal or conference paper. In general, your Abstract should be a single paragraph, and may include the following elements:

* Brief background information, if needed
* Brief description of what the resource contains - what data are in the resource?
* Brief description of the purpose of the data - why was it produced/collected?
* Brief description of your research design and methods - how was the data produced/collected?
* Brief description of location - NOTE: Detailed descriptions of data collection sites and locations should be included in a readme file and/or in a data file or shapefile in your content files.
* Brief description of the variables observed - NOTE: Also consider adding these as keywords.
* Brief information about what the data show - e.g., what results have been derived from the data?
* Brief statement of how the data might be useful or how it might be used

Avoid the following when creating your Abstract:

* Overloading the Abstract with metadata that belongs elsewhere. For example:
  * Do not put citations for related resources in the Abstract, use the Related Resources metadata instead
  * Put funding agency information in the Credits/Funding Agency metadata rather than in your abstract
* Going too in depth into the description or structure of your resource - use a readme file for that instead
* Using complex formatting - this is usually lost when being transferred among different systems* 

## Select Keywords for your Data Product

Keywords are important metadata that help categorize and describe your data product. They are also important in enabling other scientists and prospective data users to discover your data product. Use the following guidelines to select appropriate keywords to describe your dataset:

* Tag your dataset/product with the subject keyword “CZNet” (see specific guidance for CZNet data products above).
* Tag your dataset/product with a subject keyword that is unique to your Thematic Cluster project. Use this keyword consistently for all products you share (see specific guidance for CZNet data products above).
* Add keywords that describe the subject of your data product (e.g., "Critical Zone", "Streamflow", "Water quality").
* Add keywords that describe the geographic area to which your dataset applies (e.g., "Utah", "Logan River Watershed")
* Capitalize the first letter of keywords. If your keyword is a phrase, capitalize only the first word (e.g., "Water quality"). If your keyword is a proper name, capitalize the first letter of each word (e.g., "Logan River Watershed").
* Avoid misspelling or using variants of the same keyword (e.g., use "Temperature" consistently rather than "Temp.")
* Full phrases will have more meaning, but add acronyms if you want to enable discovery using that term. For example "Logan River Observatory" is more informative than "LRO", but some users may want to search using "LRO". In this case you may want to add both.
* Keywords may be a single word or several words (e.g., phrases), but keep them very brief. This isn't the place for sentences.
* Choose keywords that are commonly used to describe the type of data product you are describing.
* Avoid special characters (e.g., characters reserved for programming languages), abbreviations, and contractions. 
* Do not use punctuation.
* You may consider keywords that describe observed variables (e.g., "Temperature", "Nitrogen"), and/or methods used to produce the data product. However, avoid using units in your keywords (e.g., use "Discharge" not "Discharge (m3/s)"). 
* Where you choose keywords describing observed variables, consider selecting them from the ODM2 VariableName controlled vocabulary [http://vocabulary.odm2.org/variablename/](http://vocabulary.odm2.org/variablename/).
* You may consider using keywords that have been used by other, similar data products to ensure that they can be discovered together. You can even test this by searching HydroShare, EarthChem, or other repositories using specific keywords to see what is returned before you select your final set of keywords.

Remember - the keywords you use to describe your data product will be part of the metadata that is cataloged and used to enable discovery of your data product. Choose keywords that you think will help people find your data product. Leave all of the other descriptive metadata for the other descriptive metadata elements (e.g., Title, Abstract, etc.).

## Provide Author Information

Given that data are considered primary products of research that are citable for scholarly credit, it is important that you provide full author information for the data/research products that you deposit into a data repository. Author information ends up in the citation for resources and is also included in the CZNet data discovery capabilities, so it is also important that Author information is specified consistently across all submitted resources with which an Author is affilated. For resources submitted through or registered with the Data Submission Portal, we suggest the following format for Author names:

> Family, Given

For example:

> Horsburgh, Jeffery S.

The researchers you work with may have standardized on a particular way of expressing their name so that all scholarly products are correctly attributed to them. We encourage anyone who is submitting resources on behalf of another party (e.g., Cluster Data Managers) to check with investigators to ensure that Author names are expressed correctly prior to permanently publishing resources. Once a resource is published and a DOI is issued, author information generally cannot be changed.

It is best practice to also provide affiliation information for each author. Affiliations should be specified as the affiliation under which the resource was created. We recommend that Data Managers work with authors to ensure that affiliation information is entered correctly and consistently (e.g., use the same Organization Name, Address, etc. for each resource with which an Author is affiliated to avoid ambiguity).

## Provide Spatial and Temporal Coverage Information

Spatial and temporal coverage information is important for people who may be searching for data collected within or near a particular place or region and/or that were collected within or are representative of a specific time period. The purpose of coverage information is not to visualize the spatial or temporal qualities or complexity of your data. Instead, it is meant to provide viewers with information about where the spatial and/or temporal region to which the data are applicable. The following are recommendations for specifying spatial and temporal coverage for the different repositories supported by CZNet:

* **HydroShare**: HydroShare represents spatial coverage information as a bounding box or a discrete point in space. You can choose which to use, and you can input the coordinates for the bounding box or point manually or by using the map control to draw the point or box on the map. HydroShare allows you to enter the temporal coverage as a time period by choosing a starting and ending date. 
* **EarthChem**: The EarthChem repository allows you to specify the spatial coverage as "Global", "Regional (Continents, Oceans)", or "Space/Planetary" along with adding geographic keywords. EarthChem then draws coverage information from the coordinates associated with the dataset's individual samples. Samples must be registered with SESAR and receive IGSNs for this association to work correctly. 
* **Zenodo**: The Zenodo repository does not include spatial or temporal coverage information as part of its metadata. If you want to share a resource in Zenodo and you want to specify spatial or temporal coverage information, you could add this information to the "Additional notes" metadata field in Zenodo.
* **Other Repositories**: If you are using the Data Submission Portal to register a dataset from a different repository, specifying the spatial and temporal coverage is the same as for the HydroShare repository.

**NOTE**: The CZNet Cataloging and Discovery system includes a filter for data temporal coverage. Given that specifying the temporal coverage of your dataset is optional, only datasets that have information for temporal coverage will respond to this filter. The CZ Hub team is also working spatial filtering capability, which, similar to temporal coverage, will only work for those datasets for which spatial coverage information is specified.

## Provide Funding Agency Information

It is best practice to provide an acknowledgment to the agency or funding source that provided the support under which data/research products were produced. For CZNet Thematic Cluster projects, this is the NSF award that funded the Cluster project. Several of the Thematic Cluster projects have collaborative awards, which means that there are multiple NSF award numbers.

We recommend that you provide full funding agency information for each data/research product that is submitted to a repository. For each product, you should provide the following information:

* Agency Name - e.g., "National Science Foundation"
* Award Title - e.g., "Collaborative Research: Network Hub: Enabling, Supporting, and Communicating Critical Zone Research"
* Award Numver - e.g., "2012748"
* Funding Agency URL - e.g., "[https://www.nsf.gov/awardsearch/showAward?AWD_ID=2012748](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2012748)"

For those Thematic Cluster projects that have more than one NSF award, where appropriate we recommend adding multiple funding agency metadata elemements for each award. We also recommend this for products that may have been co-funded by multiple projects and/or agencies. You should include a funding agency element for each one.

The CZNet Catalog and Discovery system uses the NSF award numbers to match your data products to your Thematic Cluster project. Thus, if you want your data products to respond to the CZ Project filter in the Catalog and Discovery system, you must include at least one of your Thematic Cluster project's NSF award numbers in the funding agency metadata.

## Use Common Quality Control/Data Levels

We suggest a set of standardized quality control/data levels that can be used to describe data. These data levels are independent of data type. Including a specific data level as part of the metadata for a dataset will help potential users understand how the data can/should be used. Suggested data levels are listed in the following table.

| Level | Definition | Explanation |
| ----- | ---------- | ----------- |
| 0 | Raw data | Raw and unprocessed data and data products that have not undergone quality control. Depending on the variable, data type, and data transmission system, raw data may be available within seconds or minutes after the measurements have been made. Examples include real time precipitation, streamflow, and water quality measurements. |
| 1 | Quality controlled data | Quality controlled data that have passed quality assurance procedures such as routine estimation of timing and sensor calibration or visual inspection and removal of obvious errors. An example is USGS published streamflow records following parsing through USGS quality control procedures. |
| 2 | Derived products | Derived products that require scientific and technical interpretation and may include multiple-sensor data. An example is basin average precipitation derived from rain gages using an interpolation procedure. |
| 3 | Interpreted products | Interpreted products that require researcher driven analysis and interpretation, model-based interpretation using other data and/or strong prior assumptions. An example is basin average precipitation derived from the combination of rain gages and radar return data. |
| 4 | Knowledge products | Knowledge products that require researcher driven scientific interpretation and multidisciplinary data integration and include model-based interpretation using other data and/or strong prior assumptions. An example is percentages of old or new water in a hydrograph inferred from an isotope analysis. |

## Use Consistent Missing Data Labels (NoData Values)

Missing data labels, or NoData values, are values that you insert into your data to indicate that a value for an observation should exist but for some reason doesn't. Usually, these values are selected such that they are easily recognizable and out of the valid range of data values for whatever the observed variable is. We recommend the following practices for CZNet datasets
* If you use a NoData value, make sure you define it in associated metadata
* The preferred NoData value for CZNet datasets is -9999
* Don't mix strings and numeric values in a single data column. For example, don't insert a NoData value of "NA" into a numeric data column.
* Work to educate students, colleagues, and collaborators what -9999 means in a dataset to minimize potential errors in analyses.

## Linking Datasets with Publications

We strongly recommend creating formal linkages between the datasets you have deposited within the above mentioned repositories and any manuscripts that you submit for publication that use or are based on the data. This ensures that anyone who discovers the paper can link to and access the data used and anyone who discovers the data can link to and access publications that have used the data.

After depositing your datasets within one of the above repositories we recommend formally citing the data within any research manuscripts based on the data that you submit for publication. Recommendations in the Author Guide for the journal to which you submit may determine how datasets are cited in the text of the paper. In the absence of specific instructions from the journal, we recommend citing data within the text of the paper using the journal’s citation style (e.g., Author(s), Year) and including a full bibliographic citation to the dataset within the references section of the paper.

Once a paper has been accepted for publication and a digital object identifier (DOI) or citation has been issued for the paper, you should modify the metadata for the dataset in the repository to include a link to the paper as a “related resource.”

## Potentally Useful Data Management Resources

The following references are provided for publications that you may find useful in considering the data management needs of your thematic cluster as well as cross-cluster and other collaborations:

### Guidelines for Structuring and Formatting Data

Borer, E.T., Seabloom, E.W., Jones, M.B., Schildhauer, M. (2009). Some simple guidelines for effective data management, Bulletin Ecological Society of America, 90(2), 205-214, https://doi.org/10.1890/0012-9623-90.2.205

Broman, K. W., & Woo, K. H. (2018). Data Organization in Spreadsheets. The American Statistician, 72(1), 2–10. https://doi.org/10.1080/00031305.2017.1375989

Goodman, A., Pepe, A., Blocker, A. W., Borgman, C. L., Cranmer, K., Crosas, M., Di Stefano, R., Gil, Y., Groth, P., Hedstrom, M., Hogg, D. W., Kashyap, V., Mahabal, A., Siemiginowska, A., & Slavkovic, A. (2014). Ten Simple Rules for the Care and Feeding of Scientific Data. PLoS Computational Biology, 10(4), e1003542. https://doi.org/10.1371/journal.pcbi.1003542

Hart, E. M., Barmby, P., LeBauer, D., Michonneau, F., Mount, S., Mulrooney, P., Poisot, T., Woo, K. H., Zimmerman, N. B., & Hollister, J. W. (2016). Ten Simple Rules for Digital Data Storage. PLOS Computational Biology, 12(10), e1005097. https://doi.org/10.1371/journal.pcbi.1005097

Wickham, H. (2014). Tidy Data. Journal of Statistical Software, 59(10), Article 10. https://doi.org/10.18637/jss.v059.i10

### Guidelines for Citing Data

Colavizza, G., Hrynaszkiewicz, I., Staden, I., Whitaker, K., & McGillivray, B. (2020). The citation advantage of linking publications to research data. PLOS ONE, 15(4), e0230416. https://doi.org/10.1371/journal.pone.0230416

Guidelines for Making Data More Reusable

White, E., Baldridge, E., Brym, Z., Locey, K., McGlinn, D., & Supp, S. (2013). Nine simple ways to make it easier to (re)use your data. Ideas in Ecology and Evolution, 6(2), Article 2. https://doi.org/10.4033/iee.2013.6b.6.f

### Guidelines for Selecting a Data Repository

Sansone, S.-A., McQuilton, P., Cousijn, H., Cannon, M., et al (2020). Data Repository Selection: Criteria That Matter. Zenodo. https://doi.org/10.5281/zenodo.4084763
