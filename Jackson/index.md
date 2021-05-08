# Jackson's Workspace


I'm interested in looking at the relationship between ethnicity and admitted students to Universities of California (UCs) and how admissions have changed since 2007. I chose to start at 2007 even though the data set goes back to 1994 because then we'd be starting before the 2008 recession and move through periods of large social change.





## The Relationship Between Applications, Admittance, and Enrollment


I started by looking at the students who applied to UCs first from public schools then from private schools.

{% include_relative Visualizations/AppliedStudentsPublic.html %}

{% include_relative Visualizations/AppliedStudentsPrivate.html %}

What we can see is that the major demographics from either graph are different. While in public schools we see there are majorities in both the Asian student population and the Latino student population, the private schools have a majority in the White student population.

(I should bring up that it is hard to trust the data on the American Indian students as we will see in later graphs. In general it seems incomplete.)

Anyway, since we see the which majorities apply to UCs most often from public and private schools, we should see those same majorities in the admitted students just not in the same magnitude. In private schools we do until around 2018 where the balance has been more equalized.

{% include_relative Visualizations/AdmittedStudentsPrivate.html %}

But in public schools, the majorities are mainly the Asian and White students until 2011 when White and Latino students are equalized. Then it's not until 2020 when we see Latino students come out as a majority in UCs.

{% include_relative Visualizations/AdmittedStudentsPublic.html %}

While the Applied and Admitted graphs should theoretically related to each other, a relation is harder to come up with in terms of enrollment because so many factors come into ones enrollment to college. In theory we should see similar majorities and minorities, but it's harder to use this for data to find the majorities and minorities. Once again, in private schools we can see the data slowly equalize over time at least with the three majorities.

{% include_relative Visualizations/EnrolledStudentsPrivate.html %}

But in  public schools the highest majority is Asian students through the whole through the whole time period. Now there may be a host of factor that can explain why this is, but it is difficult to use this data to explain what the factors are, so I probably will not go into it.
 
{% include_relative Visualizations/EnrolledStudentsPublic.html %}

In conclusion for this section, in general we see that UCs are trying to equalize the three majorities applying to their schools. But with this we see that some groups are underrepresented specifically the African American students and more so American Indian students. In this next section, I will look at each ethnicity separately.

## A Closer Look into Each Ethnicity Admission Rates

Before I continue, I feel I should bring up an issue I found and referenced beforehand. When looking at the American Indian UC data it is vastly incomplete. Values seem to be missing both in public and prove schools. It is in general pretty inconsistent and makes me wonder why this occurred and why specifically it occurred most when documenting American Indian students. While there is very minimal inconsistencies in other parts of the data, none are as glaring as these.

{% include_relative Visualizations/AmericanIndianStudentsPublic.html %}


{% include_relative Visualizations/AmericanIndianStudentsPublic.html %}







For my reader, if you would like to you can check my work, you can. While the UC admissions data is a pain to work with because the data comes in multiple files and is encoded in utf-16le, I have consolidated all the data I used from the UC admissions data into one data frame:

{% include_relative Visualizations/UCDataCon.html %}

Also, here is a link to download all the code I used:

[UC Admissions Python File](https://drive.google.com/file/d/1E6izir4fjy9AapawBEvNEvForzPyTJct/view?usp=sharing)

As well as a folder of all the data frames I used:

[UC Admissions Data Files](https://drive.google.com/file/d/1khTUOeadGzKHnIAH9RYK9qq-trh-6jU6/view?usp=sharing)