# Best Practices for Sharing Environmental Time Series Data

## What are environmental time series data?

Environmental time series data consist of collections of observations obtained through repeated measurements of some phenomenon over time. Each observed value in a time series is indexed in time. Usually, time series data are collected using environmental sensors installed in situ. However, there are cases where time series data are produced by a simulation model or other methods. Examples of time series data include: soil moisture, precipitation, streamflow, temperature, dissolved oxygen concentration, groundwater level, etc. Each individual observation in a time series has a timestamp consisting of the date/time at which that observation was made.

## Repositories for Sharing Time Series Data

We recommend depositing time series datasets in the [HydroShare repository](http://hydroshare.org). You can submit your data to HydroShare directly but we recommend submitting your data through the CZNet Data Submission Portal.

If you need help with using HydroShare, visit the [HydroShare help system](http://help.hydroshare.org). You can also learn about the [Time Series Content Type in HydroShare](https://help.hydroshare.org/hydroshare-resources/content-types/time-series/).

## Metadata for Describing Time Series Data

At a high level, metadata associated with time series observations usually include:

* **Site**: The location at which the data were collected
* **Variable**: The observed variable or phenomena that was measured (e.g., water temperature)
* **Method**: The procedure used to make the observations (e.g., which sensor and how was it deployed)
* **Source**: The organization responsible for data collection
* **Data/Quality Control Level**: The degree of processing the observations have been subject to (e.g., raw versus quality controlled products versus derived products)

Metadata need to be shared with the time series data to enable proper interpretation of the observed data values. For more information about specific metadata for time series data, see the following references. These references describe an information model for time series data that can be implemented in a number of different ways (see Formats for Time Series Data below).

Horsburgh, J. S., Aufdenkampe, A. K., Mayorga, E., Lehnert, K. A., Hsu, L., Song, L., Spackman Jones, A., Damiano, S. G., Tarboton, D. G., Valentine, D., Zaslavsky, I., Whitenack, T. (2016). Observations Data Model 2: A community information model for spatially discrete Earth observations, Environmental Modelling & Software, 79, 55-74, https://doi.org/10.1016/j.envsoft.2016.01.010

Horsburgh, J. S., D. G. Tarboton, D. R. Maidment, and I. Zaslavsky (2008), A relational model for environmental and water resources data, Water Resources Research, 44, W05406, https://doi.org/10.1029/2007WR006392.

## Formats for Sharing Time Series Data

Time series data can come in many formats, but the data are usually stored in a table. It is strongly recommended that you share your data in non-proprietary formats. We provide two recommended options below:

### Option 1: Comma Separated Values (CSV) Files

ASCII text files, e.g., comma separated values (CSV) are a recommended format for sharing time series data. CSV files are simple text, non-proprietary, cross platform, and can be opened and read by many different software programs and programming languages (e.g., Python and R).

Best practices for formatting your time series data with CSV files include:

* Use a CSV text editor that will not change the formatting of your file, the line ending characters, or the format of the date/time values in your file. Good text editors for Mac include Sublime Text and BBEdit. Good text editors for PC include Sublime Text and Notepad ++.
* Include all relevant metadata as a header in each data file. For example, include descriptions of the site, variable, method, source, data level, and any data qualifiers in the header of the file.
* Precede header lines with a comment character “#” to make it easy for code to skip header lines when reading the file.
* Each line of the data file should have a single timestamp.
* Include only one type of data within a data column (e.g., date/time, floating point number, text string), and use standard formats within cells.
* Include only one value per table cell.
* Use standardized ISO 8601 formatted date/time strings – e.g., yyyy-mm-dd hh:mm:ss
* Describe any key word, code, or data formatting used in the data in the header. For example, if -9999 is used to represent nodata values, this should be described.
* Ensure that timestamps are unambiguous. This can be done in a number of ways, which may include specifying the local date/time, UTC date/time zone, and UTC offset as separate columns in the data table.
* Where data do not share the same timestamps or time spacing (e.g., values recorded every 5 minutes versus values recorded every 15 minutes), store the data in separate files.

The following examples are provided:

[Example 1 – Single file with one time series](examples/Example1_LR_Mendon_AA_WaterTemp_EXO_SourceID_1_QC_1.csv): Use this format when you want to include a single time series within one table in a single file. The time series may be of any length in the file. Site, variable, method, source, data level, and qualifier metadata are contained in the file header.

[Example 2 – Single file with multiple time series](examples/Example2_LR_Mendon_AA_SourceID_1_QC_0_Year_2022.csv): Use this format when you want to include multiple time series within the same table in a single file. The time series may be of any length in the file, but consider that your table may be sparsely populated if your time series do not begin and end at the same time. Values for each time series should be included in a separate column in the data table. All data columns should share the same timestamps.

### Option 2: SQLite Database

SQLite provides an alternative to CSV files for sharing time series data in HydroShare. SQLite is a serverless, file-based, relational database that is free, open, cross platform, and has several great tools for working with data stored in SQLite format. SQLite provides the ability to create relational tables and store multiple time series datasets within a single file that can be queried to “slice and dice” the data using Structured Query Language (SQL).

HydroShare includes a specific Time Series Content Type that implements time series data using the ODM2 data model implemented in a SQLite file (see HydroShare documentation at https://help.hydroshare.org/hydroshare-resources/content-types/time-series/). Formatting your data using HydroShare’s SQLite content type provides the following advantages:

Can store multiple time series in a single file
All metadata specified by the ODM2 data model can be included in the database file and can be viewed on the resource landing page in HydroShare
Can query the SQLite file using structured query language to retrieve subsets or aggregations of data for analysis
Can use HydroShare’s Data Series Viewer app to visualize the data in the SQLite database in a web browser using HydroShare’s “Open With” functionality
Nice tools exist for working with SQLite files in both Python and R

[Example 3 - ODM2 SQLite file](examples/Example3_ODM2_single_variable_multi_site.sqlite) - An example ODM2 SQLite file is provided here. This file contains time series data for water temperature for multiple data collection sites within the Little Bear River in Utah, USA.

## Organizing Data for Sharing

Organizing time series data for sharing requires several considerations that can be boiled down to questions about how to “chunk” the data into a set of resources in a repository and a set of files within those resources that are shared within prospective data users. Some of the important considerations include:

* **How do you want the data to be discovered and accessed?** It may be convenient for you to chunk time series data by data collection site. In this case, you can create a HydroShare resource for all of the time series data for a particular site. This makes it easy for potential data users to discover and access all of the data for a particular data collection site in one place.
* **How do you want the data to be cited?** You should think of your data as research products that can be cited. Each resource in HydroShare has a separate citation and can be published with a digital object identifier (DOI). You may choose to organize data into a set of HydroShare resources based on how you want them to be cited as products.
* **How will the data be used?** If you know investigators will want to use the data in a particular way, you may want to organize the data into a set of files that will make that easier – e.g., assembling a time series into a single file that is easy to read/work with rather than splitting data into multiple files that then have to be stitched back together.
* **What is practical for managing the data?** If you are dynamically updating data files in HydroShare as new sensor data become available, it may be practical for you to chunk data by year (i.e., one file per year) so that you only have to edit/update the most recent year’s data file when new data become available.

## Additional Best Practices for Time Series Data

The following recommendations are not meant to represent an exhaustive list but will provide relevant guidance. If you have specific questions about your time series data, please feel free to contact us.

* **Vocabularies for describing time series data**: Above we provided a reference to the ODM2 data model. The ODM2 Data Model Development Team created a set of Controlled Vocabularies with terms that can be used for several of the metadata elements within the data model for describing time series data. Those terms are curated at [http://vocabulary.odm2.org](http://vocabulary.odm2.org).
* **Use descriptive file names**: Regardless of whether you decide to use CSV files or SQLite, use descriptive names for your data files. These should be brief, but descriptive of the contents of the file.
* **Use standardized quality control levels**: The ODM data models linked above suggest a set of standardized quality control levels that can be used to describe data. These are listed in the following table.

| Level | Definition | Explanation |
| ----- | ---------- | ----------- |
| 0 | Raw data | Raw and unprocessed data and data products that have not undergone quality control. Depending on the variable, data type, and data transmission system, raw data may be available within seconds or minutes after the measurements have been made. Examples include real time precipitation, streamflow, and water quality measurements. |
| 1 | Quality controlled data | Quality controlled data that have passed quality assurance procedures such as routine estimation of timing and sensor calibration or visual inspection and removal of obvious errors. An example is USGS published streamflow records following parsing through USGS quality control procedures. |
| 2 | Derived products | Derived products that require scientific and technical interpretation and may include multiple-sensor data. An example is basin average precipitation derived from rain gages using an interpolation procedure. |
| 3 | Interpreted products | Interpreted products that require researcher driven analysis and interpretation, model-based interpretation using other data and/or strong prior assumptions. An example is basin average precipitation derived from the combination of rain gages and radar return data. |
| 4 | Knowledge products | Knowledge products that require researcher driven scientific interpretation and multidisciplinary data integration and include model-based interpretation using other data and/or strong prior assumptions. An example is percentages of old or new water in a hydrograph inferred from an isotope analysis. |

 
