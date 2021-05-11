## Michael Rubsamen's Workspace

---

I grew up in California and am very familiar with the UC system and the type of influence it has on Californian applicants. I am interested in comparing in state to out of state student demographics and seeing if there are any trends between the two groups. Additionally, I am interested in exploring the in state acceptance rates on a per campus basis to see if there is an overwhelming majority of accepted applicants who live in the same county as the campus or if it is harder for those students to gain acceptances into their home town UC.



I would like to explore the following to see if there are trends:



1. Instate acceptance rates in 2020
2. Compare these to previous years and investigate the relationship between test scores and the [California Resident Guarantee](https://admission.universityofcalifornia.edu/admission-requirements/freshman-requirements/california-residents/)
3. Gpa trends across UC campus admissions

I am also interested in looking at micro trends within the different California county applicants and seeing if its true that UCLA has a bias for non LA county residents and if UC Berkeley has a bias against east bay applicants. Looking at test scores and other demographics, I hope to see if there are any trends in geographic location and acceptances to different UC campuses.


I plan to use **Plotly** as a tool to create advanced visualizations of my dataset so that users can conduct an interactive exploration of the data easily and accessibly.

For example, in 2020 the proportion of admits stratified by county can be explored below. All counts under 50 were ignored:

{%  include_relative Visualizations/UC_Pie_2020.html % } 


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