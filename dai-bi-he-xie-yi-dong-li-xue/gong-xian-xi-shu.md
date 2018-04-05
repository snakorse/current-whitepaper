## 贡献系数

> #### Contribution Coefficient \(H\)

---

并不是所有的用户消费都是平等的。贡献系数\(H\)旨在抑制不正当的播放，并确定最具影响力的网络贡献者。它是通过Current公司的一个集中式的oracle操作，通过Current平台的数据点来计算的，然后注入区块链。

> Not all user consumption is equal. The Contribution Coefficient \(H\) is designed to disincentivize illegitimate plays, and to identify the most influential contributors to its network. It is calculated with data points from the Current platform via a centralized oracle operated by the Current Corporation, then injected into the blockchain.

### 锥度系数

> #### Taper Coefficient

有很多原因可能不利于长期持续的采矿。首先，广告研究表明广告疲劳会降低人们的注意力; 其次，我们希望阻止消费者欺诈，比如让用户在没有真正关注的情况下“玩”媒体。

> There are many reasons to discourage long, continuous mining. Firstly, advertising research suggests that ad fatigue decreases attention; secondly, we want to discourage consumer fraud where users “play” media without authentically paying attention to it. We define a “session” as a time period of continuous mining with some minimum time apart from the next session. We designed a coefficient function in which marginal reward tapers off as session length increases. The cumulative award then is naturally its integral.

### 播放有效性验证

> #### Verifying Play Legitimacy

===

> The play legitimacy likelihood is a coefficient designed to prevent inauthentic plays from mining CRNC. This coefficient will be regularized so that it is consistent across the network in the majority of cases and 0 \(zero\) for identified frauds on a by-user basis. Our proprietary algorithm solves an anomaly detection problem based on features generated from Current platform usage, like app foreground consumption, advertisement interaction, and session velocity and length.

===

> This algorithm is computationally expensive, and presently the required data points are located off-chain. For these reasons, our anti-fraud checks will be performed by the off-chain Current API. We’ll consider moving these checks onchain once more of our data moves onchain, and if on-chain transaction costs fall to an affordable rate.

### 客户吸引力

> #### Customer Attractiveness

===

> The customer attractiveness ratio is a coefficient within 0 \(zero\) and 1 which represents the degree to which the user is integrated in the network, coupled with the likelihood that the consumer notices the ad.

===

> 1.Attractiveness of user based on attributes, learnt on data from advertisers and in-platform analytics
>
> * Country
>
> * Gender
>
> * Occupation
>
> * Age group
>
> * Income level
>
> * User preference data
>
> * App foreground vs background use
>
> * Calendar access
>
> * Location access
>
> * Number of accounts connected
>
>   * Spotify preference profile
>
>   * YouTube preference profile
>
>   * Third-party preference profiles

===

> 2.Likelihood of user interaction and clickthrough with ad, learnt on in-app data

===

> 3.Incentives for in-network participation

===

> Similar to verifying play legitimacy, this calculation requires a significant amount of data located off-chain, and would incur large transactions cost if performed onchain. For these reasons, the majority of these calculations will be conducted in an off-chain API.



