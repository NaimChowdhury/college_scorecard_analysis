# college_scorecard_analysis

In this project, Sumitra Sankarasubramanian, Jamie Hobbs, and Naeem will perform exploratory data analysis and data munging to answer curious questions about college students, debt, and financial outcomes.

## Questions

- How long does it take the average student to pay off their debt?

- How has the relationship between tuition and debt changed over time? (First answer for a single year, then answer over multiple years.) 

- Ethnicity over time by region

## 10/08/2019

Initial change.

### Current Goals

- Make a large merged CSV which contains the data spanning several years.

- Write 9-15 questions for us to answer in our analysis.

- Come up with 2 good quality measurements

- using the PCIP variables, how has the percentage of people seeking $X$ degree changed over time?

- how has the proportion of full time faculty at an instutition changed over time?

### Variables of Interest

- HCM2 (int) - schools that are on "heigtened cash monitoring 2", flagged with a 1

- PREDDEG (int) - predominant undergrad degree awarded, 0 1 2 3 4

    - 0 not class

    - 1 certificate degree

    - 2 associates degree 

    - 3 bachelor's degree

    - 4 graduate degree

- HIGHDEG (int) - highest degree awarded 0 1 2 3 4 (same as above)

- REGION (int) - regiod id

        1	New England (CT, ME, MA, NH, RI, VT)
        2	Mid East (DE, DC, MD, NJ, NY, PA)
        3	Great Lakes (IL, IN, MI, OH, WI)
        4	Plains (IA, KS, MN, MO, NE, ND, SD)
        5	Southeast (AL, AR, FL, GA, KY, LA, MS, NC, SC, TN, VA, WV)
        6	Southwest (AZ, NM, OK, TX)
        7	Rocky Mountains (CO, ID, MT, UT, WY)
        8	Far West (AK, CA, HI, NV, OR, WA)
        9	Outlying Areas (AS, FM, GU, MH, MP, PR, PW, VI)

- LOCALE 

        11	City: Large (population of 250,000 or more)
        12	City: Midsize (population of at least 100,000 but less than 250,000)
        13	City: Small (population less than 100,000)
        21	Suburb: Large (outside principal city, in urbanized area with population of 250,000 or more)
        22	Suburb: Midsize (outside principal city, in urbanized area with population of at least 100,000 but less than 250,000)
        23	Suburb: Small (outside principal city, in urbanized area with population less than 100,000)
        31	Town: Fringe (in urban cluster up to 10 miles from an urbanized area)
        32	Town: Distant (in urban cluster more than 10 miles and up to 35 miles from an urbanized area)
        33	Town: Remote (in urban cluster more than 35 miles from an urbanized area)
        41	Rural: Fringe (rural territory up to 5 miles from an urbanized area or up to 2.5 miles from an urban cluster)
        42	Rural: Distant (rural territory more than 5 miles but up to 25 miles from an urbanized area or more than 2.5 and up to 10 miles from an urban cluster)
        43	Rural: Remote (rural territory more than 25 miles from an urbanized area and more than 10 miles from an urban cluster)

- LOCALE2

        1	Large City (a central city of a CMSA or MSA, with the city having a population greater than or equal to 250,000)
        2	Mid-Size City (a central city of a CMSA or MSA, with the city having a population less than 250,000)
        3	Urban Fringe of a Large City (any territory within a CMSA or MSA of a Large City and defined as urban by the Census Bureau)
        4	Urban Fringe of a Mid-Size City (any territory within a CMSA or MSA of a Mid-Size City and defined as urban by the Census Bureau)
        5	Large Town (an incorporated place or Census-designated place with a population greater than or equal to 25,000 and located outside a CMSA or MSA)
        6	Small Town (an incorporated place or Census-designated place with a population less than 25,000 and greater than or equal to 2,500 and located outside a CMSA or MSA)
        7	Rural, Outside MSA (any territory designated as rural by the Census Bureau that is outside a CMSA or MSA of a Large or Mid-Size City)
        8	Rural, Inside MSA (any territory designated as rural by the Census Bureau that is within a CMSA or MSA of a Large or Mid-Size City)

- LATITUDE, LONGITUDE? Could possibly do a nice map of the location of low income schools, schools that are on HCM2, or some other info. May end up using!

- CCBASIC (a classification of some kind. lots of super interesting values. where are all the faith based schools? what abotu law schools? tribal colleges?)

- HBCU, PBI, ANNHI, TRIBAL, AANAPII, HSI, NANTI, MENONLY, WOMENONLY, RELAFFIL, almost all variables are boolean, but the relaffil is broken down by religion. revisit in the data dictionary!

- ADM_RATE, ADM_RATE_ALL, admissions rate

- UG, UGDS_WHITE, UGDS_BLACK etc., the share of students who are white, black, enrollment of all students, etc

- Family income buckets variables 560-595

- Family income buckets of students who receive Title IV financial aid, variables 596-619

- TUITIONFEE_IN, TUITIONFEE_OUT, TUITIONFEE_PROG

- AVGFACSAL (average faculty salary)

-  PFTFAC (proportion of faculty that is full time)

