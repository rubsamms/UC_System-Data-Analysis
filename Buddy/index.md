## Buddy's Workspace

Here is an initial visualization I made:

{% include_relative /init_fig.html %}

[History of admissions article on Frontline](https://www.pbs.org/wgbh/pages/frontline/shows/sats/etc/ucb.html)

[Policy document from the UC website](https://admission.universityofcalifornia.edu/counselors/files/quick-reference.pdf)


Initially, I was interested in exploring the change in ethnic demographics in the UC over the course of UC admissions policy changes. However, I find far more interesting the question of Proposition 209, pased in 1995. This law discontinued the historical practice of affirmative action in the UC. According to the article linked above, this law had a "drastic" effect on the admissions profile of Berkeley in particular, when in 1998 (the year this law took effect) 56 percent fewer African Americans and 49 percent fewer Latinos were admitted. I would like to see the effect of this law at the other UC campuses, as well as on the GPA profile of all campuses.

This data was very hard to work with. It was organized in a strange way, with a column bizarrely (and to me, meaninglessly) titled "Calculation1", as well as multiple numeric and nonnumeric ways of representing dates, and a system of marking which students were admitted and which were not with a 3-letter abbreviation, as opposed to simply separating these groups into multiple datasets.

The datasets were downloadable from the UC page as .csv files, which were oddly enough encoded in UTF-16 LE. That was hard to figure out. Then the delimiter character was '\t', which was also a curveball. I think I've been spoiled with highly standardized data. After that, there were more n/A values than I was used to - I wasn't sure how to prune the rows to provide the fullest profile while also keeping the mathematical utility of the table.

My original research question (the degree of diversity shift which occurred in 1998 as a result of the ban on affirmative action) cannot be answered by the data as it is provided. In the only dataset which included time of recording, records began at the year 1998, which means I had no control group to compare to the pool of applicants admitted after the affirmative action ban. Instead, I will compare the diversity of the admitted applicants of the years 1998 (which would be perhaps the least diverse in the entire dataset, I will check this) and 2020, when the UC relaxed several application requirements incl. the SAT.


We can see from my partner Jackson's work that the overall number of white admitted students to the UC decreased between 2007 and 2020, as the overall number of admitted latino, asian, and african american students increased. However there are some strange patterns of behavior in indian (native) students, with higher admittance rates in the earlier part of the recording period.

some simple visualizations or stats that provide simple insights into the integrity of the data,
i.e. Convince the reader that this data is what it purports to be and identify possible problems with the data.
Often this involves looking at each column and doing univariate descriptions and visualizations like box plots, histograms etc

Here are a few basic visualizations of the amount of students of a certain ethnicity admitted to the University:

{% include_relative /simple2.html %}

{% include_relative /simple.html %}

{% include_relative /prettyFig.html %}

We can see from the figure below that the UC admitted students population of 1998 was not the least diverse on record. In fact, and this is striking, there seems to be no significant difference in diversity between the admitted class of 1998 and 1994. This seems to contradict the claim referenced above (PBS) that the hispanic and African American admitted student populations decreased by around 50% each in '98. However, that claim was in reference to the Berkeley campus alone; it seems unlikely but is still possible that this claim is true. Further investigation would be necessary to fully determine the veracity of this claim.

{% include_relative /normedData.html %}

We cannot conclude that the 1998 affirmative action ban did not have an effect on the admitted demographics at Berekeley, but to determine its effect would require further investigation.

However, we can tell that the UC has achieved overall parity of admissions among Hispanic, Asian and white demographics. This means Asian students are overrepresented relative to the general population, which could be due to a number of factors. However, the UC has yet to achieve representative levels of enrollment among black students. Further investigation would be necessary to determine the causes of the overrepresentationo of Asian students and to understand the policy of the UC in recruiting more black students.

[Here](https://drive.google.com/file/d/1hXziEAmwvCsGpziXKFNd0xiXvnxN-Hp3/view?usp=sharing) is a link to the Jupyter Notebook I used to create these visualizations.

To obtain these datasets, [follow this link](https://www.universityofcalifornia.edu/infocenter/admissions-source-school). Download the dataset (in crosstab format) called "HS by Year_crosstab.csv". This can be wrangled with my notebook to reproduce my results.