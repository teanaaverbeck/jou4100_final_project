**December 21st 2023**<br>
**CMN 4100 - Digital Journalism 2**<br>
**Téana Averbeck**<br>
**Presented to Professor Jean-Sébastien Marier,BA,MJ**<br>

# Take-Home Exam: Data-Driven Multimedia Story

## 1. Introduction

Access to information and privacy (ATIP) is an act under the government of Canada which gives any Canadian citizen, permanent resident or any person or corporation residing in Canada the right to access records belonging to any government institution which also includes personal information held by these government institutions (Government of Canada, 2023). Examples of records that may be requested include but are not limited to: Briefing notes, memos, reports, Correspondences (including emails), Financial reports, etc. All summaries of record requests are publicly available information and available as a Government of Canada dataset. As this dataset is rather large in size, I decided to focus only on all ATIP requests for Crown Corporations in 2023. Crown Corporations are essentially government organizations that, while representing governmental interests, have a large measure of autonomy that allows them to function as a commercial entity. This model allows the organization to function as a hybrid of both the private and public sector. The main focus of my research was to determine which Crown Corporations had the most ATIP requests, and for those requests how many records were all disclosed, disclosed in part, all excluded, all exempt and no records exist (Government of Canada, 2023). Furthermore, I wanted to use this discovered data to analyze any potential trends and examine if there was any reasoning behind a certain percentage.

## 2. Data Cleaning

In order for the data to be transparent, it is important to highlight the methodology used to clean the dataset. The original dataset I had exported from the Government of Canada into Google Sheets contained all ATIP request summaries from 2011-2023 inclusively. As this dataset was enormous, I decided to narrow down my search and only focus on the 2023 requests thus far, thus I created filters to identify all years prior to 2023 then deleted them all. To make all of the information clearer I subsequently:

`1.` Froze the top columns;
`2.` Used a filter to organize the months in order (‘Sort A-Z’);
`3.` Removed all the french using `=SPLIT(M2,"|")` then dragging the formula for the rest of the columns to ensure all the columns are split equally and are all uniform;
`4.` Copy pasted both new columns that were a result of the Split function, then deleted the french and the original column; 
`5.` Deleted all french language by deleting the columns summary_fr and comments_fr;
`6.` Hid the summary_en column as it provided immense unnecessary detail;
`7.` Remove all agencies that are not Crown Corporations according to the Treasury Board.

After completing all these steps, my dataset resembled this:
![](sheets.png)<br>
*Figure 1: Sheets Dataset after data cleaning*

Using this new dataset, I created a pivot table with each crown corporation in the y axis, each type of record disclosure (all disclosed, disclosed in part, all excluded, all exempt and no records exist) in the x-axis and all the request summaries as the values in the middle of the table. I then used this pivot table to create a multiple pie chart of all the Crown Corporations in order to illustrate the different types of record disclosure proper to each Crown Corporation in addition to demonstrating which had more/less ATIP requests in 2023.

![](ATIP%20requests%20for%20crown%20corps%20divided%20by%20dispositions%202023.png) 
*Figure 2: ATIP requests for all Crown Corporations divided by dispositions in 2023 [Interactive version here](https://datawrapper.dwcdn.net/JgLF2/3/)*

## 3. Understanding Data

### 3.1. Cleaning Data

Use three hashtag symbols (`###`) to create a level 3 heading like this one. Please follow this template when it comes to level 1 and level 2 headings. However, you can use level 3 headings as you see fit.

Insert text here.

Support your claims by citing relevant sources. Please follow [APA guidelines for in-text citations](https://apastyle.apa.org/style-grammar-guidelines/citations).

**For example:**

As Cairo (2016) argues, a data visualization should be truthful...

### 3.2. Exploratory Data Analysis

Insert text here.

## 4. Delivering Data

Insert text here.

**This section should include a screen capture of your chart and its public link, like so:**

![](map-screen-capture.png)<br>
*Figure 2: The map created with Datawrapper*
[Interactive version here](https://datawrapper.dwcdn.net/o7Wwp/2/)

## 5. Conclusion

Thank you for reading my report.

## 6. References

Include a list of your references here. Please follow [APA guidelines for references](https://apastyle.apa.org/style-grammar-guidelines/references). Hanging paragraphs aren't required though.

**Here's an example:**

Bounegru, L., & Gray, J. (Eds.). (2021). *The Data Journalism Handbook 2: Towards A Critical Data Practice*. Amsterdam University Press. [https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153](https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153)
