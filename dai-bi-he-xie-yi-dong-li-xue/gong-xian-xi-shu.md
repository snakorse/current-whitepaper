## 贡献系数

> #### Contribution Coefficient \(H\)

---

并不是所有的用户消费都是平等的。贡献系数\(H\)旨在抑制不正当的播放，并确定最具影响力的网络贡献者。它是通过Current公司的一个集中式的oracle操作，通过Current平台的数据点来计算的，然后注入区块链。

> Not all user consumption is equal. The Contribution Coefficient \(H\) is designed to disincentivize illegitimate plays, and to identify the most influential contributors to its network. It is calculated with data points from the Current platform via a centralized oracle operated by the Current Corporation, then injected into the blockchain.

### 锥度系数

> #### Taper Coefficient

有很多原因可能不利于长期持续的采矿。首先，广告研究表明广告疲劳会降低人们的注意力; 其次，我们希望阻止消费者欺诈，比如让用户在没有真正关注的情况下“玩”媒体。我们将“会话”定义为连续挖掘的时间周期，并且与下一节的时间间隔大于某一最小值。我们设计了一个系数函数，其中边际报酬随着会话长度的增加逐渐减少。总的奖励是他的自然积分。

> There are many reasons to discourage long, continuous mining. Firstly, advertising research suggests that ad fatigue decreases attention; secondly, we want to discourage consumer fraud where users “play” media without authentically paying attention to it. We define a “session” as a time period of continuous mining with some minimum time apart from the next session. We designed a coefficient function in which marginal reward tapers off as session length increases. The cumulative award then is naturally its integral.

### 播放有效性验证

> #### Verifying Play Legitimacy

播放合法性的可能性是一个旨在防止不真实的播放从采矿的CRNC中产生的系数。这个系数将被规范化，以便在大多数情况下，在网络上保持一致，并且在一个用户基础上识别出的欺诈行为为0\(0\)。我们的专有算法解决了基于Current平台使用生成的特征的异常检测问题，如app前台消费、广告交互、会话速度和长度。

> The play legitimacy likelihood is a coefficient designed to prevent inauthentic plays from mining CRNC. This coefficient will be regularized so that it is consistent across the network in the majority of cases and 0 \(zero\) for identified frauds on a by-user basis. Our proprietary algorithm solves an anomaly detection problem based on features generated from Current platform usage, like app foreground consumption, advertisement interaction, and session velocity and length.

该算法计算成本高，并且目前所需要的数据点位于链下。由于这些原因，我们的反欺诈检查将由链下 Current API执行。我们会考虑将这些检查转移到链上，当我们更多数据转移到链上，并且如果链上的交易成本降低到可以承受的程度。

> This algorithm is computationally expensive, and presently the required data points are located off-chain. For these reasons, our anti-fraud checks will be performed by the off-chain Current API. We’ll consider moving these checks onchain once more of our data moves onchain, and if on-chain transaction costs fall to an affordable rate.

### 客户吸引力

> #### Customer Attractiveness

客户吸引力比率是0\(0\)和1的系数，表示用户在网络中集成的程度，再加上消费者注意到广告的可能性。

> The customer attractiveness ratio is a coefficient within 0 \(zero\) and 1 which represents the degree to which the user is integrated in the network, coupled with the likelihood that the consumer notices the ad.

1. 用户吸引力基于从广告主和平台内数据学习的特征:

- 国家

- 性别

- 职业

- 年龄段

- 收入水平

- 用户偏高数据

- app前台和后台使用

- 日历访问

- 位置访问

- 关联账户数

    - Spotify偏好配置

    - Youtube偏好配置

    - 第三方偏好配置

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



> 2.Likelihood of user interaction and click through with ad, learnt on in-app data

==

> 3.Incentives for in-network participation

===

> Similar to verifying play legitimacy, this calculation requires a significant amount of data located off-chain, and would incur large transactions cost if performed onchain. For these reasons, the majority of these calculations will be conducted in an off-chain API.



