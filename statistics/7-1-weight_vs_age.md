[Think Stats Chapter 7 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2008.html#toc70) (weight vs. age)

###  Plot percentiles of birth weight versus mother’s age.
bins = np.arange(0, 20, 2.5)
indices = np.digitize(live.totalwgt_lb, bins)
groups = live.groupby(indices)

mean_weights = [group.totalwgt_lb.mean() for i, group in groups]
cdfs = [thinkstats2.Cdf(group.agepreg) for i, group in groups]

for percent in [75, 50, 25]:
    age_percentiles = [cdf.Percentile(percent) for cdf in cdfs]
    label = '%dth' % percent
    thinkplot.Plot(mean_weights, age_percentiles, label=label)
    
thinkplot.Config(xlabel='Weight (kg)',
                 ylabel='Age',
                 axis=[0, 16, 0, 50],
                 legend=False)


### Compute Pearson’s and Spearman’s correlations
print('Pearson Correlation Coefficient:,', Corr(live.totalwgt_lb, live.agepreg))
print('Spearman Correlation Coefficient:', SpearmanCorr(live.totalwgt_lb, live.agepreg))

#### Output
Pearson Correlation Coefficient:, 0.06883397035410907
Spearman Correlation Coefficient: 0.09461004109658228


### How would you characterize the relationship between these variables?
- Both of these results suggest very weak correlation between the two variables, close to no correlation at all.
- This reinforces what we see in both the scatterplot (which looks like a blob) and the CDFs which are fairly horizontal lines at each percentile. 
