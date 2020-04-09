## Timeline

A complete overview of the timeline and decisions made during the inception of Floyd Economy.

**16/11/2019** - Floyd Economy project inception, whereby, the project is focused on achieving a decentralised gig economy platform that allows developers to fund projects, work on bounties, etc. This project is inspired by the awesome work done by the Gitcoin.co community that allows funding of grants, bounty hunting, etc. However, limitations current exists in these solutions, hence, more research will be done in the future to figure out alternative solutions that exist. Also, Floyd Foundation is also proposed during this period, which will serve as the entity that governs Floyd Economy.

**20/1/2020** - Research of open-source software and decentralised governance has officially started, whereby, the research focused on solving the issues highlighted in the Problem Space: General Idea section of this document.  We highlight certain technical issues that exist in all open-source projects like the sustainability issue. Moreover, we also highlight developmental challenges associated with contributors/maintainers worries in open-source software (based on /OSS/1.pdf from GitHub Research).

**21/1/2020** - The structure of the business whitepaper was formally constructed.

**23/1/2020** - The sustainability issues related to open-source software was formally defined. Then, we further extend on the concepts of DAOs and define the two entities that exist in the ecosystem, the Floyd Foundation DAO (FF DAO) and the Capital-Restrained Liberal Radicalism DAO (CLR DAO). These DAOs were proposed as a solution to the sustainability issue. We proposed to allocate a portion of the block rewards to these two DAOs to ensure that the ecosystem is self-funded. The CLR DAO would act as a self-governed DAO (requiring no interaction by the community) that funds projects based concepts related to liberal radicalism such as quadratic funding. The FF DAO, on the other hand, will act as the primarily DAO that governs the governmental and administrative decisions that occur in Floyd Economy.

**24/1/2020** - Then, we discussed potential solutions that exist when dealing with plutocracy that occurs in the governance of DAOs. We highlighted the risks and potential attacks that can occur if an adversary controls the majority of voting power in the ecosystem. Henceforth, we proposed a consensus model that solves this issue by ensuring that only highly reputable members can participate in decisions that occur in DAOs (based on the awesome work done by Jiangshan Yu, also refer to GitHub Research for more information). More research should be done in the context of Proof-of-Reputation.

**25/1/2020** - Started the discussion on organisational structure within Floyd Foundation. This organisational structure will govern all future operations occur in the micro-level for Floyd Economy. We explore various business structures such as sole proprietorship, limited liability company, limited partnership and public shareholding company. Also, since we have solved the sustainability issue related to open-source software by utilising concepts extending from liberal radicalism, we have decided to explore use-case (such as the music and art industry) that this can inherently solve. Also, created a document for memes. Deal with it!

**28/1/2020** - Formally defined the Liberal Radicalism concepts and it’s importance in this project, especially in encouraging community collaboration. Then, opened up a discussion on taxation/subsidy in the platform to solve “economic disparity” (this idea was brought up due to the amazing work done by Andrew Kortina, refer here). With that, we also started to explore the “Universal Dividend” theory.

**29/1/2020** - Opened up a discussion on Ethereum’s Research Portal (refer here) on Quadratic Delegated Proof Of Stake to explore benefits and drawbacks of Quadratic based consensus algorithms. Then, the application of the Universal Dividend was formally defined. This definition was based on the two key stakeholders, the Liberal Miner and the Adversarial Miner. The Liberal Miner is a subset of the consensus participants that act as a philanthropist in the system, where, they autonomous donate a significant portion of their block rewards directly into the CLR DAO. Henceforth, if reputation-based consensus is deployed, the reputation should be a function of % of the block reward donated philanthropically.

**30/1/2020** - Circuit tokens and the use of exponential decay to issue out block rewards to DAOs was explored (refer to the amazing work done by Panvala and niran).  Then, we formally defined the Exponential Decay of Block Rewards, first by introducing the mechanism used by Bitcoin, then by Panvala.

**2/2/2020** - Started exploring various types of use-cases that this sustainability platform can be applied to. Also, opened up a discussion on the governing council of Floyd Economy.

**11/2/2020** - Exploring options for an MVE to achieve philanthropism through the Ethereum and Vechain blockchain. This MVE will be purely for philanthropic donation platforms to start exploring the viability of having Philanthropic Miners in a blockchain system.

**16/2/2020** - Further exploration of consensus mechanism has been outlined in the MVE section. We noticed that if we only use Philanthropic Miners (or Nodes), there wouldn’t be a need for consensus participants to fight/collude/bribe for block rewards as all rewards go directly to the organisations that exists in the ecosystem. Henceforth, it would be even easier to employ a BFT-based consensus agreement.

**17/2/2020** - Decided to start exploring smart contracts as an option for creating DAOs. Before this, it was decided to write the DAO contract directly using Golang.

**20/2/2020** - While listing down the Assumptions and Constraints, we noticed that there was a severe issue related to Public Bad. Therefore, we decided to explore solutions to remove Public Bads from the system through some sort of Curation Market. Also, we started to explore ways to utilize existing technologies such as Aragon (DAO platform) and integrate it directly into this project.


**22/2/2020** - The solution was completely refactored to now ensure that Floyd Economy exists as a platform that integrates existing public good platforms such as Gitcoin and Panvala by providing the necessary infrastructure required to bootstrap these solutions together. Moreover, this platform will also be able to handle future PG Platforms and allow them to join the system through smart contracts.
