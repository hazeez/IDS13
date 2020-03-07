# Normal Distribution is a probability distribution.

### The topic in question is - Is normal distribution a probability distribution? Yes, it is and this writeup provides justification as to why it is so!

## Revisiting the Normal distribution

Let's revisit the normal distribution once - its characteristics and emprical rule

- Normal distribution is the distribution of data that is symmetric over the mean.
- `50%` of the data lie to the left and `50%` of the data lie to the right
- At the origin, mean = median = mode = 0

## Emprical rule 

The emprical rule states that
- `68%` of the data will be within one standard deviation of the mean 
- `95%` of the data will be within two standard deviations from the mean
- `99.7%` of the data will be within three standard deviations from the mean

Lets see that in the figure below
![](https://i.imgur.com/wESqJeE.png)

## Example Dataset

Let's plot a normal distribution graph of 300 people with a mean salary of `50,000` and standard deviation of `8700` (sigma)

|Descriptive Statistics| Value|
|-----------|-------|
| Mean      | 50000 |
| Median    | 50000 |
| Std dev p | 8700  |
| Mode      | 50000 |

Then the following will be the ranges of the salary from the mean.

|Sigma Range| Salary|
|----------|-------|
| -1 sigma | 41300 |
| +1 sigma | 58700 |
| -2 sigma | 32600 |
| +2 sigma | 67400 |
| -3 sigma | 23900 |
| +3 sigma | 76100 |

The number of people with the respective salary range and the normal distribution is mentioned below. 

| Salary Range | No of people | Norm Dist   |
|--------------|--------------|-------------|
| 23000-33000  | 0            | 0           |
| 33001-41000  | 64           | 0.00118224  |
| 41001-50000  | 88           | 0.003468298 |
| 50001-59000  | 87           | 0.003404399 |
| 59001-67000  | 63           | 0.001154427 |
| 67001-76000  | 0            | 0           |

> Normal distribution computed with NORMAL.DIST function in EXCEL

![](https://i.imgur.com/rtwEaK0.png)

So, we have all of our 300 people salaries mapped as a normal distribution.

## Random sample

Let's take a random sample from our range of salaries.
> NOTE: use the EXCEL `RANDBETWEEN` function to generate a random sample provided a range. Here our range is from `-3` sigma to `+3` sigma which is from `23900` to `76100`

The random sample i.e. salary taken is `47243` 

### Question?

What is the chance that this random sample (e.g. `47243`) falls within `-3` sigma to `+3` sigma? i.e. the area under the curve (highlighted in red color)?

![](https://i.imgur.com/2b1UohZ.png)

Can we say that `99.7%` of the time of the time the random sample taken will fall within the -3 sigma to +3 sigma (i.e. the area under the curve)

This `99.7%` chance is called as the probability of the sample falling within the range -3 sigma to +3 sigma. 

The range of Probability is from `0` to `1`. i.e `0` for no chance and `1` for 100% chance.

### One more sample

Let's take one more sample between `-3` sigma and `+3` sigma. What is the chance that it will fall under the area of the curve highlighted below (in red color) i.e. from `-1` sigma to `+1` sigma?

![](https://i.imgur.com/coj2nOq.png)

Can we say that it will be 68% or `0.68` probability? 

#### Lets prove it!

The area under the chart is from `-1` sigma to `+1` sigma. Correct?

Let's revisit Z (zee) scores once

> z scores is the number of units of standard deviation from the mean.

Here the range in consideration is `-1` sigma to `+1` sigma i.e we want to find out if a random sample (salary) falls within this range.

So the z scores are `-1` and `+1`. To be precise we can say `-1.0` and `+1.0`

Let's bring Z-Tables. 

Z-Tables provides us the area under the curve / probability. Using Z-tables lets find the area under the curve of `-1.0Z`
Since `-1` is a negative Z, we see the negative Z score table and see that the probability is `0.15866` (see figure below)

i.e if we take a random sample between `-3` sigma and `+3` sigma, the chance of the random sample falling under the area of the curve of `-1Z` is `15.866%`. Thus Z tables us gives the probability.

![](https://i.imgur.com/ee2w6eZ.png)


For `+1Z`, let's refer to the positive Z score table. The area under the curve is `0.84134`. (See fig below). 

![](https://i.imgur.com/e47TUn3.png)

To summarize, to find out the area under the curve `-1Z` to `+1Z` , we need to subtract the area under `+1Z` with `-1Z`

> Note: Zee is 1 unit of standard deviation. So it is -1 sigma to +1 sigma

i.e `0.84134 - 0.15866 = 0.68268`.

Thus `68.268%` is the probability that a given random sample will fall under the range of `-1` sigma to `+1` sigma.

In this way, we can find out the probability of a random variable falling under the area of the curve of the normal distribution for any Zee values. i.e from `-3` sigma to `-2` sigma. or from `-2` sigma to `+3` sigma etc.

## Conclusion

Thus we have emprically concluded that the normal distribution is a probability distribution as it helps to find the probability of a random variable falling within the normal distribution range.
 

