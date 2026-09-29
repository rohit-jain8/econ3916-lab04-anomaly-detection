# econ3916-lab04-anomaly-detection
# Robust Statistics -- Automated Anomaly Detection

## Objective

My goal in this project was to compare different summary statistics and anomaly detection methods to see how extreme values can affect the analysis of California Housing data.

## Methodology

- I analyzed California Housing data containing 20,640 observations.
- I compared the mean, median, trimmed mean, standard deviation, IQR, and MAD to see how different measures respond to extreme values.
- I manually implemented Tukey Fences to identify unusual housing prices.
- I used Isolation Forest to detect unusual observations based on multiple variables at the same time.
- I compared the observations identified by Tukey Fences and Isolation Forest to see where the two methods agreed and disagreed.
- I ran a contamination experiment by replacing 1,032 values, or 5.0% of the data, and compared how the different summary statistics changed.

## Key Findings

I found that Tukey Fences and Isolation Forest can identify different observations because they look for anomalies in different ways. Tukey Fences focused on unusual housing prices, while Isolation Forest considered multiple characteristics at the same time. The contamination experiment also showed a large difference in how the summary statistics reacted to extreme values. After 5.0% contamination, the mean shifted by 67.13%, while the median shifted by only 3.56%. This showed me that the median was much less affected by the extreme values than the mean.
