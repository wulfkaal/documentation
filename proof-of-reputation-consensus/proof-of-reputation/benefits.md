# Benefits

Semada’s solutions for consensus protocols fall into 5 general categories: decentralization, efficiency, autonomy, anonymity, and most importantly, security.

**1. Decentralization.** PoR inhibits the centralization problem which arises in all previous blockchains, whether they use bitcoin’s PoW or a flavor of PoS such as BitShare’s DPoS or Ethereum’s Casper. In each of these cases, mining pools or block production cartels arise because lotteries, or voting delegations, or economy of scale give outsized rewards to powerful groups.

Under most any PoS system, the economy of scale advantage is mitigated because doubling your computing power does not double your power to build blocks.

PoR solves the other decentralization threats, since there is only ever the incentive to be part of one block production cartel, the Semada platform itself, because all fees are distributed fairly in a salary according to each user’s sem holdings.

Further decentralization is achieved under PoR because it is easy for anyone to become a block producer and validator. This naturally encourages the widest possible distribution of stakeholding. So PoR doesn’t suffer from the tragedy of the commons problems other mining protocols engender for 3 reasons. 1\) Stakeholders are empowered to participate, since every one of them gains more sem tokens by running the validation programs most recently upvoted in the forum to police block creation. 2\) Stakeholders are motivated to improve the collective value of sem so that their salary is increased, which only happens when more fees are attracted, which happens when the platform is improved. 3\) Rent-seeking stakeholders who do not participate in the validation process will generally suffer from the inflationary nature of the token.

Finally the nature of the platform is decentralized in the sense that if all but one of the nodes goes offline unexpectedly, the blockchain will continue and can regenerate from the one node38. This is because the protocol chooses future producers from the existing availability smart contracts; and when a producer doesn’t submit a block, future producers are still chosen.

**2. Autonomy.** The Semada platform on a PoR blockchain achieves perfect autonomy. The bench, the forum and the validation pool run off the Semada smart contract which runs entirely on the gas of whatever blockchain it is posted to.

Consensus is established in the forum, which is simply a collection of linked posts to the blockchain. Consensus on every suggested protocol upgrade, including program upgrades to the Semada DApp itself, is determined entirely by the bench, after debate in the forum, when validation pools conclude. There is no need for any outside centralized foundation to organize protocol forks, such as deciding how and when to scale or shard to handle more transactions, or what the standards are for block creation and policing. All protocol upgrades are therefore handled swiftly, decisively, and openly, with minimal disruption, through the weighted democracy of sem-staked decision making.

The incentive for developers to propose improved protocols on chain comes from the potential for reward given by the reference system in the forum WDAG. This allows future posts to reference development posts which initially attracted no fees, in order to share their fees as a matter of protocol.

This also solves the debate over how to slash. There are, of course, infinitely many possible protocols for determining when and how an expert producer should be punished for producing a corrupt block, whether fighting against double spending/forking, or censorship, or other attacks. Whatever protocol is adopted will witness hacking/gaming attempts. The forum and validation pool will provide the evolutionary ecosystem for continually improving slashing protocols.

**3. Efficiency.** Compared with PoW implementations, such as bitcoin and Ethereum, PoR is far more computationally efficient. Nodes will no longer hash mine. They will check the validity of the blocks, but they do that under any blockchain. The only added computation is the validation pool which happens once for each block, where nodes send one transaction, an up- or downvote.

**4. Anonymity.** Reputation is determined by actions validated on the platform, independent of any other establishment of identity. The most common actions are faithfully running

the programs established in the forum to validate and produce blocks according to protocol.

**5. Security.** Probity is assured via the positive feedback loop with properly aligned incentives.

1. **Fees** from public users are shared with all experts through the reputation-weighted salary, so expert users are motivated to produce maximally useful blocks and to police other experts’ block production, in order for the system to attract more fees from public users.
2. **Finality** for a block \(the state where a block is confidently considered to be a permanent part of the chain\) is measurable under PoR.

   First, a measurable number of expert validators risked their sem tokens on the bet that the block was valid.

   Secondly, the sem that members gain from policing block production is equal to half of all fees sent since the production of the block. In order to fork a chain from that particular block, the community will lose all sem tokens created subsequently on the chain to be forked.

   Further, since the value of the sem tokens is in the promise of future fees, all token holders are motivated to maintain the long-term stability of the chain, and less motivated by arbitrage opportunities from malicious forks or censorship.

3. **Slashing** is a natural part of PoR through the loss of availability stakes, a strong disincentive for any violation of the hard protocols validated in the forum. This solves the nothing-at-stake problem \(or tragedy of the commons problem\) associated with previous chain-based PoS protocols.

   The possibility of review through references in the forum to change the value of sem tokens allows slashing to address more subtle, long-term patterns of “spirit of the law” soft protocol violations.

4. **Liveness faults**. When users don’t participate in block creation or validation they are naturally punished by a devaluation of their sem token holdings from the natural inflation of the token which occurs during token creation. This punishment is ​**stable** in the sense that it does not dramatically and unfairly punish honest users who lose connectivity, so honest users do not lose security for their investment as nodes.
5. **Blacklists​.** Besides the slashing of availability stakes, producers and validators who demonstrate subtle, long-term patterns of protocol violation, such as censorship of transactions, may be added to blacklists developed in the forum. Then any new block produced by a token holder from the blacklist would be invalidated by majority vote. The openness of the blockchain allows analysis of past blocks in order to write these blacklists, and the validation pool ensures accuracy and fairness in their creation. Blacklisted users will not lose their tokens, which adds stability to the system, giving token holders confidence the system is not arbitrary and fickle. Blacklisted users will have the ability to argue their case in the forum using their tokens while they remain. While they are blacklisted, however, they will not be able to gain sem by producing any further successful blocks. Due to the natural inflation of the sem tokens, the blacklisted producers stakes will inevitably diminish in value as further blocks are produced.
6. **51% attacks** are inhibited in a measurable manner through the mechanisms, and because the feedback loop is closed and complete. 

   In the various 51% attacks a group that owns a significant percentage of the governing tokens can profit at the expense of the platform and the other users by exerting their power. The 51% attack is particularly dangerous in decentralized systems with potentially anonymous users because there is usually no recourse to dispute resolution. Therefore if there is the opportunity to maliciously profit, someone in the world will certainly take advantage.

   One type of 51% attack is the arbitrage scenario where a group will buy up 51% of the tokens, make a short term profit at the expense of other users \(double spending, editing, or censoring, e.g.\) then quickly sell off the tokens before their value declines from the damage done.

   Almost all other blockchain platforms sell off a significant number of their tokens in an initial token sale, or mine them, or a combination of both. Either way, these tokens are almost always perfectly fungible currencies.

   Semada’s tokens are different than most every other platform’s tokens. They can theoretically be bought and sold by buying the anonymous user’s account. So sem tokens are valuable, but not perfectly fungible for 3 reasons.

   1. Sem tokens do not hold their value as well as other currencies, naturally experiencing significant deflation. This is because more sem tokens are added to the system every time a fee is sent to the platform, so their relative value in earning the reputation-weighted salary constantly diminishes.  Therefore, if they are not being used constantly to improve the platform \(and thereby gain more sem tokens\), they punish the users for holding them by losing relative value. This gives strong incentive for maintaining nodes and actively policing the system.
   2. Sem tokens are not equally valuable to all people. People with the proper skills and knowledge in the expertise will naturally win more validation pools than others, thereby gaining more sem tokens, and ultimately more perfectly fungible currency through the reputation-weighted salary.
   3. The value of a sem token derives from its position in the reference system in the WDAG. So each token is subject to a variable, relative value which may change in time.

Therefore it is more difficult to attack Semada than other platforms by buying 51% of the sem tokens because 1\) most of the tokens should be constantly in use, 2\) more are being created all the time, 3\) holding them for a long period of time without improving the platform \(and earning more sem\) is costly due to the natural inflation of the token, and 4\) their value is difficult to determine since each token has a different value depending on the post in which it was minted. So it is almost impossible to execute a 51% attack by purchasing tokens on an exchange.

Another attack vector is to buy the tokens directly from Semada, by sending fees to the platform. However, in this case even if the attack were successful, the attacker would lose a significant amount of money to achieve their goal, at least twice the entire historical value of the platform--more likely the factor would be 6 times the total value. So the griefing factor is a minimum of 2 with an average of 6, and has no effect unless the platform is destroyed. Further, whether or not the platform is destroyed, all the fees would go entirely to the users who built the platform, who would profit significantly during the attack, even if successful.

If such an attack were identified, users could stop it by policing the creation of new PoR sem tokens, preventing any new users from gaining tokens. In this case, those tokens bought by the attacker would eventually lose value through natural inflation, and the attack would completely fail, while rewarding the users who honestly policed the attack.

Finally, the extremely decentralized nature described in 1\) above, makes it more difficult to achieve consensus between colluding whales in Semada than in other platforms, because power is naturally distributed more sparsely.

**7. The long-range attack** ​is a common problem with PoS protocols, where a malicious producer may create a long list of blocks forked from an earlier valid block, because there is no PoW energetic outlay required to prevent this41. Essentially, a new node can join the network and see the genuine chain and a fabricated chain that is longer; then the new node, lacking the proof of work hashes, could not objectively distinguish which is correct. Casper and Tendermint solve this problem with a system of token locking.

PoR naturally prevents this attack without such locking, since a false chain cannot be manufactured with more total validation than the real chain. Validators’ public keys are used to vote \(each vote is a transaction moving their sem tokens\), so votes cannot be forged from existing sem tokens. Therefore, not even a single fake block can be produced which has a stronger number of upvotes in order to fabricate a stronger fork. In this sense PoR uses the validation pool to create proof-of-strong-collaboration in place of bitcoin’s hash-mining proof-of-work to allow distributed verification of block validity.

**8. Perverse delegates.** In any PoS protocol, especially DPoS, the motives of the producers are more likely to be avaricious than average, because those with perverse motives are more likely to make the effort to produce blocks and risk slashing. The ability to achieve clear consensus on validation protocols in the forum makes it easy to police adverse actions without the need for any extra incentive besides preserving the value of your sem token holdings.

**9. Sybil attacks** are prevented with weighted voting, because all actions on the platform are fairly evaluated as determined by holdings of openly verified reputation; thus power is not increased by distributing it amongst cloned accounts

**10. Tyranny of the majority** is inhibited since all actions are reviewed by users weighted by reputation \(sem\), so direct democracy does not dilute expertise.

**11. Stake grinding attack.** In any decentralized PoS protocol there needs to be an automated mechanism for determining when and who produces a block. Generally it is a given that in a decentralized system, the selection should be random, weighted according to the producers’ stakeholdings. The randomness must be achieved with a pseudo-random number generator whose algorithm and seed must be available for verification by all nodes. If the protocol is not carefully chosen, this introduces an attack vector, called stake grinding, in which malicious producers might manipulate the seed in order to influence the selection in their favor.

As discussed above, in PoR the seed used is a hash of the joined alphabetized symmetric keys that were submitted by all validators during the vote revealing process. This protocol completely prevents stake grinding even if only one validator is not colluding.

**12. Censorship** ​can be good or bad for the platform. Good censorship includes preventing transactions which destroy the larger reputation of the platform, such as selling child pornography or chemical weapons. Bad censorship is more subtle, such as preventing competing organizations from registering transactions. Both types of censorship are naturally dealt with in the forum. Further, strong minority opinions at odds with the majority of validators have the freedom and power to create an alternate chain with different protocols within a new expertise under Semada.

**13. The P + ε attack** is no more effective than the 51% attack, because typical validators will be staking all their available sem tokens in each validation pool.

**14. Blockchain clones.** We cannot prevent a malicious party from using Sybil accounts to copy the general structure of a successful PoS blockchain. They would need to create new public keys, but the cost would still be much \(much\) lower than it would to copy a PoW blockchain’s structure. Then, when a new user joins the network, how will they be able to distinguish a truly decentralized blockchain from a cloned blockchain that has manufactured an even larger number of tokens?

The answer is, the same way a new internet user knows not to visit cloned web pages. Their UI is a trusted internet browser which steers them to a trusted search engine, which has ranked web pages throughout their history to distinguish their value. A trusted UI for interacting with blockchains has the same role.

**15. Soft protocol changes.** There will alway be changes in market forces, network performance, computing technology, cryptographic standards, social values, and the goals of any particular blockchain. Therefore there will always be the need to change block production and validation protocols. Therefore, in addition to the fundamental fact that no protocol is perfectly secure, there will always be the threat that the nodes will accept a deeply flawed protocol that can destroy a blockchain. If the protocol does not involve a decentralized medium for cheap and available communication that is eternally open to review, then the risks from centralization compound the danger.

The means by which all current major blockchains achieve their soft forks is through private communication between famous token-holding whales and developers. This results in a state of governance which is completely counter to the blockchain design goals of decentralization, anonymity, and autonomy. Any blockchain subject to such governance is ultimately less secure than legacy centralized systems which pointedly address centralized security risks.

Since soft protocol changes are a perpetual risk, proper incentivization for protocol upgrades is crucial. The forum is the needed decentralized medium for cheap and available communication that is eternally open to review. The reference process of the forum WDAG rewards long-term protocol upgrades.

