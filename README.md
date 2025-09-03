# Mini-Project 3

# Overview

In this project, you will profile a ....

# Learning Goals

- 

# Detailed Instructions

## Get to know the Data Sources

1. Read about the Civil Rights Data Collection program [here](https://civilrightsdata.ed.gov/about/crdc).

2. See a list of definitions that apply to this data  [here](https://civilrightsdata.ed.gov/assets/downloads/2021-2220List20Definitions.pdf).

3. Download the data documentation for this dataset [here](https://civilrightsdata.ed.gov/assets/downloads/2021-22%20Appendix%20Workbook.xlsx). The data dictionary in Tab B. Note that there are several data files for this dataset. This data dictionary includes definitions for all files *including restricted files that we do not have access to.* You can check the Availability column to see if you have access to the data via the public use files. 


## Set up your environment

1. In RStudio, `File` > `New Project` > `Version Control` > `Git` and then copy the URL to this repo. Open `school_analysis.qmd` and add your group member's names to the header (lines 5, 7, and 9). 
2. Navigate to the [CRDC Files](https://civilrightsdata.ed.gov/assets/ocr/docs/2020-21-crdc-data.zip), and download the 2021-2022 files. Unzip the folder and then move it into your project directory. **Note that only one student in your group needs to do this.** The dataset can be pushed to other members of your group.
3. Review and select metric. 
4. In `school_analysis.qmd`, read the CSV file you just downloaded into a data frame. 
5. **If you have not already**, install the Tidy Census package in `R` using:

* `install.packages("devtools")`
* `install.packages("remotes")`
* `remotes::install_github("walkerke/tidycensus")`.

6. **If you have not already**, create an API Key for accessing census data [here](https://api.census.gov/data/create_success.html). The key will be emailed to you, and you must activate it with the link you receive in your email. **NOTE: It may take several minutes to activate. If you click on the link in your email, and it doesn't work, try again in a bit.** After activating your census key, enter the following into your console, replacing `KEY_HERE` with your census key. 

```
census_api_key("KEY_HERE", 
               overwrite = FALSE, 
               install = TRUE)
```


## Write report

1. In 400-500 words, you should write up your findings:
  * Paragraph 1: Introduce the fenceline community
  * Paragraph 2: Report on findings from your analysis.
  * Paragraph 3: Summarize the key takeaway from your analysis and describe at least one ethical concern we should consider when analyzing this data. As a reminder of our ethics framework for this course:
    * What assumptions and commitments informed the design of these datasets?
    * Who has had a say in data collection and analysis regarding these datasets? Who has been excluded?
    * What are the benefits and harms of these datasets, and how are they distributed amongst diverse social groups?


2. When you are done, you should save the .qmd file, Render the file, commit changes, and then push changes back to GitHub. That's it for submission. You don't need to submit anything on Moodle. 

# Evaluation 

You will be evaluated on the extent to which your mini-project demonstrates fluency in the following course learning dimensions:

- Pivoting Data
  - Have you successfully reshaped a data frame longer?
- Joining Data
  - Have you successfully joined two tables for further analysis?
- Writing Functions
  - Have you successfully interpreted helper functions?
  - Have you successfully created functions?
- Point Mapping
  - Have you produced maps that plot points by latitude and longitude?
  - Have you demonstrated effective binning when coloring points?
- Polygon Mapping
  - Have you produced maps that plot polygons?
  - Have you demonstrated effective binning when coloring polygons?



