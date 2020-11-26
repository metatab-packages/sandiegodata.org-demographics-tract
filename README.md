# San Diego Demographics


The dataset includes three files all from the Census, detailing age and sex and race ethnicity. All of the files are built from Census data; see the References section for the specific dates and releases. 

## Age and Sex

The ``age_sex`` data comes from B01001 and the associated race iterations. The file combines all of the race iteration tables and adds columns for sex, race/ethnicity codes and age groups. 

THe race ethnicity codes are: 

*  white 
*  nhwhite
*  black
*  aian
*  asian
*  nhopi
*  other
*  many
*  hisp

For each of the race/ethnicity values except nhwhite and hisp, the category sums the associated 'nh_*' and 'hisp_*' categories from the raceeth table. 


## Race And Ethnicity

The  ``raceeth`` is based on the census table [C03002: Hispanic or Latino Origin by Race](https://censusreporter.org/tables/C03002/), but recormats the structure, use a code for race/ethnicity in the `raceeth` column to indicate the oricinal clumn name in the Census dataset. These codes are: 

* total: B03002_001  Total
* nonhisp: B03002_002 Not Hispanic or Latino
* nh_white: B03002_003 Not Hispanic or Latino  - White alone
* nh_black: B03002_004 Not Hispanic or Latino  - Black or African American alone
* nh_aian: B03002_005 Not Hispanic or Latino  - American Indian and Alaska Native alone
* nh_asian: B03002_006 Not Hispanic or Latino  - Asian alone
* nh_nhopi: B03002_007 Not Hispanic or Latino  - Native Hawaiian and Other Pacific Islander alone
* nh_other: B03002_008 Not Hispanic or Latino  - Some other race alone
* nh_multiple: B03002_009 Not Hispanic or Latino  - Two or more races
* nh_multiple_other: B03002_010 Not Hispanic or Latino  - Two or more races  - Two races including Some other race
* nh_multiple_more: B03002_011 Not Hispanic or Latino  - Two or more races  - Two races excluding Some other race and three or more races
* hisp: B03002_012 Hispanic or Latino
* hisp_white: B03002_013 Hispanic or Latino  - White alone
* hisp_black: B03002_014 Hispanic or Latino  - Black or African American alone
* hisp_aian: B03002_015 Hispanic or Latino  - American Indian and Alaska Native alone
* hisp_asian: B03002_016 Hispanic or Latino  - Asian alone
* hisp_nhopi: B03002_017 Hispanic or Latino  - Native Hawaiian and Other Pacific Islander alone
* hisp_other: B03002_018 Hispanic or Latino  - Some other race alone
* hisp_multiple: B03002_019 Hispanic or Latino  - Two or more races
* hisp_multiple_other: B03002_020 Hispanic or Latino  - Two or more races  - Two races including Some other race
* hisp_multiple_more: B03002_021 Hispanic or Latino  - Two or more races  - Two races excluding Some other race and three or more races

For the most part you will use the ``nh_*`` for all races, ``hisp_white`` for hispanics, and ``nh_white`` for whites. 

