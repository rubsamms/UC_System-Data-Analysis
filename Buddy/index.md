## Buddy's Workspace

I am going to endeavor to use the UC system data to describe demographic differences in the UC's admission stats across the most recent decade,
with a particular interest in the effect that inclusion or removal of admission criteria traditionally considered to reproduce existing social
inequality actually has on these demographics.

For this I will use the Freshmen ethnicity by year datasets, which are CSV files containing rows representing each student admitted, including
their ethnicity as self-reported on their application and the year they were admitted.

Here is an initial visualization I made:

{% include_relative /init_fig.html %}

[History of admissions article on Frontline](https://www.pbs.org/wgbh/pages/frontline/shows/sats/etc/ucb.html)

[Policy document from the UC website](https://admission.universityofcalifornia.edu/counselors/files/quick-reference.pdf)


more detailed discussion of the questions they are interested in exploring



some of the data issues they've encountered, e.g. missing data, outliers, conversion issues, merging etc

The datasets were downloadable from the UC page as .csv files, which were oddly enough encoded in UTF-16 LE. That was hard to figure out.
Then the delimiter character was '\t', which was also a curveball. I think I've been spoiled with highly standardized data. After that,
there were more n/A values than I was used to - I wasn't sure how to prune the rows to provide the fullest profile while also
keeping the mathematical utility of the table.

some simple visualizations or stats that provide simple insights into the integrity of the data,
i.e. Convince the reader that this data is what it purports to be and identify possible problems with the data.
Often this involves looking at each column and doing univariate descriptions and visualizations like box plots, histograms etc




Above and beyond: plotly heatmap?