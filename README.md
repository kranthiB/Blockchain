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
          * Proof of Burn
          * Proo of capacity
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
  * Bitcoin Blockchains
    * global decentralized payment network
    * distributed and publicly-owned infrastructure, operating as 'permissionless' system.
    * One of the biggest inventions and problems that it solved was that of the **double spend**  problem
    * is focused upon transferring monetary value between parties, it has a very limited programming language
    * *Bitcoin and Cryptoeconomics*
      * is about building systems that have certain desired properties using cryptography to prove properties about messages that happened in the past while using economic incentives defined inside the system to encourage desired properties to hold into the future
      * in permissionless blockchains, rather than imposing barriers to entry , its open for anyone to join including malicious actors
        * key lies in incentivizing good behavior in a critical majority of the network,such that
          * The malicious actors cannot take over the network through an **escalated attack**.
          * The malicious actors cannot **collude** to undertake an organized majority attack on the network.
          * The **payoffs** of securing the network are consistently higher than the cost of attacking the network.
          * The **cost** of attacking the network is prohibitively high.
      * https://medium.com/@cryptoeconomics/the-blockchain-economy-a-beginners-guide-to-institutional-cryptoeconomics-64bf2f2beec4
  * Ehereum Blockchains
    * Ethereum is an open blockchain platform that lets anyone build and use decentralized applications that run on blockchain technology
    * facilitates **scripting functionality**, or **smart contracts**,
      * unlike the bitcoin blockchain, it does not track transactions, it also programs them
    * uses a more expansive set of programming languages and tools to allow for many other types of programs and applications
    * EVM or Ethereum Virtual Machine
      * it runs on the Ethereum network as a Turning-complete software with its native crytocurrency called **ether**
    * Key features
      * immutability of data 
      * unauthorized users cannot make changes of data
      * is desgined to make corruption and tamper proof applications
      * secure apps are sent decentralized and secured with cryptograpy
        * they are processed against hacking attacks and fraudulent activities
      * is designed with zero downtime
        * not run on central servers in a certain geographical location
        * Instead, the computing power that runs the network is contributed by nodes that are spread across the globe
        * they never go down and, in general, cannot be switched off
      * if some of the machines go down, network maintains a stable state
    * *Dapps*
      * Decentralized applications
      * they are cryptographically secured
      * can referred as 'secure applications'
      * Example applications are
        * **Augur**, which is a Decentralized Prediction Market. Learn more at https://augur.net/.
        * **Digix**, which tokenizes gold on Ethereum. Learn more at: https://digix.global/.
        * **Maker**, which is a Decentralized Autonomous Organization (DAO). Learn more at: https://makerdao.com/.
    * *Smart Contracts*
      * hypothetical example
        * in an equity raise, transfer amount X from the investor to the company upon receiving the given shares from the company
        * The monetary amount X, which was pre-validated by the company for the transaction (much like in a credit card purchase), is held in escrow by the smart contract, until the shares have been received by the investor
        * Any kind of arbitrary sophisticated business logic can be committed to the blockchain
        * Ethereum blockchain only encodes these 'rules of the games'
        * The actual payoffs occur by interacting with the blockchain
      * ![image](https://user-images.githubusercontent.com/20100300/32277497-dfa9e6fe-becf-11e7-81a0-191f2e940eda.png)
        1. The smart contract encodes the agreement between the company raising funds and its investors (Panel 1)
        2. The smart contract sits on the Ethereum public blockchain, and is run on the Ethereum Virtual Machine (EVM). Once hitting a triggering event, like an expiration date or a strike price that has been pre-coded, the smart contract automatically executes as per the business logic (Panel 2)
        3. As an added benefit, regulators are able to scrutinize the market activity on an ongoing basis, without compromising the identity of specific players in a permissionless public blockchain, as Ethereum (Panel 3).
    * **Note:** With the advent of the Ethereum blockchain platform and the scripting functionality or smart contracts that it enables, there are ongoing attempts to do the same for the Bitcoin blockchain, which does not allow for this, due to security reasons. **RSK**(http://www.rsk.co/) is one such smart contract platform that seeks to achieve this "with a 2-way peg to Bitcoin". The added functionality can go a long way in making the Bitcoin blockchain useful for use cases other than cash transfers.  
 * Exploring Permissionless Blockchains
   * will look at block heights, transaction times, mining pools, timestamps, and block rewards
   * Bitcoin
     * Blocks info - https://blockchain.info/home
       * ![image](https://user-images.githubusercontent.com/20100300/32278012-806c5a58-bed1-11e7-942c-886157384ecf.png)
         * *Height* indicates number of blocks in a particular blockchain
         * *Transactions* column shows how many transactions included in a block
         * *Total Sent* amount of Bitcoin that was transferred in each of those blocks
         * *Relayed By* column - miner or mining pool that created that block
     * Genesis Block - https://blockexplorer.com/block/000000000019d6689c085ae165831e934ff763ae46a2a6c172b3f1b60a8ce26f
   * Ethereum
     * Blocks info - https://etherscan.io/blocks
     * Genesis Block - https://etherchain.org/block/1
       * mining reward for this was 5 ether.
   * example - the purchase of pizza for 10,000 bitcoins
     * ![image](https://user-images.githubusercontent.com/20100300/32278835-26e2d216-bed4-11e7-83bd-8002ed6ca23d.png)
     * ![image](https://user-images.githubusercontent.com/20100300/32278895-5b84dd2a-bed4-11e7-83f7-bc9f19085eef.png)
     * ![image](https://user-images.githubusercontent.com/20100300/32278935-7aa6fe4a-bed4-11e7-927c-9be4892fb47c.png)
   * 'Certifying' a Document
     * using Stamp.io, which is a certification tool
       * https://stamp.io/
       * easily obtaining a 'Stampery Certificate' which indicates
         * name of the file
         * when it was added to Stampery
         * person who signed it
       * ![image](https://user-images.githubusercontent.com/20100300/32282050-c908c95c-bedd-11e7-8d73-73a5059f928d.png)
         * hash of this document was stored in transactions which were placed in various blocks on both Ethereum and the bitcoin blockchain
       * we can open this transaction in ethereum using https://etherscan.io/tx/*transaction-id*. We can see
         * timestamp
         * particular block 
 * Consensus Algorithms
   * it refers to process of achieving agreement among the network participants as to correct the state of data on the system
   * it leads to all nodes sharing the exact same data
   * it prevents malicious actors from manipulating the data
   * *Proof of Work(Pow)*
     * involes solving a computaional solving puzzle in order to create new blocks in the bitcoin blockchain. This process is known as *mining* and the networks that engage in mining are known as *miners*
     * is the outcome of a successful mining process and, although the proof is hard to create, [it] is easy to verify
     * https://99bitcoins.com/proof-of-work-proof-of-stake/
     * requires a huge amount of energy to be expended, given the computationally heavy algorithm
     * has a high latency of transaction validation
     * concentration of mining power is located in countries where electricity is cheap
     * In terms of the network security
       * PoW is susceptible to the '51% attack', which refers to an attack on a blockchain by a group of miners controlling more than 50% of the network's computing power
   * *Proof of Stake (PoS)*
     * generalization of the Proof of Work algorithm
     * nodes are known as the 'validators'
       * rather than mining the blockchain, they validate the transactions to earn a transaction fee
     * Simply put
       * nodes are randomly selected to validate blocks, and the probability of this random selection depends on the amount of stake held
         * if node X owns 2 coins and node Y owns 1 coin, node X is twice as likely to be called upon to validate a block of transactions
     * specific implementation of PoS can vary, depending on the use case, or as a matter of software design
       * Instances include **Proof of Deposit** and **Proof of Burn**
     * saves expensive computational resources that are spent in mining under a PoW consensus regime
   * **Proof of Elapsed Time (PoET)**
     * emulates the Bitcoin-style Proof of Work
     * Hyperledger's Sawtooth implementation is an example of PoET at work
       * The validator with the shortest wait time for a particular transaction block is elected the leader.
       * This "leader" gets to create the next block on the chain
     * instead of mining the next block, PoET is a hybrid of a random lottery and first-come-first-serve basis
     * each validator is given a random wait time.
   * **Simplified Byzantine Fault Tolerance (SBFT)**
     * implements an adopted version of the Practical Byzantine Fault Tolerant (PBFT) algorithm - https://blog.acolyer.org/2015/05/18/practical-byzantine-fault-tolerance/
     * involves a single validator who bundles proposed transactions and forms a new block 
     * unlike the Bitcoin blockchain, the validator is a known party, given the permissioned nature of the ledger
     * Consensus is achieved as a result of a minimum number of other nodes in the network ratifying the new block
     * In order to be tolerant of a Byzantine fault,
       * the number of nodes that must reach consensus is 2f+1 in a system containing 3f+1 nodes, where f is the number of faults in the system
         * For example, if we have 7 nodes in the system, then 5 of those nodes must agree if 2 of the nodes are acting in a faulty manner
     * Example - http://hackingdistributed.com/2016/08/04/byzcoin/
       * key improvements over the original Bitcoin protocol
         * Addressing the challenge around scalability due to high latency
         * ByzCoin transactions are irreversibly committed to the blockchain within seconds
         * added advantage is the communication trees to "(...) optimize transaction commitments and verification under normal operations
   * **Proof of Authority (PoA)**
     * can be used for permissioned ledgers
     * uses a set of 'authorities', which are designated nodes that are allowed to create new blocks and secure the ledger
     * using PoA require sign-off by a majority of authorities in order for a block to be created.
   * **Comparing Permissioned Consensus Approaches and Standard PoW**
     * lottery-based algorithms - PoET / PoW
     * voting-based methods - SBFT
     * Lottery-based algorithms are advantageous in that they can scale to a large number of nodes
     * Voting-based algorithms provide low-latency finality.
     * ![image](https://user-images.githubusercontent.com/20100300/32283552-e73ea546-bee1-11e7-9c70-5dfdd6030454.png)
 * Hyperledger
   * open source effort created to advance cross-industry blockchain technologies
   * boasts a host of enterprise-ready solutions.
   * are generally permissioned blockchains
     * means that the parties that join the network are authenticated and authorized to participate on the network.
   * main goal is to create enterprise grade, open source, distributed ledger frameworks and code bases to support business use cases
   * Advantages of Using a Permissioned Blockchain over a Permissionless Blockchain
     * permissionless blockchains - 
       * anyone can join the network, as well as write and read transactions
       * there could be some malicious actors within the network as actors in the system are not known
     * provides all the capabilities of the blockchain architecture - data privacy, information sharing, immutability, with a full stack of security protocols - all for the enterprise
 * Other DLT
   * Chain Core 
     * created by chain.com
     * intially has been designed for financial serve institutions
     * for things like security / bonds / currencies has strong ties with Visa / Citygroup and Nasdaq
     * is an enterprise permissioned blockchain system that is mostly focused on financial services, like currencies, securities, derivatives, gift cards, and loyalty points
     * the creation and transfer of assets is decentralized
     * https://chain.com/technology/
   * Corda
     * designed to record / manage and automate legal agreements between businesses
     * creaed by R3
     * which features a blockchain-style P2P network; however, it is not a blockchain platform
       * Unlike blockchains, which involve global availability of data across the network and third party validators, Corda only allows information access and validation functions to parties actually involved in the transaction
     * https://www.corda.net/
   * Quorum
     * is permissioned implementation of ethereum 
     * which supports data privacy
       * it achieves this by allowing data visibility on need-to-know basis by voting based consensus algorithm
     * it's an open source created by JPMorgan 
     * is designed to support "both transaction-level privacy and network-wide transparency"
     * The network validates all smart contracts and overall system state through the involvement of all running nodes
     * As with other permissioned ledgers, regulatory compliance is front and center in the Quorum platform
   * IOTA
     * It is the first cryptocurrency that provides the whole ecosystem based on blockless blockchain" to enable machine-to-machine (M2M) transactions
     * is more than just a cryptocurrency
     * the platform entails a generalization of the blockchain protocol (the technology called Tangle) that sits at the backend of the IOTA platform.
     * Instead of paying miners to validate the transactions, the architecture of the network involves peer-based validation
       * This allows the platform to be completely free of cost, without facing the scaling challenges that are inherent in the first generation of blockchains. 
 * Challenges in the Adoption/Deployment of Distributed Ledger Technologies
   * number of challenges to the widespread use of permissioned distributed ledger technologies
     * Key among them are challenges around the lack of standards, regulatory challenges, and the lack of knowledge about distributed ledger technologies
 * Standards
   * https://www.iso.org/committee/6266604.html
   * ![image](https://user-images.githubusercontent.com/20100300/32312191-659a36c2-bfc2-11e7-8f89-f9738ea3bac1.png)
 * Regulation
   * the lack of regulation around transactions on the blockchain creates an environment of uncertainty for all players
   * no regulatory guidelines governing smart contracts, causing much anxiety among various players like lawyers, regulators, programmers, and businesses
   * lack of regulatory guidelines, along with a lack of industry standards, exacerbates hindrances to rapid adoption of DLT
 * Lack of Know-How
   * The lack of know-how (and know-whom and know-where) around distributed ledger technologies and the availability of experts in the area is a major challenge in the adoption of distributed ledger technologies
   * https://coin.dance/stats/blockchain
 * The Promise of Buisness Blockchain Technologies
   * Blockchain use case
     * Supply Chain Management
     * Provenance
     * Property Rights
 * Technical Requirements
   * cURL
   * Node.js
   * npm package manager
   * Go Language
   * Docker
   * Docker Compose
   * VirtualBox (for windows)
 * Hyperledger Sawtooh (Usecase)
   * consensus algorithm Proof of Elapsed Time
   * transaction families
   * batches
   * validators
   * Defining Our Actors
     * **Sarah** is the fisherman who sustainably and legally catches tuna.
     * **Tuna processing plant** processes and bags the tuna after they have been caught.
     * **Regulators** verify that the tuna has been legally and sustainably caught.
     * **Miriam** is a restaurant owner who will serve as the recipient in this situation.
     * ![image](https://user-images.githubusercontent.com/20100300/32329225-66687150-c002-11e7-8310-1bf721dd8a87.png)
 * **Terminology**
   * *Block* - A set of transactions that are bundled together and added to the chain at the same time.

   * *Byzantine Fault Tolerance Algorithm* - A consensus algorithm designed to defend against failures in the system caused by forged or malicious messages. In order to be fault tolerant of a Byzantine fault, the number of nodes that must reach consensus is 2f+1 in a system containing 3f+1, where f is the number of faults in the system. 

   * *Chaincode* - Smart contracts in Hyperledger Fabric. They encapsulate both the asset definitions and the business logic (or transactions) for modifying those assets.

   * *Consensus Algorithm* - Refers to a system of ensuring that parties agree to a certain state of the system as the true state.

   * *Cryptocurrency* - is a digital asset that is used as a medium of exchange. A cryptocurrency is exchanged by using digital signatures to transfer ownership from one cryptographic key pair to another key pair. Since this digital asset has characteristics of money (like store of value and medium of exchange), it is generally referred to as currency. Note: It should not be confused with digital currency or virtual currency.

   * *Cryptoeconomics* - A field of study that explores the intersection of cryptography and economic incentives. While cryptography is used for ensuring network security at various levels and functions, the built-in economic incentives provided to the participating nodes in the network ensure that, at any given point, the majority of players in the network operate in a desirable way. 

   * *Cryptography* - The study of the techniques used to allow secure communication between different parties, and to ensure the authenticity and immutability of the data being communicated.

   * *Distributed Ledger* - A type of data structure which resides across multiple computer devices, generally spread across locations and regions.

   * *Hash Function* - It is used to map data of any size to a fixed length. The output of a hash function is referred to as a hash, hash value, or digest. One important characteristic of a hash function is that, when given a specific input, the hash function will always produce the exact same output.

   * *Key/Value Pair* - It consists of two parts, one designated as a 'key', and another as a 'value'. The 'key' is an identifier that allows you to look up the 'value'. The 'value' is the data that is stored for a given 'key'.

   * *Mining* - The process of solving computational challenging puzzles in order to create new blocks in the Bitcoin blockchain.

   * *Node* - Computer device attached to a blockchain network. Types of nodes include: mining nodes, validator nodes, committer nodes, and endorser nodes. Nodes are sometimes also called 'peers' because they make up the devices within a peer-to-peer network.

   * *Peer-to-Peer Network* - A network witch consists of computer systems which are directly connected to each other via the Internet without a central server.

   * *Private/Public Keys* - Private keys are used to derive a public key. While private keys remain confidential, public keys are available to everyone in the network (similar to an email address). Anything encrypted with a public key can only be decrypted using its corresponding private key, and vice versa. 

   * *Proof of Elapsed Time (PoET)* - Consensus algorithm used by Hyperledger Sawtooth that utilizes a lottery function in which the node with the shortest wait time creates the next block. 

   * *Proof of Stake (PoS)* - Consensus algorithm where nodes are randomly selected to validate blocks, and the probability of this random selection depends on the amount of stake held.

   * *Proof of Work (PoW)* - Consensus algorithm first utilized by Bitcoin that involves solving a computational challenging puzzle in order to create a new block.

   * *Smart Contract* - Computer program that executes predefined actions when certain conditions within the system are met. Smart contracts were first proposed by Nick Szabo in 1996 (http://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/szabo.best.vwh.net/smart_contracts_2.html).

   * *State* - Contains up-to-date data that represents the latest values for all keys included in the network's ledger. The state of a network encompasses all past transactions in the network, from the genesis block to the present time.

   * *Transaction* - A record of an event, cryptographically secured with a digital signature, that is verified, ordered, and bundled with other such records into blocks. 

   * *Transaction Families* - Smart contracts in Hyperledger Sawtooth. They define the operations that can be applied to transactions. Transaction families consist of both transaction processors (the server-side logic) and clients (for use from web or mobile applications).

   * *Turing-Complete* - Named after Alan Turing, an English mathematician and computer scientist, it refers to a computer that can solve any problem that a Turing Machine can. A Turing Machine is a machine that can simulate any computer algorithm, no matter how complicated. Bitcoin scripting language is not Turing-Complete, as there are no looping and branching types of computing sequences. Ethereum's Solidity language is considered Turing-Complete, as it does have looping and branching.
            
 * **References**
   * https://courses.edx.org
   * https://www.safaribooksonline.com/library/view/mastering-blockchain/9781787125445/
   
