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


{% include_relative Visualizations/AmericanIndianStudentsPrivate.html %}


In terms of the African American student population, while there is an inconsistency in 2007, and for the rest of the data, it seems pretty complete. Anyway, for the other ethnicities we see general trends. For this, I think looking at the public data gives a little bit more insight to how ethnicity plays into admittance. To start I'd like to look at the African American student numbers.


{% include_relative Visualizations/AfricanAmericanStudentsPublic.html %}

To start off, we should talk about the admission rate as a percentage so we can get an accurate representation of these graphs in context with each other. So in 2007 the admittance rate of African American students from public schools was 17.3 percent in 2020 it decreased to 7 percent and more importantly the number of admitted students did not change by much (-20 students difference). So what we see is that the number of African American students applying to UCs has increased by more than double but UCs have not increased their admittance rate to compensate. But in order to see how problematic this is, we must look at the other data as well.

{% include_relative Visualizations/AsianStudentsPublic.html %}

In 2007, the admittance rate for Asian students was 91.7 percent and in 2020 it decreased to 80.5 percent. However compared to the African American students change of -20 students admitted, the Asian student change was of 5049 students. So the UCs admitted 5049 more students than in 2007. I find this problematic, why were no more African American students admitted into the UC program. While this graph alone is pretty good in the fact that since more students had applied more were admitted, when its in context with the African American students I see it as being more problematic as we should see more African Americans being admitted.

{% include_relative Visualizations/HispanicLatinoStudentsPublic.html %}

As we move on, I'd like to say once again that this is not a bad trend when you look at it alone. As more Latino and Hispanic Students applied to UCs more were admitted. In 2007 we see 83.3 percent admittance rate and in 2020 a 65.8 percent admittance rate with a difference of 15000 students admitted. But I feel that once again we should've seen an uptick in African American admittance as the years went on.

{% include_relative Visualizations/WhiteStudentsPublic.html %}

Anyway, the final visualization I have is what I would call not a great trend. In 2007 white student admittance was 91.8 percent and in 2020 was 71.4 percent with a student difference -5100 students, but while the other graphs had an general increase in applicants, this graph see no general change in applicants. I would like to be clear that I do not think this graph is as damning as the African American students because while there is a larger decrease in students with the white students, at least there are around 40 times the amount of students as African American students in UCs.

In conclusion, working on diversifying the UCs would be good, while it is difficult to increase applicants to UCs working on making the admittance rate percentages around the same number would be good to go towards.


For my reader, if you would like to you can check my work, you can. While the UC admissions data is a pain to work with because the data comes in multiple files and is encoded in utf-16le, I have consolidated all the data I used from the UC admissions data into one data frame:

{% include_relative Visualizations/UCDataCon.html %}

Also, here is a link to download all the code I used:

[UC Admissions Python File](https://drive.google.com/file/d/1E6izir4fjy9AapawBEvNEvForzPyTJct/view?usp=sharing)

As well as a folder of all the data frames I used:

[UC Admissions Data Files](https://drive.google.com/file/d/1khTUOeadGzKHnIAH9RYK9qq-trh-6jU6/view?usp=sharing)

And a folder of a the data visualizations I made in HTML format:

[Data Visualizations](https://drive.google.com/file/d/1DdoVO8G2ec8y2IQxbcByM-TQ6QqoBcTi/view?usp=sharing)