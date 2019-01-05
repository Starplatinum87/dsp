[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

# Code(PMF)
import numpy
nums = numpy.random.random(1000)
nums_pmf = thinkstats2.Pmf(nums)
thinkplot.Pmf(nums_pmf)
thinkplot.Config(xlabel='Numbers', ylabel='PMF')

# Code (CDF)
nums_cdf = thinkstats2.Cdf(nums)
thinkplot.Cdf(nums_cdf)
thinkplot.Config(xlabel='Numbers', ylabel='CDF')

# Analysis
- The PMF of this distribution looks like a massive block since every number within 1 - 10000 has a roughly equal probability (0.0010) of being chosen by the random function. As such we end up  a uniform distribution. This stronly implies that the random function does indeed choose numbers randomly. 
- The CDF has a very linear plot, further confirming that the random function chooses numbers randomly, with each number having the same probability of being chosen. 