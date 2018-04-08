# 附录一：比较分析和token动力学

> #### Appendix 1: Comparative Analysis and Token Dynamics

---

### Spotify

> #### Spotify

由于Spotify没有公开交易，我们在这里依靠的是Spotify财务状况的新闻报道。向其卢森堡母公司的报告。

> As Spotify isn’t publicly traded, we rely here on news reports of Spotify’s financials. reported to its Luxembourg parent.

Spotify在2016年的月活跃用户数为1.26亿，其中有7800万（62%）的免费用户，以及4800万（38%）的付费订阅用户。然而，其收入的89.9%，即264亿欧元。是由付费订阅驱动的。由于收入的成本，高级订阅的毛利润为4838万英镑，而Spotify的广告支持业务则录得33.3亿欧元的总亏损。

> Spotify ended 2016 with 126 million monthly active users, with 78 million \(62%\) free-tier users and 48 million \(38%\) paid subscriptions. However, 89.9% of its revenue, 2.64bn Eur., is driven by paid subscriptions. Due to cost of revenues, the gross profit on premium subscriptions was €483.8m, while Spotify’s ad-supported business recorded a gross loss of €33.3m.

我们认为，收入的成本是由流媒体版税向唱片公司、专业人士、后台服务和出版商提供的，以每一次播放为基础。我们使用的是1:2的欧洲美元换算率。

> We assume that cost of revenue is driven by streaming royalties to record labels, PROs, back-office services, and publishers, approximated on a per-play basis. We use a EURUSD conversion rate of 1:1.2.

收入的总成本

> **Total Cost of Revenue**

![](/assets/totalcost.png)

估计每个用户每年的收入成本：

> **Estimated Cost of Revenue per User per Year:**

![](/assets/p7.png)

我们假设平均播放产生的版税为0.006美元（工业eCPM）：

> We assume the average play generates $0.006 in royalties \(industry eCPM\):

平均每个用户每年的播放次数：

> **Number of plays per average user per year:**

![](/assets/Number of plays per average user per year.png)

假设Spotify Premium的消费者估值完全是由免广告（除了其他好处，比如移动应用使用或更高的音频质量）驱动的：

> Assuming that consumer valuations for Spotify Premium are solely driven by the avoidance of ads \(aside from other benefits, for instance mobile app usage or higher audio quality\):

平均每个用户每年的播放次数：

> **Number of plays per average user per year:**

![](/assets/Number of plays per average user per yeard.png)

因此，我们估计，与免费的用户相比，Spotify的高级用户对每条流的估值超过了35%。

> Thus we estimate that Spotify Premium users overvalue each stream around 35% as compared to free tier users

### Pandora

> #### Pandora

与Spotify和Current等流媒体音乐提供商相比，Pandora是一家互联网广播提供商——这意味着它的版权和分销模式有所不同，我们追踪听众的时间，而不是合法的播放次数。这些数据来自其财务报表：2016年10-K和2016年第三季度10-q。

> Pandora, in contrast with streaming music providers like Spotify and Current, acts as an internet radio provider -- which means its royalty and distribution model is somewhat different, and we track listener time, rather than number of legitimate plays. These figures are quoted from its financial statements: the 2016 10-K and 2016 Q3 10-Q.

和Spotify一样，Pandora的订阅用户数量也超过了免费用户。在2016年，有7450万的免费用户，以及439万用户。其基于订阅的服务记录了279 B的总听众时间，而免费广告层的服务时间为19.17亿。

> Like Spotify, there are more Pandora subscribers than there are free-tier. There were 74.5M free-tier users, and 4.39M subscribers in 2016. Its subscription-based service logged 2.79B total listener hours, as compared to 19.17B on the free advertising tier.

我们使用在Pandora 10-K上提供的RPM度量（每千个听小时的收入）（只包括前9个月，因为在2016年第三季度之后，RPM度量被放弃）：

**基于RPM的广告**

14.53B listening hours = $58.10

**基于订阅的RPM**

2.04B listening hours = $80.98

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



