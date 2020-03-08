# Confidence level Vs the accuracy of estimation of the population mean

Does the more the confidence level in the confidence interval mean more the accurate prediction of the estimation of the population mean?

## Confidence Interval

A confidence interval is the *range of numbers* that is believed to include an unknown population parameter.

## Confidence Level

It is the measure of confidence that the unknown parameter (of the population) lies within the confidence interval.

## A case study

Comcast, the computer services company, is planning to invest heavily in online television
service. As part of the decision, the company wants to estimate the average
number of online shows a family of four would watch per day. A random sample of
`100` families is obtained, and in this sample the average number of shows viewed
per day is `6.5` and the population standard deviation is known to be `3.2`. Construct a
`95%` confidence interval for the average number of online television shows watched
by the entire population of families of four.

### Known measures

- sample size - 
$$
n = 100
$$
- sample mean - 
$$ 
\bar{x} = 6.5
$$ 
- population standard deviation - 
$$
\sigma = 3.2
$$
- confidence interval
$$
Z = 1.96 (for the value of 95 percent)
$$

### To be found:

Confidence interval of within which the population mean i.e. the average number of online television shows are watched by the entire population

### Let's picturize it

![](https://i.imgur.com/eERtscN.png)

#### Let's understand the picture

![](https://i.imgur.com/yEdaHfO.png)

### Let's compute the confidence interval 

Confidence interval = 

$$
\mu \pm Z * (\sigma / \sqrt n)
$$

Since we don't know the population parameter $$ \mu $$ here, we will replate it with the value we know about the sample i.e. the sample mean $$ 
\bar{x} 
$$ 

So the confidence interval in this case is

$$
\bar{x} \pm Z * (\sigma / \sqrt n)
$$

When substituted with values above, we get

$$
confidence interval = 6.5 \pm 1.96 * (3.2 / \sqrt(100)
$$
 >Note: The Z value for 95% confidence is 1.96

We get the confidence interval as `[5.8728, 7.1272]`

### If we reduce the confidence level to 80%, what happens?

> Note: the Z score for 80% confidence is 1.282

$$
confidence interval = 6.5 \pm 1.28 * (3.2 / \sqrt(100)
$$

The confidence interval becomes `[6.0904, 6.9096]`

### Inference

So, when the confidence level decreases from 95% to 80%, the confidence interval becomes narrorwer - which would mean our chance of finding the population mean reduces by 15%

So it is better to always have a high confidence level to get more accurate estimations of the population mean

### What if i need to have a good confidence level i.e. 95% but the confidence interval should be narrower to get closer to the population mean - more accuracy in predicting?

Answer: Increase the sample size i.e. increase the sample size `n=100` provided above to `n=200`. 
