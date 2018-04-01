# 附录一：比较分析和token动力学

> #### Appendix 1: Comparative Analysis and Token Dynamics

---

### Spotify

> #### Spotify

===

> As Spotify isn’t publicly traded, we rely here on news reports of Spotify’s financials . reported to its Luxembourg parent.

===

> Spotify ended 2016 with 126 million monthly active users, with 78 million \(62%\) free-tier users and 48 million \(38%\) paid subscriptions. However, 89.9% of its revenue, 2.64bn Eur., is driven by paid subscriptions. Due to cost of revenues, the gross profit on premium subscriptions was €483.8m, while Spotify’s ad-supported business recorded a gross loss of €33.3m.

===

> We assume that cost of revenue is driven by streaming royalties to record labels, PROs, back-office services, and publishers, approximated on a per-play basis. We use a EURUSD conversion rate of 1:1.2.

===

> **Total Cost of Revenue**

![](/assets/totalcost.png)

===

> **Estimated Cost of Revenue per User per Year:**

![](/assets/p7.png)

===

> We assume the average play generates $0.006 in royalties \(industry eCPM\):

===

> **Number of plays per average user per year:**

![](/assets/Number of plays per average user per year.png)

===

> Assuming that consumer valuations for Spotify Premium are solely driven by the avoidance of ads \(aside from other benefits, for instance mobile app usage or higher audio quality\):

===

> **Number of plays per average user per year:**

![](/assets/Number of plays per average user per yeard.png)

===

> Thus we estimate that Spotify Premium users overvalue each stream around 35% as compared to free tier users

### Pandora

> #### Pandora

===

> Pandora, in contrast with streaming music providers like Spotify and Current, acts as an internet radio provider -- which means its royalty and distribution model is somewhat different, and we track listener time, rather than number of legitimate plays. These figures are quoted from its financial statements: the 2016 10-K and 2016 Q3 10-Q.

===

> Like Spotify, there are more Pandora subscribers than there are free-tier. There were 74.5M free-tier users, and 4.39M subscribers in 2016. Its subscription-based service logged 2.79B total listener hours, as compared to 19.17B on the free advertising tier.

===

> We use the RPM metric \(revenue per thousand listening-hours\) provided on the Pandora 10-K \(only the first nine months are included, because the RPM metric is abandoned after Q3 2016\):
>
> **Advertising based RPM**
>
> ![](/assets/ok3.png)
>
> **Subscription based RPM**
>
> ![](/assets/ok2.png)

===

> By comparison - 80.98/58.10 - we arrive at an estimate of roughly a 39.4% increase in revenue per listening hour with the subscription viz. An advertising model. Keep in mind that Current’s RPM is slightly different than Pandora’s RPM in the sense that we have an enforced 30-sec minimum per track when counting listener time.

### ===

> #### Behavioral Dynamics

===

> Why do users pay more for subscriptions to get rid of ads?
>
> 1. Mental accounting. Individuals often assign expenditures to specific accounts, and constrain their spending differently across accounts in ways that often violate the economic principle of fungibility. Instead of viewing ads, which is a constantly salient expenditure of “attention,” users may file streaming subscription renewal fees under a “utilities” bucket, a decision frame in which expenditure “matters less.”
> 2. Salience. Advertising is a continuous demand on attention, whereas a monthly fee is a less salient, one-off expenditure.

===

> Why are there always more free-tier users than subscribers?
>
> 1. Consumers view free prices more highly irrespective of cost-benefit difference. By being free to use, Current leverages the “free” effect to make everyone subscribers.
> 2. Frictions for payment, like credit card validation and service fees, exist for currency transactions. Using CRNC tokens removes the frictions of small payments.

### ===

> #### Token Dynamics Visualization

===

> We calculate a rough projection for hours of play each day on the Current network by approximating an exponential growth rate, using figures from internal projections. We start with a rough projection for total hours of play by all users each day at 180 hours, high exponential growth in the first two months, and 25% per month for the first year. The block reward decreases over time linearly as more tokens are mined. We estimate the change of block reward using the block reward equation, and assuming that the growth pool stays at 4% of mined tokens.

===

> As total blocks mined increases exponentially over time, block reward per hour of streaming decreases exponentially:

![](/assets/p1.png)

===

> Afterwards, we estimate the token reward per listener hour. Using our Spotify average play revenue estimates from page 38 \(an eCPM of $0.006/legitimate play\), and minute length \(3 minutes\) and average contribution coefficient \(0.5\), we estimate the average token reward per hour the average listener listens.

![](/assets/p2.png)

===

> We use our Spotify estimate of revenue per hour of legitimate plays \($0.12\) divided by average token award \(0.25\) to arrive at a starting price estimate of $0.48 per token. As one token roughly represents how much economic value one hour of listening brings, so we estimate the price of a token given that it equals the revenue brought by its equivalent in Spotify listener time:

![](/assets/p3.png)

===

> Given that the average price of a Spotify subscription is $5.78, we estimate that the number of legitimate listening hours for a consumer to earn back a subscription is 43.7 hours.



