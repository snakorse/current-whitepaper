# 附录二：去中心化的媒体

> #### Appendix 2: Decentralized Media

---

将大量的数据存储在Ethereum区块链上是非常昂贵的。星际文件系统（IPFS）可以在维护去中心化网络的同时做到这一点。IPFS是一个点对点的分布式文件系统，它将所有的计算设备与相同的文件系统连接起来。这些文件由其内容的散列哈希来寻址，而不是集中控制的位置。下面的图表显示了节点如何使用IPFS与实际的HTTP协议访问数据。

> It is cost prohibitive to store large amounts of data on the Ethereum blockchain. The InterPlanetary File System \(IPFS\) makes it possible to do so while maintaining a decentralized network. IPFS is a peer-to-peer distributed file system that connects all computing devices with the same system of files. The files are addressed by the hash of their content as opposed to a centrally controlled location. The diagram below shows how nodes access data with IPFS vs the de facto HTTP protocol.

IPFS将作为Current平台的数据存储层。Current将为用户提供CRNC，以鼓励他们在由IPFS驱动的网络上存储上传的文件。如果需要的话，Current会可以通过像Filecoin或IPFSstore这样的服务来实现额外的存储措施，在这些服务中，每一种媒体产品的可忽略的关税将被强加给创建者，并支付给那些在为上述服务网络中提供内容托管的人。

> IPFS will serve as the data storage layer of the Current platform. Current will offer users CRNC as an incentive to provide storage of uploaded files on the network powered by IPFS. If needed, Current may implement additional storage measures via services like Filecoin or IPFSstore where a negligible tariff per media item sold would be imposed on the creator and paid to whomever is hosting the content for the network on the aforementioned services.

为了使系统运行，Current还必须实现一个逻辑层，通过以太坊智能合约完成。合约以公平和透明的方式为创作者提供适当的内容支付。为了控制对ipfs托管内容的访问，我们使用了非对称加密机制。所有上传至当前IPFS网络的文件都会先用Current基金会的公钥加密。这可以在iOS应用程序中执行，并避免任何单点故障。

> In order for the system to operate, Current must also implement a logic layer, done via Ethereum smart contracts. The contracts provide creators with the appropriate payments for their content in a fair and transparent way. To control access to IPFS-hosted content, we employ an asymmetric encryption mechanism. All files uploaded to the Current IPFS network are first encrypted by the Current Foundation's public key. This can be performed in the iOS application, and avoids any single point of failure.

当用户想要下载数据时，IPFS地址散列哈希被发送到Current的API，该API将从IPFS网络下载文件，并使用Current基金会的私钥解密它。然后，将使用用户的公钥对跟踪数据进行重新加密，然后再提供给用户。

> When a user wants to download a track, the IPFS address hash is sent to the Current API which will load the file from the IPFS network, decrypt it using the Current Foundation's private key. The track will then be reencrypted using the user's public key, and then provided to the user.

这最后一步需要与我们的集中式API进行交互。当我们专注于构建一个稳定的、冗余的系统时，我们认识到这可能是网络中可能出现的单一故障点。在平台的这一阶段实现之前\(第一季度，2019年\)，我们期望在IPFS平台上看到改进，以允许更多的细粒度访问控制被包含在文件系统中。这将使我们可以采用完全去中心化的内容分发系统。

> This final step presently requires interaction with our centralized API. While we have focused on building a stable, redundant system we recognize that this presents a possible single point of failure in the network. Before this phase of the platform is implemented \(est. Q1, 2019\), we expect to see advancements in the IPFS platform to allow for more finegrained access controls to be included in the filesystem. This would allow us to employ a fully-decentralized content distribution system.

![](/assets/Centralized vs Decetralized Computing Model.png)

集中式体系结构表示多个客户机到单个服务器模型，其中服务器计算机是所有主要处理或存储完成的地方。一个去中心化的体系结构允许在多个计算节点之间进行处理，而没有单独的服务器机器负责所有的处理。

> A centralized architecture represents a multiple client to single server model where the server computer is the one where all of the major processing or storage is done. A decentralized architecture allows for processing to be distributed among multiple computeing nodes with no single server machine solely responsible for all the processing.

![](/assets/uploading content.png)

![](/assets/accessing content.png)

