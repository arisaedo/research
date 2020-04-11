## Discussion

### Decentralised Governance
 * How do coordinating institutions affect plutocracy?
 * How will the funding mechanism react if everyone stops voting?
 * Is this an issue about Liveness then?
 * Issues related to colluding
    * Can the community bribe other members to act in their favour?
      * A bribe is when members bribe each other to vote for them
    * Will the governance system be safe against plutocracy?
      * Plutocracy is when large cartels collude for their benefit
 * How do we solve voting issues such as low voter participation rate?
    * Maybe, we can instead use some sort of relative reputation-based quantification for calculating the voter participation rate
    * How is this affected by wealth distribution?
 * Discuss on-chain governance, off-chain governance and how they affect key stakeholders.
    * for some context, tightly coupled voting and loosely coupled voting are competitors in the governance mechanism space, so it's worth dissecting: what are the advantages and disadvantages of each one? Assuming zero transaction costs, and if used as a sole governance mechanism, the two are clearly equivalent. If a loosely coupled vote says that change X should be implemented, then that will serve as a "green flag" encouraging everyone to download the update; if a minority wants to rebel, they will simply not download the update. If a tightly coupled vote implements change X, then the change happens automatically, and if a minority wants to rebel they can install a hard fork update that cancels the change. However, there clearly are nonzero transaction costs associated with making a hard fork, and this leads to some very important differences.
 * Should votes be based on the function of stake + reputation?
 * Dichotomous based Party system (i.e two-party system in American, Australia, Malta, etc) as opposed to “the double ballot majority system and proportional representation” that forms multipartism
  * Duverger's Law forms the basis of our understanding of how two-party systems work
 * “the paramount importance of civilization in human history rests with its role in promoting cooperation”

### Decentralised Autonomous Organisations
  * Are “contributors” also regarded as DAOs? By that, can contributors donate to other contributors?
  * How should we be modelling the funds? Can external parties directly request funds from the DAO?

### Floyd Economy
  * Is there a consensus model? If yes, what is the consensus model of Floyd Economy?
  * Coin Holder or User? A user that is a coin holder? Where is the line between all of them?
  * **IMPORTANT**: Can we extend the architecture to work with different use-cases like the music and art industry? Explore methods to allow other DAO’s to implement a utilitarian optimal DAO solution.
  * **IMPORTANT**: Can we let 100% of the block rewards to be allocated to the DAOs based on CLR?
    * Does that mean that the system becomes dPoS then?
    * Discuss plutocracy issues that arise with these settings
  * **IMPORTANT**: What happens if there is “tax” in the system?
    * Can we tax wealthy stakers to ensure proper distribution of wealth?
      * Power Tax
      * Wealth Tax
    * What about Universal Dividends?
      * sharing the block rewards and fees with all contributors.
      * a power tax on organisations which are rich and reputable
    * What about “tax/subsidy incidence” for developers?
  * Can participants advertise their content on the application?
    * “more power you exert by trading wealth for attention, the more you simultaneously redistribute wealth. The right to free speech is essential to the functioning of a healthy democracy so that citizens can critique the inequities and failures of the existing regime and laws, but the ability to trade money for attention presents a real threat to democracy, particularly under conditions of extreme (and increasing) economic disparity” - Andrew Kortina
    * charge fees based on quadratic concepts
  * Should there be a mechanism in place to retrieve funds from “fake projects”?
    * e.g. Dispute Resolution, Locking funds, etc

### Floyd Foundation
 * What is the organisational structure of Floyd Foundation?
  * How does this relate to the administrative and governmental decisions that occur in Floyd Foundation?
 * Can we allow FF DAO to instead become the Government in the system?
  * Should only Philanthropic Miners be able to participate in the Government decisions?
 * What kind of governance decisions can the community partake in?
  * Taxation
  * Universal Income Proposal

## Important Caveats

1. Money that flows through the platforms comes in several ways
  *  Block Rewards and Fees
  * People contributing their funds (e.g fiat, other cryptos) to projects
2. Hence, should there be a form of Taxation to stabilise the “economic disparity”?
  * Reformation of Capitalism
3. **IMPORTANT**: Instead of creating an ecosystem of DAOs, maybe the platform should just be used to solve sustainability in public goods without the need for participation in governmental and administrative decisions
  * This will ensure that the community does not need to participate in every decision that happens in every DAO
  * Simplifies solution by a large margin as we do not need to think about administrative and governmental decisions and how reputation/stake affects those factors
4. **IMPORTANT**: Should there exist a dispute resolution protocol to ensure that we can distinguish public good from public bad.
5. What if we utilise an EVM-based blockchain like Ethereum/Vechain for this system?
  * Not agnostic enough
6. What risks might ensue as a result of getting it wrong?
7. **IMPORTANT**: Well,  now that we have defined most of the business activities and caveats in the application, the technical solution may need some change considering that there already are existing Platforms that allow for Public Good Funding (Gitcoin and Panvala)
  * Will there be an increase of platforms such as Panvala that contribute funds for the sustainability of public good projects?
  * Initially, can we architect the infrastructure required for Panvala and Gitcoin to fund public good projects in a more effective and formatted manner?
    * Then, can we extend this solution that if other projects join the system, they are able to join the central pool of funds?
  * Can we create a central hub for projects to create various grants on different platforms such as Panvala, Gitcoin, etc.

## Future Works
This section provides some context on the areas to research before making any decisions in this ecosystem.

* Micro-level Organisation Structure of Floyd Foundation DAO
  * Link: ​Organisational Structure
* Macro-level DAO Structure of Floyd Economy
* Explore different use-cases that can benefit from the sustainability solution
* Explore reputation as a solution to the plutocracy and bribes that exist in decentralised governance
  * Open to solutions other than reputation as well
* Explore other methods of solving the sustainability solution through economic incentives
  * pure % block reward
  * CLR-based % block reward (QV)
  * what else?
* Explore Quadratic Voting Mechanisms in regards to governmental decisions that occur in a DAO
* Explore ideas whereby FF DAO is not a DAO but everything else can be DAOs.
  * People
  * Organisations
  * Donation platform
  * Open-source projects
* Achieving Sustain through Utilitarian optimal Philanthropic Consensus
* Advantages and Disadvantages of Liberal Miners
* Competitor Analysis of various sustainability solutions and DAOsS
