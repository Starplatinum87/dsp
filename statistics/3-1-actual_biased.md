[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

# Code
resp = nsfg.ReadFemResp()

under18_pmf = thinkstats2.Pmf(resp.numkdhh, label='under18_actual')
thinkplot.Pmf(under18_pmf)
thinkplot.Config(xlabel='Under 18 Children', ylabel='PMF')

biased18_pmf = BiasPmf(under18_pmf, label='under18_biased')
thinkplot.PrePlot(2)
thinkplot.Pmfs([under18_pmf, biased18_pmf])
thinkplot.Config(xlabel='Under 18 Children', ylabel='PMF')

print('Actual PMF for Under 18 Children in Household: ', under18_pmf.Mean())
print('Biased PMF for Under 18 Children in Household: ', biased18_pmf.Mean())

Results:
Actual PMF Mean for Under 18 Children in Household:  1.024205155043831
Biased PMF Mean for Under 18 Children in Household:  2.403679100664282

# Analysis
- There is a very significant difference in results between the biased and actual distributions and means, confirming that the class size paradox is very real.
- For the biased sample the mean for  households with more children have a mean that is twice that of the actual. 