### ***Project 1 Feedback***

***Nico Van de Bovenkamp***

***

**Overall:** Good work on this! You wrote a very detailed exploratory analysis plan, with some nice pseudo code, that's pretty close to what you would actually want to do. Also, awesome job finding the Dixon's Q test. It's always a good idea to find more concrete methods for testing out assumptions and claims about the data.

**Some Notes**

* *Q.3a* Outliers will skew the mean, but what outliers will also impact the models that we build. We will discuss this in class, but we usually have to find some way to handle them intelligently.
* *Q.4a/b* We can definitely test/observe co-linearity via a regression, but  usually co-linearity will impact your regression and you want to investigate it before hand via a correlation matrix or some statistical test. Also, it's good to note that this is a linear relationship (a concept we will discuss further in class).

**Something to think about**

We touch on this a bit in class, but think about how you can apply statistical tests to your data. There are many handy tests to determine difference of means (very useful), tests to determine assumptions of an underlying distribution, etc. For example, there are specific tests which will estimate how close a given distribution is to a normal distribution.

You mentioned one method already, but check out this KDNuggets post for [outlier analysis](https://www.kdnuggets.com/2017/02/removing-outliers-standard-deviation-python.html) in Python!
