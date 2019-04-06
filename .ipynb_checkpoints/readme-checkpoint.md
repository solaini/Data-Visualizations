# Airline Cancellation Rates and Causes
## by Alexander Coffin


## Dataset

> The dataset I picked was the Flight information from 2004 to 2008 to determine what was the biggest cause for delays along with which carrier is historically the least reliable based on cancellations over the 5 year period.  This dataset has been pulled from a larger data set that was downsampled to compile a dataset that did not require 10+ seconds for processing.  Each year had 100000 samples pulled into a new dataframe for reference and to give the sampling a spread over the entire year.  2003 was not able to be included as parts of the data were corrupt causing an issue with combining the frames.

> In order to dig deeper into the data to answer the question of what the drove cancellations and who was the biggest culprit we needed to create a new dataset under Cancelled-Record.  This allows us to skip the data cleaning process and jump right into the analysis at a later date.


## Summary of Findings

> To start we saw that of the 500,000 samples from 2004 to 2008 roughly 2% of these are cancellations leading me to dig into the cause and most likely time that cancellations would occur.  After shrinking down the dataset and removing unnecessry columns we find that Wednesday and Sunday are the most unlucky days to fly when considering when cancellations occur.

>Digging further into a new dataframe, df_c we found that the cancellation through the week is bimodal leading to the thought that a pattern exists.  Although, our Carrier cause has an outlier in 2005 when Bad Weather seemed to be at an all time high and devestated almost 1600 of the 100,000 flights in the 2005 dataset.

>Finally, looking into a multivariable approach we see that new Carrier XE is not as polished as we htought and UA Airlines upped its game compared to the statistics.


## Key Insights for Presentation

> The key insights I have brought over to the presentation highlight the least reliable airline, WN Airlines and the worst times to fly.  As we see in the results we find that Carrier caused cancellations are the most prevelant causing WN to be completely at fault for their bad record as opposed to whether weather or NAS caused the problems.  In order to best present these findings I needed to relabel UniqueCarrier and CancellationCode so they are more easily identified in the graphs.



## Resources
>https://stackoverflow.com/questions/18603270/progress-indicator-during-pandas-operations-python 
>https://seaborn.pydata.org/tutorial/relational.html#relational-tutorial
>https://pythondata.com/visualizing-data-overlaying-charts/
>Udacity Reviewer from April 4th highlighting changes to meet specifications.