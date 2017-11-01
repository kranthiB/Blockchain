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
        * Blockchain able to create distributed consensus between mutually distrustful parties, in many ways
          * allows to create an instantaneous single source of truth
          * able to record things in real time, up-t0-odate accounting of the state of the world.
          * not batch processing at night anymore
          * more of log-based system, so recording what was happened, as it is happening
            * its not business process type of software because it is a log / source of the truth / lot of other business logic will be based upon it.
      * if all the members of distributed ledger are participating in a closed network ( not in public / trustless environment) then they are known as permissioned.    
      * different hyperledger projects have different trade-offs
        * Fabric
          * more centralized ordering service
          * networks follow hub-and-spoke model
            * each peer connected to service will run either on one of the nodes, or on a neutral third party.
            * gossip messages that do the consensus mechanism go through a central hub
          * that sounds counterintuitive but they are distributed in a sense that the blockchain itself is replicated amongst all the nodes
          * your data is much more resilient to disruption
        * Sawtooth
          * more of like star model
            * they talk to each other, either one hub , or two hubs, or three hubs away, depending on the size of the network
        * Iroha
          * these are designed to function well in a mobile environment
            * mobile phones can be conneced or disconnected at random
            * structure is more of a layered network
              * end clients' mobile phones submit transaction to servers which then do the distributed ledger
        * Security is much same in all of these
          * use cryptography and digital signatures to validate all the messages
          * tampering messages is essentially impossible
          * immutability of distributed ledger is guaranteed by the cryptography
          * nature of trusted network(of permissioned) treat like any other back-office service
      * *Transactions* may involve the transfer of any asset or record of some service being rendered
        * Record of an event , cryptographically secured with digital signature, that is verified, ordered, and bundled together in to blocks, form the transactions in the block chain
        * *Smart Contract* with in the blockchain may allow automatic execution of transactions upon meeting predefined criteria.
        * *Cryptography* plays a key role in the security, as well as in the immutability of the transactions recorded on the blockchains
          * It ensures authenticity and immutability of the data being communicated
          * For blockchain technologies, Cryptography
            * used to prove that a transaction was created by the right person
            * also used to link transactions into a block in a tamper-proof way
            * as well as create links between nodes, to form a blockchain
      * Diferrences between Blockchains and Databases
        * blockchain is a write-only data structure, where new entries get appended ono the end of the ledger
        * new block gets appened to chain by linking previous block's 'hash'
          * Hash Function - It is used to map data of any size to a fixed length. The output of a hash function is referred to as a hash, hash value, or digest. One important characteristic of a hash function is that, when given a specific input, the hash function will always produce the exact same output.
        * There are no administration permissions within a blockchain that allow editing or deleting of data
        * blockchains designed for decentralized applications where as in relational databases ,single entity controls the data
        * ![image](https://user-images.githubusercontent.com/20100300/32273678-a89e27a6-bec0-11e7-9612-d5c97ae99519.png)
    * Permissioned and Permissionless blockchains and its key characteristics
      * permissionless like Bitcoin or Ethereum
        * also known as public blockchain
        * anyone can join the network
      * permissioned like different Hyperledger blockchain frameworks
        * private blockchain
        * requires pre-verification of participating parties within the network and these parties are usually known to each other.
        * supply chain management is an ideal use case
    * Various components of DLT including Consensus algorithms and smart contracts.
      * Peer-to-Peer Network Architecture
        * systems are directly connected to each other via the inernet without a central server
        * Peers contribute to the computing power and storage that is required for the upkeep of the network
        * do not have a single point of attack
        * Permissionless P2P systems do not require a set amount of peers to be online and are generally slower
        * Permissioned P2P networks have to guarantee uptime and require a high level of quality of service on the communication links.
        * ![image](https://user-images.githubusercontent.com/20100300/32274000-1dbe258a-bec2-11e7-9662-ed954e17bdcb.png)
      * Consensus
        * is a process whereby the peers synchronize the data on the blockchain.
        * mechanisms or algorithms
          * Proof of work
          * Proof of stake
          * Proof of Elapsed Time
          * Simplified Byzantine Fault Tolerance
          * Bitcoin and ethereum uses Proof of work currently, but they are moving towards proof of stake
          * The Hyperledger Sawtooth uses Proof of Elapsed Time.
       * Immutability of Data
         * *unchanging over time* feature makes the blockchain useful for accounting / financial transactions / identity management / asset ownership, management and transfer
         * Once a transaction is written onto the blockchain, no one can change it, or, at least, it would be extremely difficult to change it
         * it don't mean that the data can't be changed, it means it is extremely hard to change without collusion, and if you try, it's extremely easy to detect the attempt.
         * ![image](https://user-images.githubusercontent.com/20100300/32274352-b4b448a6-bec3-11e7-8d28-e96c6d32f304.png)
       * Blockchain applications
         * Financial transactions
           * bitcoins, UPort, KYC-Chain, Netki, etc.
         * Identity management and autentication
           * https://letstalkpayments.com/22-companies-leveraging-blockchain-for-identity-management-and-authentication/
         * Even more
           * https://www.coindesk.com/7-cool-decentralized-apps-built-ethereum/
       * Smart Contracts
         * computer programs that execute predefined actions when certain conditions within the system are met
         * provide the language of transactions that allow the ledger state to be modified
         * They can facilitate the exchange and transfer of anything of value 
           * e.g. shares, money, content, property 
         * ![image](https://user-images.githubusercontent.com/20100300/32274491-4d38f180-bec4-11e7-8030-91213d72db44.png)
    * High-level explanation of what Hyderledger is
      
            
 * References
   * https://courses.edx.org
   * https://www.safaribooksonline.com/library/view/mastering-blockchain/9781787125445/
   
