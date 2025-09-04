# README for MOVES-Matrix 4.0 for High-Performance On-road Energy Use and Emission Rate Modeling Applications  
University Transportation Centers Program (UTC), U.S. Department of Transportation (USDOT)  
2025-08-13  

## Links to Dataset  
Dataset Archive Link: <https://doi.org/10.5281/zenodo.15497651>  
GitHub Archive Link: <https://github.com/gti-gatech/moves_training>

## Summary of Dataset  
This study introduces MOVES-Matrix 4.0, an innovative high-performance implementation of MOVES 4.0.1 that generates exactly same energy and emission rate results as EPA’s latest version of MOVES 4.0.1, but allows users to deploy MOVES model in complex and dynamic analyses.  The team utilized the same conceptual design used in MOVES-Matrix 2014 and MOVES-Matrix 3.0, and updated the configurations on PACE supercomputing clusters to account for the programming changes with respect to MOVES databases (e.g., migration to MariaDB) and MOVES’ algorithm updates since MOVES2014b (e.g., extended VSP/STP parameters).  The team adapted MOVES4 for cross-platform use on PACE (RHEL 7.0) without requiring root access by manually configuring MOVES4 and its dependencies in a user-space, self-contained setup.  The MOVES-Matrix 4.0 system develops sub-matrices of energy and emission rates by executing 181,818 MOVES runs to generate more than 5.8 trillion energy and emission rates in the populated matrix for a single modeling region (represented by a unique combination of fuel specification regime and inspection and maintenance program).  A total of 120 modeling areas are needed in MOVES4 to represent every county in the United States.  Performance tests demonstrate that MOVES-Matrix 4.0 produces results that are exactly the same as MOVES4 (insignificant internal rounding errors that are less than 0.0005%).  In modeling applications, generating emission rates from MOVES-Matrix is 200 times faster than running a MOVES instance.  MOVES-Matrix 4.0 is ready to be used for large-scale, dynamic transportation network analyses and emissions modeling, given its open-source nature, and its compatibility with various scripting languages.  

## Table of Contents  
A. [General Information](#a-general-information)  
B. [Sharing/Access & Policies Information](#b-sharingaccess-and-policies-information)  
C. [Data and Related Files Overview](#c-data-and-related-files-overview)  
D. [Methodological Information](#d-methodological-information)  
E. [Update Log](#e-update-log)

**Title of Dataset:**  MOVES-Matrix 4.0 for High-Performance On-road Energy Use and Emission Rate Modeling Applications  

**Description of the Dataset:** This study introduces MOVES-Matrix 4.0, an innovative high-performance implementation of MOVES 4.0.1 that generates exactly same energy and emission rate results as EPA’s latest version of MOVES 4.0.1, but allows users to deploy MOVES model in complex and dynamic analyses.  The team utilized the same conceptual design used in MOVES-Matrix 2014 and MOVES-Matrix 3.0, and updated the configurations on PACE supercomputing clusters to account for the programming changes with respect to MOVES databases (e.g., migration to MariaDB) and MOVES’ algorithm updates since MOVES2014b (e.g., extended VSP/STP parameters).  The team adapted MOVES4 for cross-platform use on PACE (RHEL 7.0) without requiring root access by manually configuring MOVES4 and its dependencies in a user-space, self-contained setup.  The MOVES-Matrix 4.0 system develops sub-matrices of energy and emission rates by executing 181,818 MOVES runs to generate more than 5.8 trillion energy and emission rates in the populated matrix for a single modeling region (represented by a unique combination of fuel specification regime and inspection and maintenance program).  A total of 120 modeling areas are needed in MOVES4 to represent every county in the United States.  Performance tests demonstrate that MOVES-Matrix 4.0 produces results that are exactly the same as MOVES4 (insignificant internal rounding errors that are less than 0.0005%).  In modeling applications, generating emission rates from MOVES-Matrix is 200 times faster than running a MOVES instance.  MOVES-Matrix 4.0 is ready to be used for large-scale, dynamic transportation network analyses and emissions modeling, given its open-source nature, and its compatibility with various scripting languages.  

**Dataset Archive Link:** <https://doi.org/10.5281/zenodo.15497651>  

**Authorship Information:**  

>  *Principal Data Creator or Data Manager Contact Information*  
>  Name: Lu, Hongyu ([https://orcid.org/0000-0002-0170-7169`](`https://orcid.org/0000-0002-0170-7169`))   
>  Institution: Georgia Institute of Technology [(ROR ID: https://ror.org/01zkghx44)](https://ror.org/01zkghx44)  
>  Address: 225 North Ave NW, Atlanta, GA 30332  
>  Email: [lhy@gatech.edu](mailto:lhy@gatech.edu)  

>  *Organizational Contact Information*  
>  Institution: The National Center for Sustainable Transportation (NCST) [(ROR ID: https://ror.org/05ac9kx40)](https://ror.org/05ac9kx40) 
>  Address: 1 Shield Surge Ste 112, Davis, CA 95616  
>  Email: [ncst@ucdavis.edu](mailto:ncst@ucdavis.edu)  
  

**Geographic location of data collection:** United States [(GeoNames URI: http://sws.geonames.org/6252001/)](http://sws.geonames.org/6252001/)  

**Information about funding sources that supported the collection of the data:** This project was funded through the US Department of Transportation and produced by the National Center for Sustainable Transportation, a National University Transportation Center. The contract numbers are: 69A3552348319, 69A3552344814.  

## B. Sharing/Access and Policies Information  

**Recommended citation for the data:**  

>  Lu, Hongyu (2025). MOVES-Matrix 4.0 for High-Performance On-road Energy Use and Emission Rate Modeling Applications [Data set]. Zenodo. https://doi.org/10.5281/zenodo.15497651 

**Licenses/restrictions placed on the data:** This document is disseminated under the sponsorship of the U.S. Department of Transportation in the interest of information exchange. The United States Government assumes no liability for the contents thereof. This content is released under the Creative Commons BY 4.0 International Attribution License <https://creativecommons.org/licenses/by/4.0/>. Use of this dataset my include attribution to the original authors. 

**Was data derived from another source?:** No  

This document was created to meet the requirements enumerated in the U.S. Department of Transportation's [Plan to Increase Public Access to the Results of Federally-Funded Scientific Research Version 1.1](https://doi.org/10.21949/1520559) and [Guidelines suggested by the DOT Public Access website](https://doi.org/10.21949/1503647), in effect and current as of December 03, 2020.  

 
## C. Data and Related Files Overview  

File List for the `Insert Full Dataset ZIP File Name Here: Ex: 12348_DATASET`  

>  1. Filename: moves master slide deck 030520.pdf    
>  Short Description:  This presentation provides a comprehensive overview of the U.S. EPA’s Motor Vehicle Emission Simulator (MOVES) framework, including its development, applications, and methodological foundation.  The deck introduces the key processes modeled within MOVES (such as running exhaust, evaporative emissions, start emissions, and brake/tire wear) and explains how emissions are calculated as a function of vehicle-specific power, operating modes, and environmental conditions.  A substantial portion of the slides illustrate fleet composition, driving cycles, and operating mode bins, complemented by three-dimensional visualizations of fuel use and pollutant emissions across vehicle classes and model years.   The material is designed for both technical audiences and policy stakeholders, highlighting MOVES’ role in federal regulatory analyses, state implementation plans, and transportation conformity assessments.  It also emphasizes the model’s adaptability to second-by-second vehicle activity data (how activity distributions can be translated into emissions estimates at scales ranging from regional inventories to microscale environmental impact studies).  The deck serves as a foundational teaching and reference tool for understanding the scientific and regulatory context in which MOVES-Matrix was conceived.

>  2. Filename: moves-matrix master slide deck 092021.pdf  
>  Short Description:  This slide deck presents the development, methodology, and applications of MOVES-Matrix in integrated transportation and environmental modeling contexts.  It details how MOVES-Matrix leverages distributed computing resources (such as Georgia Tech’s PACE cluster and Oak Ridge National Laboratory’s Titan supercomputer) to pre-run the U.S. EPA’s MOVES model across a full range of input variables.  The resulting high-dimensional matrices provide emission rates by vehicle type, model year, meteorological condition, fuel program, and inspection/maintenance regime, enabling fleet-level emission estimates at scales ranging from individual road links to regional networks.  The presentation emphasizes MOVES-Matrix’s computational efficiency, with results equivalent to MOVES (with differences below 0.0001%), while reducing runtime by more than 200-fold.  Case studies demonstrate its adaptability, including applications with travel demand models (e.g., Atlanta’s ABM15), microsimulation platforms such as Vissim™, and dispersion modeling with AERMOD. The deck also illustrates use cases at regional, corridor, and project levels, including analyses of high-occupancy toll lane conversions and corridor-specific air quality assessments.  Beyond transportation conformity and regulatory planning, the slides highlight emerging applications in big data analytics, mobile app development, and deep learning integration, positioning MOVES-Matrix as a versatile, high-performance tool for dynamic energy and emissions modeling.

>  3. Filename: moves matrix quick start guide 092021a.pdf  
>  Short Description:  This quick start guide provides step-by-step instructions for implementing the MOVES-Matrix running module in project- and network-level analyses.  It explains how to configure Python, prepare input datasets (including link characteristics, fleet source type and age distributions, meteorological conditions, and operating mode inputs), and execute batch mode tasks using the provided Python scripts and database files. The guide emphasizes practical workflows for linking MOVES-Matrix with transportation modeling applications.  It details how to generate emissions inventories and rate tables at high resolution, validate input selections, and interpret output CSV files for both aggregated link-level and disaggregated source-type results.  Examples demonstrate integration with large-scale simulation models and corridor analyses, which highlights the system’s ability to deliver rapid, accurate, and reproducible results equivalent to MOVES while dramatically reducing runtime.

>  4. Filename: moves_matrix_py27_060418.py  
>  Short Description:  This Python script is the execution engine for running MOVES-Matrix in batch mode (which is written to run in both Python 2.7 and Python 3 environments).  It automates the process of reading user-specified tasks from batchmode.csv, locating and importing the appropriate MOVES-Matrix sub-datasets, processing input files (including link definitions, fleet distributions, meteorology, and activity data), and generating emissions inventories and rate outputs in CSV format.  By scripting MOVES-Matrix operations, the file allows users to reproduce MOVES results at a fraction of the runtime while supporting large-scale or repeated analyses.  Users are only required to edit the working directory and database directory paths in the script, located on row 14 (path) and row 16 (matrixdatapath).  All other functions are pre-configured to handle the execution flow automatically, including calculating operating mode distributions, merging age and fleet structure data, and exporting final results.  Detailed instructions for preparing the required input and batch configuration files are provided in the MOVES-Matrix Quick Start Guide.

>  5. Filename: batchmode.csv*  
>  Short Description:  The 'batchmode.csv file' is the control file that organizes and manages MOVES-Matrix modeling tasks.  Each row specifies a unique task (including the geographic region, calendar year, meteorological inputs, source type distributions, age distributions, and link-level data needed for project- or network-scale analyses).  It also designates the method for defining vehicle activity—either through driving schedules, operating mode distributions, or average speeds tied to road types.  This structure enables users to queue and execute multiple tasks efficiently in batch mode, facilitating large-scale or repeated modeling runs.  Configuration of this file is critical for ensuring proper execution of MOVES-Matrix workflows.  The Quick Start Guide (slides 17–19) provides detailed instructions on how to populate each field, including the correct use of task IDs, file references, and activity mode indicators (“d” for drive schedules, “o” for opmode distributions, “v” for MOVES default cycles).  By centralizing task definitions in a single CSV, the file allows automated execution via the MOVES-Matrix Python script.

## D. Methodological Information   

**Description of methods used for collection/generation of data:** 
Test runs verified MOVES-Matrix’s computational and analytical equivalence to standard MOVES 4.0.1 runs. Using various fleet and environmental conditions, the team demonstrated that emission rates derived from the matrix were consistent within 0.0005% of those generated directly by MOVES (i.e., the only differences are rounding errors). The performance tests revealed a greater than 200 times speed increase across modeling scenarios, and these speed advantages unlock the feasibility for performing network-wide regional analyses and temporally resolved emissions analysis (e.g., for every hour of an entire year) that are intractable using the traditional MOVES user interface with conventional batch runs.  

**Instrument or software-specific information needed to interpret the data:** 
The .csv, Comma Separated Value, file is a simple format that is designed for a database table and supported by many applications. The .csv file is often used for moving tabular data between two different computer programs, due to its open format. The most common software used to open .csv files are Microsoft Excel and RecordEditor, (for more information on .csv files and software, please visit https://www.file-extensions.org/csv-file-extension). The Portable Document Format (PDF) file format was developed by Adobe Systems and represents two-dimensional documents in a device-independent and resolution-independent format. There are PDF readers available on many platforms, such as Xpdf, Foxit, and Adobe's own Adobe Acrobat Reader. PDF readers/viewers or online services for basic functions are generally free (for more information on .pdf files and software, please visit https://www.file-extensions.org/pdf-file-extension). The .py file extension is commonly used for files containing source code written in Python programming language. Python is a dynamic object-oriented programming language that can be used for many kinds of software development (for more information on .py files and software, please visit https://www.file-extensions.org/py-file-extension). The .docx file is a Microsoft Word file, which can be opened with Word and other free word processor programs, such as Kingsoft Writer, OpenOffice Writer, Apache OpenOffice, and ONLYOFFICE.     

## E. Update Log  

This README.md file was originally created on 2025-08-13 by Peyton Tvrdy ([0000-0002-9720-4725](https://orcid.org/0000-0002-9720-4725)), Data Management and Data Curation Fellow, National Transportation Library <peyton.tvrdy.ctr@dot.gov> 
 
2025-08-13: Original file created  
