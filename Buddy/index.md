## Buddy's Workspace

Here is an initial visualization I made:

{% include_relative /init_fig.html %}

[History of admissions article on Frontline](https://www.pbs.org/wgbh/pages/frontline/shows/sats/etc/ucb.html)

[Policy document from the UC website](https://admission.universityofcalifornia.edu/counselors/files/quick-reference.pdf)


Initially, I was interested in exploring the change in ethnic demographics in the UC over the course of UC admissions policy changes. However, I find far more interesting the question of Proposition 209, pased in 1995. This law discontinued the historical practice of affirmative action in the UC. According to the article linked above, this law had a "drastic" effect on the admissions profile of Berkeley in particular, when in 1998 (the year this law took effect) 56 percent fewer African Americans and 49 percent fewer Latinos were admitted. I would like to see the effect of this law at the other UC campuses, as well as on the GPA profile of all campuses.

This data was very hard to work with. It was organized in a strange way, with a column bizarrely (and to me, meaninglessly) titled "Calculation1", as well as multiple numeric and nonnumeric ways of representing dates, and a system of marking which students were admitted and which were not with a 3-letter abbreviation, as opposed to simply separating these groups into multiple datasets.

The datasets were downloadable from the UC page as .csv files, which were oddly enough encoded in UTF-16 LE. That was hard to figure out. Then the delimiter character was '\t', which was also a curveball. I think I've been spoiled with highly standardized data. After that, there were more n/A values than I was used to - I wasn't sure how to prune the rows to provide the fullest profile while also keeping the mathematical utility of the table.

some simple visualizations or stats that provide simple insights into the integrity of the data,
i.e. Convince the reader that this data is what it purports to be and identify possible problems with the data.
Often this involves looking at each column and doing univariate descriptions and visualizations like box plots, histograms etc

Here are a few basic visualizations of the amount of students of a certain ethnicity admitted to the University:
{% include_relative /init_fig.html %}


Above and beyond: plotly heatmap?