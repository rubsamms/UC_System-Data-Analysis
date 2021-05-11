
## Michael Rubsamen's Workspace
---

I grew up in California and am very familiar with the UC system and the type of influence it has on Californian applicants. I am interested in comparing in state to out of state student demographics and seeing if there are any trends between the two groups. Additionally, I am interested in exploring the in state acceptance rates on a per campus basis to see if there is an overwhelming majority of accepted applicants who live in the same county as the campus or if it is harder for those students to gain acceptances into their home town UC.



I would like to explore the following to see if there are trends:



1. Instate acceptance rates in 2020\
2. Compare these to previous years and investigate the relationship between test scores and the [California Resident Guarantee](https://admission.universityofcalifornia.edu/admission-requirements/freshman-requirements/california-residents/)
3. Gpa trends across UC campus admissions

I am also interested in looking at micro trends within the different California county applicants and seeing if its true that UCLA has a bias for non LA county residents and if UC Berkeley has a bias against east bay applicants. Looking at test scores and other demographics, I hope to see if there are any trends in geographic location and acceptances to different UC campuses.


I plan to use **Plotly** as a tool to create advanced visualizations of my dataset so that users can conduct an interactive exploration of the data easily and accessibly.

For example, in 2020 the proportion of admits stratified by county can be explored below. All counts under 50 were ignored :

{%  include_relative Visualizations/UC_Pie_2020.html% } 


---
I had a hard time deciding where to get my data from and making sure that all of the entries were completely filled in with the information that I wanted to extract. To test this, I decided to make a grouped bar chart to see whether the counts were accurate or not. I imagine that the number of students who enrolled had to be less than the number of students accepted and the total number of applicants. If the trend of the graph follows this prediction, I would have a better time rationalizing that my data had enough completeness to be used for future analysis. 

To see the initial trends in public school applicants and their outcomes, the following figure was made to compare side by side the university wide applicant outcomes based off of the applicant's county:

---

{%  include_relative Visualizations/UC_Public_BarOutcomes.html  %}

--- 

However, this figure is for all UC campuses and is not stratified by campus. The data does seem to be complete and accurate since in all cases the number of applicants > number of acceptances > number of enrolled students which would be the expected trend. Taking a deeper look, I found that the total number of applicants in 2020 was 99,339, total number of admits to be 70,751, and the total number of enrolled students to be 34,600. To account for possible missing data, and since we can't interpolate admissions data, all graphs were normalized so lack of data did not skew the visualization. 

I was also curious about the overall gender spread for the 2020 incoming first year class. The pie chart below confirms that the proportion of women who apply, are admitted, and enroll are about 19 percent greater than men. This was fascinating and I hope to use this demographic in the future to compare geographic location trends in college admissions.

---
{%  include_relative Visualizations/UC_GenderPie_2020.html  %}


### In State Admissions by Campus 

Looking at the proportion of admits by county, we can clearly see that southern California schools dominate the admissions market.

{%  include_relative Visualizations/UC_Public_Bar_Proportion.html  %}

A couple key takeaways:

1. San Francisco, Contra Costa, Alameda, San Joaquin, Sacramento, Riverside, and San Diego counties have the highest proportion of enrolled students comparatively to their proportion of applicants.
1. LA county has the highest application proportion out of all in state counties.
1. Northern California counties serve as a large minority

The question remains, do UC campuses preferentially accept applicants from geographically close counties or do they discriminate against their own county's applicants? Lets take a look at UC Berkeley first. UC Berkeley's admission statistics for in state public schools is given below:

{% include_relative Visualizations/UC_Berk_Bar_Proportion.html  %}

Clearly, East bay counties represent a large majority of enrolled students despite their contribution of applicants. LA is still the largest shareholder of admitted students. Interestingly enough, LA, Orange, and San Bernardino counties have a higher proportion of applicants than enrolled students. So far, I am inclined to believe that UC Berkeley does preferentially select for nearby county applicants.

Lets take a look at UCLA: 

{%include_relative Visualizations/UC_Berk_Bar_Proportion.html %}

This visualization has a much different outcome. First, we can see that LA county provides the largest proportion of enrolled students, but the results for the other SOCAL counties is pretty similar to UC Berkeley. However, It does look like the proportion of in state enrolled students is lower than compared to Berkeley.

Looking at some Other schools, we have...

Davis:
{%include_relative Visualizations/UC_Davis_Bar_Proportion.html %}

UCSB:

{% include_relative Visualizations/UC_SB_Bar_Proportion.html %}

UCSD:

{%include_relative Visualizations/UC_SD_Bar_Proportion.html %}

UC Merced:

{%include_relative Visualizations/UC_Merced_Bar_Proportion.html %}

It looks like for the more remote schools like Merced and Davis, a large majority of those enrolled students come from those counties. Furthermore, I was surprised to see the same trend for UCSD and UCSB!

When looking at the total proportion of students accepted into the UC system from out of state schools, Its clear that the majority of applications come from Texas and Washington. However, It looks like Oregon, Virginia, and New Jersey have the highest proportion of enrolled students relative to their application footprint. 

{%include_relative Visualizations/UC_OOS_Bar_Proportion.html %}

Looking at this, I decided to see the admissions GPA statistics for in state and out of state acceptances. As it turns out, they're very similar. Lets take a look...


Taking the original data and grouping by state and county, we can see average all of the GPAs for each high school per state/county and view the average GPA acceptances for each group.
In State:

{%include_relative Visualizations/UC_Public_GPA.html %}

Out of State:

{%include_relative Visualizations/ UC_OOS_GPA.html %}

International:

{%include_relative Visualizations/UC_foreign_GPA.html %}

All three groups have alarmingly similar data. Also notice how Los Angeles is a category for the out of state section, which is a mistake and obviously strange. However, if you take a closer look at the in state GPAs, it can be found that LA has the lowest average gpa Very interesting....

Looking even deeper at the bar graphs, we can see just how similar the spreads are between the groups:

In State:

{%include_relative Visualizations/UC_cabox_GPA.html %}


Out of State:

{%include_relative Visualizations/UC_OOSbox_GPA.html %}

International:

{%include_relative Visualizations/UC_foreignbox_GPA.html %}



