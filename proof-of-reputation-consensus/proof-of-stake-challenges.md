# Proof of Stake Challenges

In this section we review the major challenges to any PoS protocol, in order to explain how the Semada's Proof of Reputation \(PoR\) addresses each of them. Valuable resources for a more exhaustive introduction which are still aimed at a general technical audience is the Ethereum foundation’s PoS summary and the Bitcoin Wiki page. Readers familiar with PoS research may wish to skip to [later sections](https://semada.gitbook.io/project/~/edit/drafts/-LOQxTFv4ip2yb2oALUv/proof-of-reputation-consensus/proof-of-reputation) where the Semada platform and the PoR protocols are detailed.

## Hard theoretical limits

To begin, there are three basic theoretical boundaries from computer science to consider when choosing block production protocols:

1\) The ​33% BFT threshold: ​If more than 1⁄3 of participants are maliciously colluding, honest users cannot immediately establish consensus with certainty.

2\) The FLP impossibility theorem: It is impossible to simultaneously achieve complete availability9 and security in an asynchronous network.

3\) The ​CAP theorem: ​It is impossible for a distributed data store to simultaneously guarantee complete consistency, availability, and partition tolerance.

Given the inevitable possibility of Byzantine faults in a distributed system, such results require any protocol to hedge, promising only a probability of finality and security inversely proportional to liveness and speed.

The PoR protocol, recognizing the changing realities of history and society, doesn’t permanently choose which qualities are most important to stress. PoR gives users the freedom and power to choose which quality is important to safeguard, depending on the changing environment, as the blockchain progresses and contemporary threats are identified.

The initial PoR protocols stress security and honest block production. Once stability is achieved with a large enough user base which has proven itself honest by earning valuable reputation with positive contributions, more availability can be achieved with more confidence--this is the bootstrapping problem relevant to any distributed system. Then long-term stability in the honesty of the system is maintained by slashing from the validation pool.

One final theoretical obstacle is the general impossibility of creating a fixed protocol which will always reflect the will of its creators. Arrow’s Impossibility Theorem from social choice theory is the simplest expression of this limitation.

## Soft Attacks

Beyond the above theoretical limits, there are several attacks and degeneracy dangers to keep in mind when choosing block production protocols that we detail below: 1\) centralization, 2\) lack of anonymity/DoS attacks, 3\) valuable transactions, 4\) the nothing-at-stake problem \(tragedy of the commons\), 5\) “Spirit of the law” soft protocol violations, 6\) liveness faults, 7\) 51% attacks, 8\) long range attacks, 9\) perverse delegates, 10\) Sybil attacks, 11\) tyranny of the majority, 12\) stake grinding, 12\) censorship, 13\) the P + ε attack, 14\) soft protocol changes, and 15\) the altruism cliff.

**1\) Centralization** is an existential threat to distributed systems. This threat arises in all previous blockchains. Under bitcoin’s PoW, centralization occurs mainly due to economy of scale issues. ​E.g., building an ASIC farm of 1000 CPUs is far cheaper than 1000 people buying 1 CPU each. The second problem with PoW happens when lotteries do not have time to thoroughly sample the users. Even if the the algorithm is fair, a user with a tiny fraction of the computing power of the system is running the risk of never winning a hash race, so they can gain financial security by joining a mining pool.

Under most any PoS system, the economy of scale advantage is mitigated because doubling your computing power does not double your power to build blocks. However, block production cartels may still arise due to lotteries, or the fact that voting delegations are built into the system, or the fact that the stakes needed to be a block producer may be bought, so there is an incentive to control the blockchain.

Another type of centralization is common in PoS systems. If the blockchain goes offline for a long period, or if too few nodes are active, can the blockchain restart or regenerate autonomously12? Or is there a need for social coordination between the nodes? If so, anonymity is threatened and famous nodes are required.

Similarly, a final type of centralization occurs if the blockchain lacks on-chain autonomy. The question is, how is node consensus achieved for protocol upgrades/forks such as deciding how and when to scale or shard to handle more transactions, or how to improve standards for block creation and policing? Again, if famous people or powerful consortia are needed to lead development and drive the debate, decentralization is not truly achieved, and this leads to the security risks blockchains were supposed to mitigate compared with centralized organizations.

**2\) Lack of Anonymity/DoS attacks.** A second existential threat to a PoS blockchain is the danger that block producers will need to use their identity in order to convince nodes to choose them to produce a block. This is particularly evident in DPoS, where delegates must win popularity contests to become producers. If block producers’ identities are revealed, the supranational independence of the blockchain is threatened as is its security. In this case local jurisdictions could exert legal power over block production, which will weaken confidence in its fairness.

Secondly, DoS attacks can be performed on stable block producers \(especially delegates\) whose identities or locations are revealed.

**3\)  Valuable transactions.** ​No protocol can guard against Byzantine faults if a transaction is more valuable than the promise of all future fees for the entire platform; in this case a party could bribe the entire set of nodes \(or 51%\) to destroy their own blockchain’s integrity. Therefore an obvious assumption is that the sum of all fees should not be smaller than the value of any individual transaction. The idea is that there are a great number of global transactions, so only a tiny fraction of the value of each transaction is required to maintain security. Fees are crucial at some point, since we cannot rely on altruism in a decentralized, anonymous system in our selfish world. Therefore it seems necessary for there to exist several blockchains with different fee structures to guarantee different security for different values of transactions.

**4\)  The nothing at stake problem.** More generally, the ​tragedy of the commons happens when a protocol does not properly reward positive contributions or punish damaging behaviors \(slashing13\).

**5\)  “Spirit of the law” soft protocol violations**. Any protocol can be gamed to benefit a minority group at the expense of the whole \(cf. Arrow’s Impossibility Theorem\).

**6\)  Liveness faults.** When some users don’t participate in block creation or validation, then security is weakened and decentralization is threatened.

**7\)  51% attacks.** In the various 51% attacks, a group that owns a significant percentage of the governing tokens can profit at the expense of the platform and the other users by exerting their power. The 51% attack is particularly dangerous in decentralized systems with potentially anonymous users and automated protocols because there is usually no recourse to petition a centralized authority with the power to effectuate dispute resolution. Therefore if there is an arbitrage opportunity due to any weakness in the system, someone in the world will certainly exploit it eventually.

One type of 51% attack is the arbitrage scenario where a group will buy 51% of the tokens, make a short term profit at the expense of other users \(double spending, editing, or censoring, e.g.\) then quickly sell off the tokens before the platform’s value declines from the damage done.

Almost all other blockchains sell off a significant number of their tokens in an initial token sale, or mine them, or a combination of both. Either way, these tokens are almost always perfectly fungible currencies, so there is a clear answer to how much it would costto corrupt or destroy blockchain running a PoS protocol based on cryptocurrency stakes.

**8\) The long-range attack** ​is a fundamental problem PoS protocols must address, where a malicious producer may create a long list of blocks forked from an earlier valid block, because there is no PoW energetic outlay required to prevent this. Essentially, a new node can join the network and see the genuine chain and a fabricated chain that is longer; then the new node, lacking the proof of work hashes, could not objectively distinguish which is correct. Casper and Tendermint solve this problem with a system of token locking.

**9\) Perverse delegates.** In any PoS, especially DPoS, the motives of the producers are more likely to be avaricious than average, because those with perverse motives are more likely to make the effort to produce blocks and risk slashing. The ability to achieve clear consensus on validation protocols in the forum makes it easy to police adverse actions without the need for any extra incentive besides preserving the value of your sem token holdings.

**10\) Sybil attacks** are prevented with weighted voting, because all actions on the platform are fairly evaluated as determined by holdings of openly verified reputation; thus power is not increased by distributing it amongst cloned accounts.

**11\) Tyranny of the majority** is inhibited since all actions are reviewed by users weighted by sem tokens, so direct democracy does not dilute expertise.

**12\) Stake grinding.** In any decentralized PoS protocol there needs to be an automated mechanism for determining when and who produces a block. Generally it is a given that in a decentralized system, the selection should be random, weighted according to the producers’ stakeholdings. The randomness must be achieved with a pseudo-random number generator whose algorithm and seed must be available for verification by all nodes. If the protocol is not carefully chosen, this introduces an attack vector, called stake grinding, in which malicious producers might manipulate the seed in order to influence the selection in their favor.

**13\) Censorship.** ​A block producer may choose to violate protocol and run an edited block production program which picks and chooses which transactions to include in their blocks. Such censorship would open the possibility of personally profiting at the expense of the integrity of the system. In a distributed system--which cannot achieve constant perfect communication between nodes--we can never certainly determine that a block producer was censoring certain transactions, instead of simply not being aware of them.

Censorship can be good or bad for the platform. Good censorship includes preventing transactions which destroy the larger reputation of the platform, such as selling child pornography or chemical weapons. Bad censorship is more subtle, such as preventing competing organizations from registering transactions.

**14\) The P + ε attack.** ​See \[Buterin 2015\].

**15\) Soft protocol changes**. There will alway be changes in market forces, network performance, computing technology, cryptographic standards, social values, and the goals of any particular blockchain. Therefore there will always be the need to change block production and validation protocols. Therefore, in addition to the fundamental fact that no protocol is perfectly secure, there will always be the threat that the nodes will accept a deeply flawed protocol that can destroy a blockchain. If the protocol does not involve a decentralized medium for cheap and available communication that is eternally open to review, then the risks from centralization compound the danger.

The means by which all current major blockchains achieve their soft forks is through private communication between famous token-holding whales. This results in a state of governance which is completely counter to the blockchain design goals of decentralization, anonymity, and autonomy. Any blockchain subject to such governance is ultimately less secure than legacy centralized systems which pointedly address centralized security risks.

**16\) The altruism cliff.** An important problem with PoS experiments is that the nascent space is currently dominated by altruists. In many areas of the economy it is understood that the majority of people who choose to work in the area do so for motives aside from monetary profit, such as nurses, teachers, and police. This is also generally true of any population involved in any emerging industry, since they need the larger industry to succeed in order to profit, and it is evidently true for the currently emerging crypto economy. People are investing themselves in the hope that the industry will succeed, so they tend to work for the greater good.

However, once the crypto economy is mature, we cannot assume users will continue to behave altruistically. We can anticipate, with certainty, an influx of hedgers and rent seekers who will quite naturally exploit any weakness in the system for profit.

