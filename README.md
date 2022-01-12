# NYPD-Arrests-Data-Warehouse-Pentaho-DI-Oracle-21C-Tableau
Pentaho DI tools for ETL that pushes data to an Oracle 21C database eventually read by a live Tableau connection for data visualization &amp; analysis.


## Background

With nearly 36,000 officers and 19,000 civilian employees, the New York City Police Force (NYPD) is the largest and oldest municipal police department in the United States. The New York Police Department (NYPD) was founded in 1845 and is currently in charge of policing an 8.5-million-person city by providing public safety, law enforcement, traffic management, counterterrorism, and emergency response services. The NYPD’s principal objective is to enhance the quality of life by enforcing the law, maintaining peace, safeguarding the public, removing fear, and maintaining order. With such a large city and many different demographics to protect, some arrests are justifiable, and others are considered false arrests – being held without probable cause.
In an attempt to increase transparency and awareness, a datawarehouse is designed and analyzed in this project to analyze the NYPD's historical arrest data with a primary focus on building an effective data pipeline and then using it to identify any underlying NYPD arrest trends based on various attributes.

## Source Data

Data for this project has been retrieved from NYC OpenData, free public data published by New York City agencies and other partners. From 2006 to the end of the previous calendar year, every arrest in New York City is chronicled. Each arrest documented contains information such as demographics of the suspect, kind of offense, location, and time of enforcement. Every quarter, this information is manually retrieved and evaluated by the NYPD's management Analysis and planning office before being disseminated on the internet

## Key Performance Indicators

In order to breakdown the data provided by NYC Open Data and provide valuable insights, the data warehouse uses the following KPIs:

• Number of arrests by borough and location
• Number of arrests by date (overall, pre and post COVID)
• Number of arrests by offense and NYS Penal law type
• Number of arrests by perpetrators demographic
  o Age group
  o Gender
  o Race
• Number of arrests by precinct and jurisdiction
• Number of arrests by Average Income Household (by precinct Zip Code)

## Project Tools

### Data Integration/ETL Tool Selection

Extract, Transform & Load (ETL) tool Pentaho by Hitachi Vantara is used to to utilize data integration, ETL, and database mapping functionalities - all in one platform.

### Database Selection

Oracle 21c Database is used as the cloud data storage (warehouse) in this project. The database will act as the cloud storage that receives data pipelines through Pentaho and then be used as a data lookup for analysis calls by data visualization software Tableau.

### Analysis Tool Selection

Tableau visualization software is used to visualize and analyze the datasets. Tableau directly connects to the Oracle 21C database and provides fast access to the data for descriptive visualizations. These visualizations are used to explore and explain the underlying trends and insights within the arrests data.

### Results

The results of this warehouse, in the form of Tableau visualizations, can be found under the Assets folder while the ETL transformations and example input files are available under the corresponding folders.

-- Aarif M Jahan -- Dec 13, 2021
