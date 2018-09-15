# Understanding the P-value

The P-value is one important yet often confusing concept in statistics, today I will be delving into it using layman's terms.

Before doing any hardcore statistics gymnastics, let's consider an example: 

As a "blameless" human being, I consistently maintain that on average I arrive in class on time, of course, with the exception of that "one" time where I am unfashionably late due to the rain and "uncontrollable factors". Seeing me coming to class late again, my statistics professor challenged my firm-held mental belief and said I always come to class around 10 min late. To that I said, “yes, however, even someone who consistently show up on time can be late once or twice, you cannot just use this one time I’m late to reject my perfect stellar record!” 

In statistics, my claim regarding my average arrival time is called a Null Hypothesis, and the professor’s alternative claim is an Alternative hypothesis. . If we take 0 to be on time, and 10 to be coming to class 10 minutes late. The null hypothesis would be $H_0=0$ and the alternative hypothesis would be $H_0$ is not 0 

How could the professor prove my claim (Null hypothesis) wrong?

One way is to randomly sample and average my arrival times, let’s say that it turns out to be 5. Okay, pretty clear that I am a late comer, right? 

Not so fast, it’s possible that even if my true average arrival time is 0, the arrival times you sampled will give you an average of 5 or greater. We call this probability the P-value. Without knowing the P-value, it’s impossible to make sense of this “5”.  Is the sample average 5 likely or unlikely to occur when the true mean is 0? 

To better make sense of the P-value, let’s take an extreme example, suppose that you sampled 1000 arrival times and yielded an average of 0.0001. Clearly not equal to 0. Can we reject the null hypothesis that the mean is 0? That would be absurd. The probability that even if the true mean is 0, the arrival times you’ve sampled is just slightly larger than 0 is extremely large. In other words, the p-value of sample mean=0 is extremely large.

On the other extreme, if the sampled average arrival time is 100, greater than the length of the lecture (in other words I skipped class altogether). We would clearly reject the null hypothesis that I come to class on time on average. In this case, the P-value( the probability that the true mean is 0 but the sampled mean is 100 or greater) is exceedingly small. 

Okay, now you might ask the golden question : where do we draw the line between a small P-value and a large one. Even if P-value = 0.01, isn’t there still 1 percent chance of the null hypothesis being correct? Are we not making an error if that is the case? In statistics, this type of error is called Type 1 error. When we do hypothesis testing, we need to constantly balance the evil of “wronging the good guy” and “letting the bad guy go free”. This whole trade-off is a subject of another day. For now, it’s good to know that “smart guys” have decided 0.05 a cut off point in P-value. If the P-value of a given statistic is less than 0.05, we reject the null hypothesis! 


