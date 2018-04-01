# 附录二：去中心化的媒体

> #### Appendix 2: Decentralized Media

---

===

> It is cost prohibitive to store large amounts of data on the Ethereum blockchain. The InterPlanetary File System \(IPFS\) makes it possible to do so while maintaining a decentralized network. IPFS is a peer-to-peer distributed file system that connects all computing devices with the same system of files. The files are addressed by the hash of their content as opposed to a centrallycontrolled location. The diagram below shows how nodes access data with IPFS vs the de facto HTTP protocol.

===

> IPFS will serve as the data storage layer of the Current platform. Current will offer users CRNC as an incentive to provide storage of uploaded files on the network powered by IPFS. If needed, Current may implement additional storage measures via services like Filecoin or IPFSstore where a negligible tariff per media item sold would be imposed on the creator and paid to whomever is hosting the content for the network on the aforementioned services.

===

> In order for the system to operate, Current must also implement a logic layer, done via Ethereum smart contracts. The contracts provide creators with the appropriate payments for their content in a fair and transparent way. To control access to IPFS-hosted content, we employ an asymmetric encryption mechanism. All files uploaded to the Current IPFS network are first encrypted by the Current Foundation's public key. This can be performed in the iOS application, and avoids any single point of failure.

===

> When a user wants to download a track, the IPFS address hash is sent to the Current API which will load the file from the IPFS network, decrypt it using the Current Foundation's private key. The track will then be reencrypted using the user's public key, and then provided to the user.

===

> This final step presently requires interaction with our centralized API. While we have focused on building a stable, redundant system we recognize that this presents a possible single point of failure in the network. Before this phase of the platform is implemented \(est. Q1, 2019\), we expect to see advancements in the IPFS platform to allow for more finegrained access controls to be included in the filesystem. This would allow us to employ a fully-decentralized content distribution system.

![](/assets/Centralized vs Decetralized Computing Model.png)

===

> A centralized architecture represents a multiple client to single server model where the server computer is the one where all of the major processing or storage is done. A decentralized architecture allows for processing to be distributed among multiple computeing nodes with no single server machine solely responsible for all the processing.

![](/assets/uploading content.png)

![](/assets/accessing content.png)

