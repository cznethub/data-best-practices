# Best Practices for Sharing Data Derived from Physical Samples

## Sample Metadata and Collection Management with Sesar

Samples are a critical element of research in nearly every science domain, especially in Earth, Environmental, and Planetary sciences. They represent highly valuable, often irreplaceable records of nature and carry enormous potential for future discoveries.

SESAR offers services to advance the management and sharing of samples in the Earth, Environmental, and Planetary Sciences.  By registering your samples with SESAR, you will:

* Create a catalog of your samples
* Ensure preservation of all information about your samples
* Allow researchers to discover your samples to start new collaborations
* Link your samples to your analysis data.

[MySESAR](https://app.geosamples.org/index.php) is your private working space in the System for Earth Sample Registration. MySESAR allows you to:

* Obtain IGSNs for your samples by registering them with SESAR.
* Register samples one at a time by entering metadata into a web form.
* Generate customized SESAR spreadsheet forms to register multiple samples at once.
* View and edit metadata profiles of samples that you have registered.
* Upload images and related documents such as field notes, maps, or links to publications to a sample profile.
* Transfer ownership of a sample to another SESAR user.
* Restrict access to metadata profiles of your samples.
* MySESAR functionality can be tailored to personal and institutional sample management.

## What is an IGSN?

As part of our registration services, SESAR is an ‘Allocating Agent’ for the IGSN e.V., the implementation organization of the IGSN. IGSN stands for [International Geo Sample Number](http://igsn.org/). The IGSN is an alphanumeric code that uniquely identifies samples taken from our natural environment (for example: rock specimens, water samples, sediment cores), as well as related sampling features (sites, stations, stratigraphic sections, etc.).
SESAR provides IGSN during the registration process, and maintains the metadata profile pages that IGSN ‘resolve’ to. In addition to the registration metadata required by the IGSN e.V., SESAR collects and maintains descriptive metadata unique to the SESAR community.
Except in special cases*, IGSNs obtained from SESAR are 9 characters long. IGSNs obtained from Allocating Agents other than SESAR may have different syntax, but all are guaranteed to be globally unique via a central registry.

Examples:

1. [IGSN: HRV003M16](http://app.geosamples.org/sample_display.php?sample_id=48658) (Registered object: Malachite specimen from Angola, registered by the Mineralogical Museum of Harvard University)
2. [IGSN: WHO000BC7](http://app.geosamples.org/sample_display.php?sample_id=76639)  (Registered object: Dredge CHAIN35-2 St18 D18, registered by the Woods Hole Oceanographic Institution)

## How do I Register Samples with SESAR?

SESAR provides three methods for registering samples:

* Individual Sample Registration
* Batch Registration
* Registration using Web Services.  

* Before registering your samples, you must create a SESAR account.  See our [Resources for Researchers](https://www.geosamples.org/resources/researchers) and [Resources for Institutions](https://www.geosamples.org/resources/institutions) for more information on creating an account.

## Individual Sample Registration

Through the Individual Batch Registration method, SESAR users are able to register samples one at a time through an online form. This method of sample registration is best for when you have few samples that you would like to register.

To Individually Register a sample:

1. Login to [MySESAR](https://app.geosamples.org/index.php)
2. Click the “Register an individual sample” link under the “Registration” header on the home page.
3. Follow the prompts to fill in the sample’s metadata in the sample registration forms. Once complete, click ‘Submit to SESAR’.

## Batch Registration
Through the Batch Registration method, SESAR users are able to register multiple samples at once by uploading a sample batch registration template. This method of sample registration is best for when you are registering multiple samples. It also provides additional quality checks as submissions are reviewed by SESAR curators. To create a Batch Registration template see this tutorial.

To upload a batch template:

1. Login to [MySESAR](https://app.geosamples.org/index.php)
2. Click “Upload my batch samples” under the “Registration” header on the home page
3. Upload your Batch Registration template, complete the automated validation check, and submit it.

After submission, your sample metadata will be reviewed by a SESAR curator. SESAR curators review template contents for accuracy (is your location information in the right format?) and completeness (one row had a blank field, was that in error?). Once your submission has been approved, you will receive an email confirmation along with your completed Batch file. If there are any changes that need to be made to your template a SESAR curator will contact you.

## Web Services Registration

SESAR provides Web Services as a way for user client programs to register and update samples within the SESAR system. Starting in July 2021, new users must request access to SESAR’s Web Services. Documentation for Web service sample registration and management can be found in our technical documentation (SESAR GitHub).

## Repositories for Sharing Data Derived from Samples

We recommend depositing data derived from samples in the [EarthChem Library])(https://www.earthchem.org/ecl/) repository. You can submit your data to EarthChem directly through the submission page for EarthChem Library (ECL) in this Data Submission Portal.

If you need help with using the ECL, go to [https://www.earthchem.org/resources/support/earthchem-library-documentation/](https://www.earthchem.org/resources/support/earthchem-library-documentation/).

## Metadata for Describing Data Derived From Samples

At a high level, metadata associated with data derived from samples usually include:

* **Title**: Your dataset title must contain concise and descriptive information about the content of the dataset (the “what” and “where”, for example “Gakkel Ridge basalt melt inclusion and mineral chemistry”). If submitting data from a publication, the dataset title may be the same as your publication title, but likely will be different since your ECL dataset will paint a different story than your full publication.
* **Abstract**: Your abstract must describe in full sentences the measurements, location, and purpose of the dataset. The abstract should be <250 words and different from your related publication abstract. Avoid abbreviations and acronyms. Include relevant keywords, such as the geographic area or cruise or field program name, for example “This dataset presents analyses of volatile, major, and trace elements for a suite of glasses and melt inclusions from the 85 degrees E segment of the ultra-slow spreading Gakkel Ridge”.
* **Methods**: All analytes, units, and technique, instrument and laboratory  must be clearly stated and defined. Relevant standards, reference measurements, and additional information about instrument calibration should also be included when possible.
* **Sample names**: Every analyte must be linked to a sample with a  sample name and geospatial information (unless not applicable, i.e. experimental samples).
* **Identifiers**: We strongly recommend use of IGSNs (International Geo Sample Number) as persistent identifiers to identify samples.

If submitting a compilation dataset, the ECL requires a reference sheet or tab with full citations of all referred publications.

## Formats for Sharing Data Derived From Samples

If you are submitting tabular data it should be in an ECL template but must at the very least be in a .csv, .txt, or .xlsx file (not in .pdf, .docx, .jpeg, etc.). For more information on file formats please consult our [file policies](https://www.earthchem.org/ecl/policies/#files).

## Organizing Data for Sharing

We strongly recommend the use of [data submission templates](https://www.earthchem.org/ecl/templates/). Templates are available for various data types such as bulk analysis (majors, traces, isotopes), mineral analysis (in-situ analysis), and melt inclusion analysis. If a template does not yet exist for your data type, you may contact us about creating one at [info@earthchem.org](mailto:info@earthchem.org).

## Additional Best Practices for Data Derived From Samples

The following recommendations are not meant to represent an exhaustive list but will provide relevant guidance. If you have specific questions about your time series data, please feel free to contact us.

* **Vocabularies for describing sample data**: A list of recommended terms can ve accessed at https://www.earthchem.org/ecl/vocabularies/.
* **Release Date**: By default the release date is set to the date of submission. If this is not desirable, you may select a release date within the next two years. Every approved ECL dataset receives a DOI and is searchable in the ECL, even if the release date has not yet been reached. This allows investigators to submit datasets in compliance with data management policies of funding agencies and journals without releasing the actual data immediately.
* **Licenses**: Use of digital materials obtained from the EarthChem Library is licensed under varying Creative Commons licenses that can be selected by the data contributor. EarthChem Library strongly recommends use of the [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/) license. The license that is applicable for a given dataset can be found on its landing page. Contributors have 4 Creative Commons data file license options to choose from:
  * [Creative Commons — Attribution-ShareAlike 4.0 International — CC BY-SA 4.0 (default)](https://creativecommons.org/licenses/by-sa/4.0/)
  * [Creative Commons – Attribution 4.0 International – CC BY 4.0](https://creativecommons.org/licenses/by/4.0/legalcode)
  * [Attribution-NonCommercial-ShareAlike 4.0 International — CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
  * [Attribution-NonCommercial-ShareAlike 3.0 United States — CC BY-NC-SA 3.0 US](https://creativecommons.org/licenses/by-nc-sa/3.0/us/)
  * [CC0](https://creativecommons.org/share-your-work/public-domain/cc0/)
* **Funding Information**: We strongly encourage US-based researchers to link their NSF award numbers with their ECL datasets. This will allow tracking of datasets by Award number and show compliance with Data Management policies of funding agencies.
* **Related Publications**: It is very important for users accessing your data to be able to easily reach and credit your full publication.

