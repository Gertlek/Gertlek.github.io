---
layout: post
title: Nuances in leveraged ETFs
categories: [Miscellaneous, Jekyll]
---

Long term, indices go up. So why not leverage this and achieve higher returns? Why is the standard 0% leverage? We will try to answer this.

Let us first introduce leveraged ETFs. In 2022, inflows for leveraged ETF have doubled compared to 2021. Now representin 5% of all ETF purchases. The most common leveraged ETF is a daily rebalanced etf that uses total return swaps to amplify or invert returns. For example, the S&P 500 ETF (SPY) rising 5 %, the 2x SPY ETF would rise approximately 10 %. A simplified example that over a given time period, 2x ETF does not imply 2x returns. In this example, the returns alternate 4 times between +10% and -10%.


| SPY                  |   2x SPY             | 
|--------------------- | ---------------------|
| 1.1			     | 1.2			    |
| 0.99 		     | 0.96 		    |
| 1.09		     | 1.15                 |
| 0.98 		     | 0.92			    |

In this simplified example, we have omitted management fees and interest expenses.  Management fees are usually higher due for leveraged etf's, around 0.75 % anually.
Any online sources on leveraged etfs dont dive into interest expenses, while I theorize in this article that this is the most import denominator for out/under-performance.

## Perfect world

We will return to SPY later, but now consider the MSCI all world index. Since this data set was freely accesible from 1999. 
Suppose we live in a perfect world, without management fees and interest expenses. MSCI going up 10% implies 2x MSCI going up 20%.  But the downside is also doubled. Would we have outperformed the index historically?

![](/images/msci2.png)

We notice fast outperformance in this perfect world against the index over the last 23 years. But inspecting the graph, we have periods of underperformance and the large outperformance is in periods where the market is continually moving up. 

### Interest and management expenses

Let us now compute the leveraged return under different levels of interest + management expense. From 1-7 %. And see at what level of interest rate + management expense (r) we still outperform the unlevered index: 

![](/images/mscir.png)

In the above plot, we see that with r > 0.04, we dont outperform anymore! Since we have double the downside, we should want adequate return as compensation. Perhaps only r < 0.02 is sufficient outperformance? We will now proceed to do something which has received little to no public attention, and maybe for more nefarious reasons. Can we find out what r is in a real levered index? 

## Reverse engineering r

Let us
