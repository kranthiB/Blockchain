# Blockchain 
  * **Overview**
    * Linux Foundation
      * Big data and analytics: ODPi, R Consortium
      * Networking: OpenDaylight, OPNFV
      * Embedded: Dronecode, Zephyr
      * Web tools: JS Foundation, Node.js
      * Cloud computing: Cloud Foundry, Cloud Native Computing Foundation, Open Container Initiative
      * Automotive: Automotive Grade Linux
      * Security: The Core Infrastructure Initiative
      * Blockchain: Hyperledger
      * https://www.linuxfoundation.org/
    * Distributed Ledger Technologies
      * Hyperledger
        * aims at advancing and promoting cross-industry blockchain technologies to ensure accountability, transparency, and trust among business partner.As a result, Hyperledger makes business network and transactions more efficient.
        * valued by many industries
          * technology
          * finance
          * healthcare
          * supply chain
          * automotive etc
        * offers different blockchain platforms
          * Iroha
          * Sawtooth
          * Fabric
        * https://www.hyperledger.org/
  * Discovering Blockchain Technologies
    * Blockchain and Distributed Ledger Technologies
      * It aims - *give explicit control of digital assets to end-users and remove the need to trust any third-party servers and infrastructure*
      * *Distributed Ledger* is a type of data structure which resides across multiple computer devices, generally spread across locations or regions
      * DLT includes blockchain technologies and smart contracts
        * Bitcoin blockchain marks the converence of host of technologies ,including
          * timestamping of transactions
          * Peer-to-Peer(P2P) networks
          * Cryptography
          * Shard Computational power
          * Consensus algorithm
      * DLT consists of three components
        * *Data Model* - captures the current state of the ledger
        * *Language Of Transactions* - that changes the ledger state
        * *Protocol* - used to build consensus among participants around which transactions will be accepted, and in what order , by the ledger.
      * What is blockchain technology?
        * P2P distributed ledger, forged by consensus, combined with a system for smart contracts and other assistive technologies
          * Together, these can be used to build a new generation of transactional applications that establish
            * trust
            * accountability
            * transparency at their core
        * while streamlining business process, with all distributed ledgers
          * there's an initial record or, in this case a block or genesis block
            * Each block will include one or more transactions
        * Connecting to block chain involves connecting to distributed ledgers via, typically, an application
        * Example - Wallet
          * a digital asset, like a crytocurrency, may transfer from one person to another and that asset will move from one's wallet to another wallet.Then, that transaction will be shown on a blockchain. So, this DL transaction, will move peer-to-peer through out the network, and there's no intermediaries, like a bank, or a payment company
          * These are best known for Bitcoin
          * Nodes / machines on a blockchain network group up these transactions and they send them throughout the network
          * On P2P, how do they sync up?
            * through concept of consensus - an agreement among the netwrok peers.
              * eventually, each machine has an exact copy of the blockchain throughout the network
        * *Smart Contracts* - computer programs that execute predefined actions when certain conditions within the system are met.
        * *Consensus*  - refers a system of ensuring that parties agree to a certain state of the system as the true state.
      * Blockchain
        * constructs a chronological chain of blocks
          * in Bitcoin blockchain, the miner nodes bundle unconfirmed and valid transactions into a block
          * miners solve crytographic challenge to propose the next block known as 'proof of work'
        * Block consists four pieces of metadata
          * reference to previous block
          * proof of work also known as nonce
          * timestamp
          * Merkle tree root for the transactions included in this block
            * also known as binary hash treee
            * it follows anti-tamper mechanism to ensure that the large dataset has not been changed
            * in bitcoin protocol
              * Merkle trees are used to summarize all the transactions in a block, producing an overall digital fingerprint of the entire set of transactions, providing a very efficient process to verify whether a transaction is included in a block
                * ![image](https://upload.wikimedia.org/wikipedia/commons/7/7a/Bitcoin_Block_Data.png)
              * http://chimera.labs.oreilly.com/books/1234000001802/ch07.html#merkle_trees
        
          
    * Permissioned and Permissionless blockchains and its key characteristics
    * Various components of DLT including Consensus algorithms and smart contracts.
    * High-level explanation of what Hyderledger is
 * References
   * https://courses.edx.org
   * https://www.safaribooksonline.com/library/view/mastering-blockchain/9781787125445/
   
