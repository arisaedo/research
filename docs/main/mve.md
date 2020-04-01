# Minimum Viable Ecosystem (MVE)

> “the minimum ecosystem of stakeholders and value flows ” - RMIT Online

For the RMIT course, we will instead cover a very small subset of what this application will be able to provide. Initially, it will only cover the aspects of philanthropic donations to not-for-profit organisations.

## Key Stakeholders
The MVE consists of the minimum group of key players (users and actors) that must be involved for the core network to be successful and add value. 

### Contributors
1. Contribute the economy by providing public goods of any form
2. able to contribute directly to an open-source repository through version control services such as GitHub, BitBucket, GitLab, etc

### Organisations

1. large organisations like Facebook, Unicef, etc

### Philanthropist
1. dependent on open-source projects to build systems
2. for example, developers may need to use front end frameworks ( like Angular, Vue, React) to build a web application
3. methods
  - Philanthropist Miner
  - Philanthropist Contributor

## Digital Objects

A digital object is created and takes on the characteristics of a physical object by offering proof of:

- uniqueness – it exists only once
- ownership – who holds it now
- previous ownership – who held it
- history – what has happened to it (an improvement on physical objects)
- end of life – when it ceases to exist.

Having this single source of information about a digital object allows us to immediately determine the object's current state and verify its history.

In this context, properties related to a decentralised autonomous organisation (DAO) are modelled as a digital object.

1. Public Goods
  - the abstraction of a public good
  - it can in the form of source code, music, donations, etc
2. Maintainer
  - a person that is given the right to maintain a public good
  - can be the sole owner
  -joint ownership, etc
3. Proposal
  - the ability of a contributor to request funds through a formal proposal

## Architectural Strawman

A straw man is an early, low-fidelity proposal that is designed to be "torn down" as you move further through the design process. In the meantime, it provides reference and structure to prevent teams from working in a vacuum.

It covers:
- who the primary users are
- the platforms that the users will interact with
- the components that the platforms will interact with
- the micro-services proposed
- the data tiers
- analytics components
- standard tiers (inc security + DevOps and infrastructure)

From this, we can then define:
- Process View
- Data View
  - Objects
  - Relationships

## Transaction Accessibility

Transaction accessibility describes patterns on how "visible" a blockchain is; that is, who can join the network and "see" transactions.

Networks typically fall into one of the following categories:
- Public: Anyone can join the network by setting up a node to maintain a copy of the ledger and participate in the consensus process.
- Private: One or more organisations determine who can set up a node to join the network.
- Consortium: A variation of private networks (also called regulated networks). The ability to join the network, access data or submit transactions to the chain is limited, but not by a single organisation. Quorum and R3's Corda are examples of consortium networks.

## Transaction processing

Transaction processing can be used to describe how open the network is to transaction processors (i.e., which notes can process transactions). They can be described as permissioned and permissionless.

In a **permissioned network**, the identity of users is whitelisted (or blacklisted) through a know your business (KYB) or know your customer (KYC) procedure. By identifying participants, different permissions can be granted (e.g. read or write access).

In a **permissonless network**, the identity users are either anonymous (or pseudonymous). Anyone in the network can perform actions on the network (e.g. read or write transactions) and expect to see their transactions included on the chain if they are valid.

## Nodes

All nodes play a role in processing transactions. The level of processing depends on the blockchain platform. If we take two common patterns for nodes.

### Rudimentary Nodes
1. Fully Validating Nodes
  - Definition
    - Fully validating nodes are a technical solution pattern in which a node runs all validations defined by the specific DLT standard.
    - This means it validates the metadata of the chain (the “header information”) as well as the transaction data since the creation of the ledger.
  - Enabling Principle
    - Prepare for Failure: Vital to ensuring the validity of all aspects of the distributed ledger.
  - Benefits/force
    - Security: When a full validation and integrity check of the transaction is required.
    - Auditability: When the full integrity of the distributed ledger has to be guaranteed; when preserving the transaction history of a distributed ledger is required.
  - Risks/issues
    - Availability: Fully validating nodes may need to stay permanently online to ensure availability of all data.
    - Storage: Node has to store the entire chain with all its related data on the local system, which can lead to storage issues.
    - Performance: Performance is low compared to a lightweight node.
2. Lightweight Nodes
  - Definition
    - Lightweight nodes are a technical solution pattern – also called Simplified Payment Verification (SPV) pattern. 
    - Contrary to fully validating nodes, the lightweight nodes will not do a full validation of the entire chain including the transaction data, as originally required by the specific DLT standard. It may only validate the header information of the chain
  - Enabling Principle
    - Lightweight nodes are a technical solution pattern. It is also called Simplified Payment Verification (SPV) pattern.
  - Benefits/force
    - Performance: When performance is key or the storage of the device is limited.
  - Risks/issues
    - Security: As a full verification of the chain has been skipped, the integrity and validity of transactions cannot be ensured.
    - Availability: The lack of fully validating nodes poses a risk to the availability of data stored on the distributed ledger.


## Consensus Mechanisms

Distributed consensus is required when participants independently produce transactions and we require agreement about ordering and executing them. 

In a distributed system we can encounter two types of fault: benign faults and Byzantine faults. Benign faults are easy for the network to detect. Examples include a node becoming unresponsive, responding to a request with nonsense, or responding with an error message.

Byzantine faults, on the other hand, are much harder (or impossible) to be detected by peers. How could a peer detect when a node responds with a valid, but incorrect message? How can they know that a message has been intercepted and altered?

### Proof of Work
1. Definition
  - Each new block is asked to perform protocol called a proof of work. This is an asymmetrical problem; that is, it's time consuming and difficult to perform, but easy for others to verify.
  - For a block to be accepted by network participants, miners must complete a proof of work that covers all of the data in the block. For a block to be valid, it must hash to a value with x leading 0s. x can be varied to control the difficulty (and therefore frequency) of newly mined blocks.
  - Each block contains the hash of the preceding block, so each block has a chain of blocks that, together, contain a large amount of work. Changing a block (which can only be done by making a new block containing the same predecessor) requires regenerating all successors and redoing the work they contain. The blockchain is therefore protected from tampering.
2. Limitation
  - While proof of work solves the problem of reaching consensus in a distributed network, it does have limitations such as:
    - slow validating interval (high latency)
    - low throughput
    - energy consumption
    - cost of computational power to mine
    - risk of centralisation.

### Proof of Stake
1. Definition
  - Proof of stake is another way to validate transactions and achieve consensus. The probability of validating a new block is determined by the user's stake in the network (how many coins/tokens they possess) rather than their computational power. If two users make a stake (if User A stakes 10 coins and User B stakes 100), User B is 10x more likely to be chosen to validate the next block.
  - By cutting out the mining process, proof of stake offers a more energy-efficient solution and promotes network health, because users wishing to validate must own and support the coins/tokens they are verifying. The performance is somewhat better than proof of work, reducing the latency of validation and offering an increased throughput of transactions.

### Delegated Proof of Stake
1. Definition
  - Anyone that holds cryptocurrency can elect a list of nodes that can stake blocks to add to the blockchain. They are then allowed to create a number of blockchains, based on the number of their votes.

Now that we have elaborated on several alternatives of consensus mechanism, we’ll explore the consensus requirements for this system.

Well, it’s pretty clear that all miners that participate in the consensus agreement are technically philanthropist actors, hence, all the block rewards are donated back into the ecosystem. Therefore, it would be pretty nonsensical to have them fight for block rewards by staking coins (PoS) or having the most computation power (PoW). Also, we would like to keep the environmental effects to a minimal, henceforth, any consensus mechanism that requires an excess of computational power is negligible.

Henceforth, the consensus solution that is to be proposed in this context doesn’t require stake and computational power. Therefore, a deterministic-based Byzantine fault-tolerant (BFT) consensus can be applied in ease as there isn’t any incentive to reorg.

Hence, we propose an alternative solution that allows actors to gain reputation in the system by allowing them to participate in administrative and governmental decisions that occur in the organisations. So, in the effort of creating new blocks in the system, Philanthropist Miners are allocated “reputation” that allows them to create proposals, create organisations, request funds from the central fund, etc in the ecosystem. In other words, a fair-alternative to Proof-Of-Reputation is used (based on the awesome work done by Jiangshan Yu, David Kozhaya, Jeremie Decouchant and Paulo Esteves-Verissimo, refer to GitHub Research for more information).

## Smart Contracts

The primary goal of blockchains with inbuilt smart contracts was to create self-enforcing agreements that independently control and automate the exchange of value according to predetermined rules based on predefined inputs. From a business perspective, smart contracts represent the business rules.

### Opportunities
1. Logic-driven, simplified contracts that provide a clear statement of events, actions and triggers
2. Increased auditability of contracts by legal and compliance
3. Lower cost contracts by eliminating third parties
4. Automated action triggering (such as payments) based on contractual clauses
5. Increased security preventing contract tampering or change
6. Near-real time amendments to multi-party contracts

### Limitations
1. The current level of complexity is similar to the “triggers” in traditional databases or middleware logic
2. Language of smart contracts will be opaque to people who don't have a blockchain or coding background
3. The legislative framework is unclear about whether these contracts are enforceable
4. Do not deal well with ambiguity (e.g., if a scenario has not been accounted for)
5. Are the bugs in smart contracts defects or features? (Applications running on smart contracts need to be thoroughly tested)

### The lifecycle of a smart contract

There is a key problem here: How do you update when your contracts are immutable?

Smart contracts can be destroyed. Remove contracts when they outlive their usefulness or are no longer required; otherwise, like everything on a chain, they'll sit there forever and ever.

### Development Stages
1. Compile contract to bytecode for the Ethereum Virtual Machine (EVM), EVM bytecode is a stack-based bytecode language, similar to Java bytecode
2. Upload to the Ethereum blockchain
3. The execution of a particular function in the smart contract is then requested by clients and captured as a transaction.
4. Transactions are executed on the EVM
