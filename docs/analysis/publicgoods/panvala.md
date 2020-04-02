## Economic Model of Panvala

Panvala grants are awarded to teams who work to fulfil the Ethereum vision with infrastructure and applications that the whole ecosystem depends on.

Grants are issued using the PAN token, so they can be issued from the first day of the system. The intended buyers of the granted tokens are donors who want to fund these ecosystem development projects.

Restrictions of Grant Issuance:
1. The token has a fixed supply of 100 million tokens.
2. The rate that donated tokens can be released is limited by the token capacitor.
3. The token holders must govern the issuance of grants using the system’s slate governance model.

While Panvala’s grants are issued to individual teams, **donations are made to the system as a whole**, not to individual project

The **token capacitor** is the smart contract that releases tokens for grants and accepts tokens as donations. The tokens in the capacitor are released at a rate that decays exponentially over time.

The **slate governance**, ensure that each quarter, the system approves one slate of actions and all of the individual proposals it contains. Pan holders who don’t believe that a slate represents the consensus of the community can propose a competing slate of proposals. Pan must be staked on each proposed slate in order for that slate to appear on the ballot, and the tokens staked on losing slates are donated to the token capacitor.

Panvala avoids fork-based governance with the goal of building a committed community that cooperates even when they don’t get their way

Each period of governance is called an epoch, and lasts thirteen weeks. Epoch zero started on November 2, 2018 at 1700 UTC and ended with the issuance of Batch One of grants on February 1, 2019.

## Issues related to Panvala Economic Model

1. Panvala’s token depreciates every time there is a new grant cycle as all the projects receive funds the same time. Then, these projects sell their tokens meaning that there is an influx of supply and the price drops as a result.
2. Liveness is only guaranteed if the equilibrium point is reached in each epoch.
3. Economic Model does not take into account the inflation rate (which is based on exponential decay of token issuance).
  - Essentially, this is a negatively correlated inflation factor that effects price.
