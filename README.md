# FM412-Quantitative-Security-Analysis-Project-1-P2-Sentiment-Analysis

This file concerns about the bias when maunnally reading submissions and comments in Reddit. It will provide insufficient sample space and may result in bias.
Therefore, I prefer to use the NLP method, by scraping the submissions and comments and do a sentiment analysis.

To aviod confusion, I used the commonly used pre_trained packages 'Bert', which rank sentences from 1 to 5. The higher, the more positive the sentence shows. Thus, any sentence below 3 should be regarded as negative and else are positive.

However, in this situation, this analysis may not work in this way. By checking through results, I found that many low number of sentiments actually are cynical and complaining itself, but it may result in a positive impact in the stock price of GME. 

Check this one:

'Could the masses turn MULN into the next GME? This company is 45% shorted at the moment...'

It is marked as 1.72 but actually shows that the author like the GME.

and also:

'Nah, it obviously means you are bought by Melvin Capital and Citadel and you had lunch with Vlad Tenev today to orchestrate a planned shutdown of WSB and RH at the same time to stop purchases from accelerating the price of GME to $69,420,420 and also your dad is Jerome Powell and the SEC and they made love to create you.'

There are so many negative words and it is marked as 1.89 but it shows positive impact to GME stock.

In that sense, I recognized that among the cynical people, one may need to lower the benchmark from 3 to 2, which might be fairer to find the positive and negative percentages.
