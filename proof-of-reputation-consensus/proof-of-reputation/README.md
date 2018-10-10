# Proof of Reputation

We herein explain the PoS blockchain consensus protocol which uses the Semada reputation verification platform to ensure block production is honest, economically viable, scalable, and secure. We call this protocol Semada’s Proof of Reputation \(PoR\) to distinguish it from the several previous PoS protocols.

Since PoR relies on the user reputation created by the Semada platform, before readers can understand and trust the PoR protocol, readers must understand and trust that the Semada platform is secure against the host of problems that have plagued all previous attempts to create meaningful reputation for potentially pseudonymous users, including powerful centralized commercial platforms such as Ebay and Amazon which rely on buyer and seller reputation. Though we review the generalities here, a prerequisite to understanding PoR is to read and understand the Semada technical white paper explaining its architecture.

Given a secure reputational system, the stakes in PoR are given by the reputation tokens \(called sem tokens​\), then the protocols follow naturally. Other PoS protocols regularly use ad hoc solutions to solve problems as they are identified, such as the long range attack, cartel formation, and censorship resistance. These problems are automatically handled in a self-policing reputational system.

Therefore the PoR architecture has several advantageous features over the other PoS protocols. First, PoR is more secure because it has a different reward structure, which ensures the motivations of users is to maintain protocols that attract the maximum use and to honestly produce blocks following those protocols. In particular, the stakes \(sem tokens\) are naturally far less fungible than cryptocurrency stakes, so long-term probity is incentivized, eliminating many short-term arbitrage opportunities. The reward structure involves the following:

1. All fees gained by block creation are shared with the entire group according to a reputation-weighted salary. Therefore, unlike every other implemented platform, there is no direct monetary reward incentive for creating mining pools or block production cartels, which are a threat to decentralization which increases the likelihood of 51% attacks. These reputation-weighted salaries encourage actions that benefit the platform long term and guard against short term arbitrage opportunities which harm the reputation of the blockchain. 
2. All positive contributions to the platform are directly rewarded with sem tokens, not currency. All negative actions \(determined by votes from the community\) are punished with loss of sem tokens \(slashing\). Policing is swift and effective through reputation staked bets in the validation pool. Since the value of a sem token derives from the regular reputation-weighted salary, which is split amongst all users, long-term platform improvement is incentivized. Sem tokens are less fungible than the currency received in salary, which prevents short term arbitrage attacks.
3. Anyone can gain new sem tokens at any time and join in the process of block creation and share the rewards, which encourages maximum decentralization. The opportunity to purchase sem tokens may appear to open the platform to an obvious 51% attack. However, whenever someone sends a fee to the platform to gain sem tokens, at least half of the tokens minted are shared with the community who polices the application. We provide a mathematical proof that shows this alone completely eliminates all incentives to perform the 51% attack. Further, other protocols are naturally incorporated that safeguard this threat, such as requiring new nodes to prove their worth in various ways.
4. Users who produce valid blocks and who are knowledgeable enough to decide on protocol improvements will enjoy substantially greater rewards. Users who don’t will be punished with loss of sem tokens. Inactive users \(liveness faults\) are indirectly punished with the natural inflation of the token, which happens because new tokens are minted whenever the platform attracts a fee. Therefore, the system will naturally and stably tend toward probity.
5. The Semada forum holds evidence of positive contributions to the blockchain, including evidence of proper block production, policing block production, protocol suggestions, and discussion. Every post is subjected to a validation pool where all sem token holders have the opportunity to stake their tokens to decide the value of a contribution. The staking of tokens, with its potential for slashing, is necessary to avoid the tragedy of the commons. A reference system allows new validated posts to alter the value of sem tokens minted from older posts. This opportunity for review adds stability against slashing, giving users the ability to police long-term systemic attacks, the ability to reverse previous decisions, and the ability to reward long-term improvements such as protocol upgrades.

Secondly, PoR is evolutionary in nature. It’s architecture naturally incorporates a mechanism for 1\) proposing, deciding, and rewarding authors of protocol improvements, and 2\) policing any gaming during block production. The forum holds a history of all protocol improvement suggestions, the validation pool specifies the consensus of the community on each issue, and the reference system allows retroactive rewarding of proposers and testers who contributed to the security and success of the blockchain.

The primary concern in PoR is achieving consensus on block finality, while maintaining liveness, decentralization, autonomy, anonymity, efficiency, and especially security--which includes Byzantine faults, 51% attacks, stake grinding, the nothing-at-stake problem \(tragedy of the commons\), Sybil attacks, tyranny of the majority, liveness faults, DoS attacks, perverse delegates, censorship, and soft protocol changes.

## Generalities

PoR uses the Semada platform to vest users who contribute to the success of the blockchain with sem tokens. All sem token holders share all fees the blockchain attracts \(typically transaction fees\). Contributing to the success of the blockchain includes following the protocols developed in the forum for block production and policing, and suggesting protocol improvements. Block production and policing will generally consist of running a full node with the currently approved algorithm from the forum.

This general approach has the following consequences:

1. Protocols for block creation are automated and openly viewable on the blockchain.
2. Semada allows automated analysis of blocks, with both immediate policing through the validation pool and long-term policing via the referencing system of the WDAG.
3. The evolutionary environment of continual posts in the forum judged in the validation pool encourages stable consensus on continual protocol improvements, which ensures security.
4. The WDAG incentivizes protocol improvements since it allows retroactive rewards through references.
5. Many types of blockchains can be created with this protocol. Depending on the goals for the blockchain \(cryptocurrency blockchains, smart contract blockchains, IoT blockchains, etc.\), different fee structures will be appropriate.

## Evolution Implications 

The PoR protocol will continually evolve in the forum. Therefore anything we claim now is provisional, since the platform is completely autonomous and the authors will have no control over its evolution. We can only specify here how the protocol will begin.

PoR has elements of DPoS and chain-based PoS, as time slots are regular, and block producers are chosen randomly based on stake holdings. PoR also has BFT20-style PoS elements since all blocks are evaluated through Semada’s validation pool.

As we explain the protocol below, keep in mind that all steps are automated and performed by computers, except \(perhaps\) the protocol proposals which are posted in the forum.

