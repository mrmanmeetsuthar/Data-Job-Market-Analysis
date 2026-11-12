# Data Job Market Analysis Dashboard

## Project Overview

This project analyzes a dataset of job postings to explore demand across
job roles, locations, industries, companies, salary estimates, education
categories, company ratings, and technical skills. The analysis was
prepared using **Power Query** for data cleaning and **Microsoft Power
BI** for data modeling, DAX measures, and dashboard visualization.

## Dashboard Snapshot

Add your final Power BI dashboard screenshot to this repository and
update the image path below.

``` markdown
![Data Job Market Analysis Dashboard](images/dashboard.png)
```

## Dataset Overview

The loaded dataset contains:

  Metric                      Value
  ------------------------ --------
  Job postings                  742
  Companies                     343
  Industries                     60
  Average salary measure     101.48

The dashboard displays salary using an average salary measure. The
project presentation assumes the salary figures are in USD thousands;
confirm the original dataset's currency and units before using the
figures externally.

### Main fields used

-   Job title and simplified job title
-   Salary estimate, lower salary, upper salary, and average salary
-   Company name, company rating, location, and headquarters
-   Company size, founded year, company age, industry, and sector
-   Revenue and competitors
-   Technical skill indicators such as Python, SQL, Excel, AWS, and
    Spark

## Tools and Technologies

-   Microsoft Power BI Desktop
-   Power Query Editor
-   DAX
-   CSV

## Data Preparation

The preparation steps completed during the project walkthrough included:

1.  Imported the CSV data into Power Query.
2.  Promoted the first row to column headers.
3.  Reviewed and assigned column data types.
4.  Removed one unwanted column.
5.  Replaced `-1` placeholders with `null` in selected fields, including
    `Founded` and `Age`.
6.  Loaded the transformed data into Power BI.

> **Data quality note:** Before publishing, validate missing values,
> duplicate records, salary parsing, education labels, and the meaning
> of the skill-indicator columns. The project screenshots show the data
> preview and transformations, but do not establish that every column
> has undergone a complete quality audit.

## Dashboard KPIs

The report includes four KPI cards:

-   **Total Job Openings:** 742
-   **Total Companies:** 343
-   **Total Industries:** 60
-   **Average Salary:** 101.48

## Dashboard Visualizations

The dashboard contains the following analysis views:

1.  Top 10 States by Job Opportunities
2.  Top 5 Industries by Job Demand
3.  Average Salary by Education
4.  Company Ratings Comparison
5.  Top 10 Hiring Companies
6.  Average Salary by Job Role
7.  Most Demanded Technical Skills
8.  Top 10 Most In-Demand Job Roles

## Key Findings Visible in the Dashboard

-   California has the highest displayed state count, with **152** job
    postings.
-   Massachusetts follows with **103**, and New York with **72**.
-   The largest displayed job-role category is **Data Scientist**, with
    **251** postings.
-   The next displayed job-role categories are Other Scientist (**111**)
    and Data Engineer (**77**).
-   Biotech & Pharmaceuticals is the leading displayed industry, with
    **112** postings.
-   Insurance Carriers (**63**) and Computer Hardware & Software
    (**59**) are the next displayed industries.

These findings describe the records in this dataset only. They should
not be interpreted as a complete measure of the overall job market.

## Business Recommendations

-   Explore opportunities in locations with higher posting counts, while
    also considering remote and hybrid roles.
-   Compare the requirements of Data Scientist, Data Engineer, and
    Analyst positions to identify relevant skills.
-   Investigate opportunities in industries with higher posting counts,
    including biotechnology, insurance, technology, and healthcare.
-   Compare salary ranges by role and location rather than relying only
    on a single average.
-   Validate company-rating sample sizes and skill indicators before
    making rankings or career decisions.

## Repository Structure

A suggested repository structure is:

``` text
data-job-market-analysis/
│
├── README.md
├── dashboard/
│   └── Data_Job_Market_Analysis.pbix
├── reports/
│   ├── Data_Job_Market_Analysis_Report.pdf
│   └── Data_Job_Market_Analysis_Presentation.pptx
├── images/
│   └── dashboard.png
└── data/
    └── README.md
```

Keep the original CSV files in the `data/` folder only if you have
permission to share them. If the dataset has licensing or redistribution
restrictions, upload a data dictionary or source link instead.

## Limitations

-   The dataset contains 742 postings and may not represent the entire
    job market.
-   The source and collection date should be documented if available.
-   Salary currency and units should be confirmed from the original
    dataset.
-   Missing values, duplicates, and skill-flag definitions should be
    validated.
-   Some education categories appear abbreviated in the dashboard and
    should be made readable before final publication.

## How to Use

1.  Download the `.pbix` file from this repository.
2.  Open it in Microsoft Power BI Desktop.
3.  If Power BI requests the CSV source, update the data source path to
    your local copy.
4.  Use the dashboard visuals to explore job demand, salary, industry,
    location, and skill patterns.

## Author

**Manmeet Suthar**\
Data Analyst Portfolio Project
