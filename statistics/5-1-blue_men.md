[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

# Code
short_cent = 70/0.39370
tall_cent = 73/0.39370
mean = dist.mean()

# Convert to centimeters
print('5\'10" =', short_cent)
print('6\'1" =', tall_cent)
print(mean)

#Output
5'10" = 177.8003556007112
6'1" = 185.4203708407417
178.0

# Solution
shortest = dist.cdf(short_cent)
tallest = dist.cdf(tall_cent)
blue_men = tallest - shortest

print('Shortest Blue Man Percentile:', shortest)
print('Tallest Blue Man Percentile:', tallest)
print('Proportion of male population in Blue Man range:', tallest - shortest)

# Output
Shortest Blue Man Percentile: 0.489657445578779
Tallest Blue Man Percentile: 0.8323979423791308
Proportion of male population in Blue Man range: 0.3427404968003518