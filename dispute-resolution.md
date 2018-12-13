---
description: >-
  This page presents a basic conceptual framework for smart contract dispute
  resolution on the Semada Platform.
---

# Dispute Resolution

In this section, we detail an important application of the Semada platform, dispute resolution in the distributed and anonymized environment of the crypto economy. We call this application of the Semada platform **Distributed Jurisdiction \(DJ\)**. DJ illustrates how several expertise tags in the forum can work in parallel, as smart-contracting parties will typically require several skills from their arbiters, as detailed below.

Bench experts in the dispute resolution expertise tags will be called **arbiters** in this section.

To use the Distributed Jurisdiction platform, public users must choose their own smart contracting language. Therefore, the protocols of dispute resolution are entirely determined by the contract parties as stipulated by the smart contract at the point of creation.

Successful smart contract language is expected to be developed in the forum through the evolutionary process driven by the validation pool. The protocols suggested in this section are therefore entirely hypothetical.

#### Contract creation

When a smart contract is created, the means of dispute resolution is included before parties sign.

**Break clause**

A break clause in the smart contract will transfer to a 3rd party arbiter the complete power to disburse the encumbered assets of the smart contract between the parties. The break clause is triggered whensoever either party chooses to initiate a dispute.**Third-party arbiter**

Distributed Jurisdiction is designated as the platform for dispute resolution of smart contracts by including a 3rd party arbiter in the respective smart contract—an open position for a randomly selected expert from the bench whose power is triggered when a contracting party initiates a dispute. The arbiter’s power to disburse the assets of the contract between the other parties, once triggered, must be preeminent in order to ensure certainty of outcomes.

Before being selected to adjudicate any case, each arbiter posts an availability stake. This is a number of their sem tokens that will be included as the arbiter’s upvote bet on their final post justifying their eventual decision on the case.

An arbiter is randomly selected, weighted according to availability stakes posted and according to the expertise tags specified by the contract. These tags decide value assumptions for the contract. Expertise tags signal the type of dispute and indicate the experience required of potential arbiters. Examples of expertise tags include relevant areas of law \(property, employment, Delaware corporate law, etc.\), technical matters disputed, languages, territorial or cultural assumptions, and anonymity level.

**Fees**

Fees are determined by market factors at any given point in time. Fees are calculated based on the availability of relevant arbiter availability stakes. Arbiters specify the fees they will accept for each sem token staked, the availability stakes, by advertising in the forum. The Semada platform does not dictate the fees.

If the fees chosen by the contracting parties are insufficient, the arbitration will fail as the arbiter selected will refuse to do the work. If the arbiters require fees higher than the public is willing to pay, they will fail to attract cases.

The smart contract must specify that the fee is sent in the arbiter’s name to the Distributed Jurisdiction platform associated to the arbiter’s judgment post in the forum. The fee is not sent directly to the arbiter, or else the parties are not technically using the Distributed Jurisdiction platform.

The reason the parties will prefer to send fees to the platform instead of the arbiters directly is the insurance provided by the evidence-of-work post, which only rewards the arbiter if other arbiters approve of their decisions.

#### Arbiter Selection

A random arbiter is chosen based on availability, expertise, reputation, and fees. Before the choice is made, all arbiters from the pool have submitted a stake signaling their availability, and the forum has advertised protocols and fees the arbiters will accept for dispute resolution work. The arbiter’s availability stake is a number of their sem tokens, chosen from each of the expertise tags they’ve improved.

Then the system takes the weights that the contracting parties chose for each expertise tag \(summing to 100%\) and multiplies these weights by the available users' weights to determine the likelihood of each arbiter being picked. Using this distribution, the arbiter is randomly chosen from the pool of arbiters.

As an example, imagine there are 3 expertise tags in the contract, which the parties chose as 50% English speaking arbiter, 25% intellectual property law, 25% corporate law expertise. Next suppose arbiter A has 10% of the available sem tokens staked from the entire bench in English, 5% of the intellectual property, and 7% of corporate law expertises. Then \(0.5\)\(0.1\) + \(0.25\)\(0.05\) + \(0.25\)\(0.07\) = 0.08 so arbiter A has an 8% chance of being selected for the dispute by the system.

Once chosen, the arbiter has the power of disbursing the assets of the contracts as seen fit between the disputants. Asymmetry in party asset encumbrance may be abused if assets from each party are encumbered equally. However, the arbiter also has the power to combat such abuses by choosing at any point to release a portion of the property to either party before the judgment is complete, based on temporal concerns.

The arbiter’s stake also represents a bet that the community will agree with their decision. An arbiter’s stake is combined with the half the contract fee as the arbiter’s upvote bet on the post of the decision, half the fee is staked as a downvote against the bet. This encourages careful participation of arbiters in the adjudication portion of the platform.

#### Private hearing

A private hearing is initiated with the arbiter as moderator. This hearing takes place entirely off platform, following the protocols set by the smart contract. Solutions for how to perform the hearing will be decided as protocols evolve in the forum.

One possible approach for the beginning of the platform is detailed as follows. Symmetric encryption \(PGP, e.g.\) guarantees efficient, anonymous communication between the parties and arbiter using their asymmetric public-key identifiers. Then the trial proceeds as follows:

1\) Plaintiffs submit their case, including proposed settlement.

2\) Defendants submit their rebuttal, including proposed settlement.

3\) Arbiters ask open questions until deciding to close the question session.

4\) Arbiters repeat 1\)-3\) until choosing to close the trial.

Standard procedure small asset contracts may have an arbiter ask no questions and deliver a verdict after step 2 by quickly explaining the relevant precedent. Standard procedure for larger asset contracts may involve several rounds.

**Judgment posted**

The decision of the arbiter is posted to the forum, with official spaces for comments by the claimants. The arbiter can only benefit by increased reputation if the post wins in the upvote validation pool.

#### Precedent 

The posted judgment is viewable by the pool of arbiters in perpetuity in the forum. Comments praising and criticizing judgments will serve as a record of precedence in the system. Comments live as records of votes eternally, but the system allows for review of comments by reposting the same or similar comments further down the branch for a new, potentially more decisive vote, allowing further confirmation of a precedent or the possibility of overturning it.

The system employed to encourage careful adjudication is the betting pool. Arbiters stake a percentage of their reputation on an up- or downvote. After 1 day of voting the results are revealed and the winners of the decision \(upvoters or downvoters\) split the losers’ stakes, weighted according to their bets. This method determines justice with a democracy weighted according to expertise and encourages effort in discernment of truth.

There is an obvious threat to the anonymity of parties and arbiters in any adjudication process which requires information to be exposed during arbitration and the judgment post. This threat is minimized by good practices in adjudication, such as the use of highly standardized template language which will develop in the forum.

#### Appeals

The rules of the appeals process is encoded in each individual smart contract. Therefore the specifics of the process will evolve as best practices are discovered in the forum and upvoted. In this section we detail one possible scenario.

If an appeal is triggered by a claimant within the designated statute of limitations, a second hearing is initiated. A much higher stake is posted by the appellant to restrain frivolous abuse of resources.  A panel of 3 arbiters is randomly selected, and power to disburse the assets is transferred from the original arbiter. In this case the only variation in the hearing is to repeat the question phase, Step 3\), with the 3 arbiters asking questions, in order, according to reputation.

When a majority of arbiters choose to close the hearing, a private conversation between arbiters is initiated to settle the dispute. When a majority of arbiters choose to close the private conversation between arbiters, a binary vote between claimants is cast. The arbiter with the greatest reputation in the majority opinion writes and posts the judgment, with space available for dissenting opinions.

A second and final appeal is possible, within the contractually specified statute of limitations, which repeats the process with 9 randomly chosen arbiters and a higher stake posted by the appellant.

As stressed previously, ultimately the type of appeals process is always determined by the parties of the smart contract at the point of signing. As the Distributed Jurisdiction platform matures, standards for statutes of limitations will evolve determined by the jurisdiction related to the relevant expertise tags. Similarly, the very process of appeals may vary depending on subject matter. For example, large disputes with less concerns for privacy, such as DAO forks, may begin with several arbiters who are not anonymous. In some cases it is possible arbiters are not even randomly chosen, but are respected figures in the field specified during contract creation. In such cases a dispute may be coded to begin when a quorum percentage of members triggers the break.

Appeals are a challenging element of the Distributed Jurisdiction system, since contradictory demands need to be satisfied. Due to the potential anonymity of claimants, the assets of the contract must be bound by the first smart contract until the end of all possible appeals, which puts the goals of careful deliberation and timely resolution at odds. The crowd-sourced efficiency of the open comment system as an experimental proving ground for good practices is again invoked to give solutions for this challenge.

#### Triage

The details of smart contract creation given above place a significant intellectual burden on the parties—they need to be experts in which type of contract to choose and then which type of dispute resolution protocol is appropriate including weights of expertise tags in various areas of law. It is assumed that the forum will solve many such problems, creating standardized contract templates that are easy to choose for the vast majority of business needs. However, there will always be novel situations, and in order to make the platform more attractive to business use, another layer will be developed which adds a 4th party triage expert who can make such decisions after a dispute starts.

Under this more complicated system, contracting parties can simply add a randomly selected triage expert to their smart contract. Triage expertise will be a separate expertise tag in the forum. A triage expert will have reputation in the expertise of deciding the areas of case law in which general contracts fall. The smart contract gives this triage expert the ability to transfer part of the adjudication fee and the power of asset disbursement to the appropriate expertise tags to randomly select an appropriate arbiter. Then following the general Semada platform function, the triage expert will submit their work for evaluation by other triage experts to the forum.

#### Attacks

Dispute resolution on the Semada Platform is susceptible to a type of corruption: arbiters may be bribed. When both arbiters and parties are anonymous and the channels of communication are carefully limited, this is far less likely than in legacy legal systems.

However, when the bench is limited or when anonymity is neglected, the danger may seem more pronounced than it is in the traditional court system. For instance, an anonymous judge has the opportunity to blackmail a known claimant. Or when an arbiter’s pseudonymous identity is revealed, a claimant may attempt a bribe. Or when the bench is small, a powerful private user could spend a great deal of money engaging the bench with separate contracts beforehand, as happens today in the U.S. when traditional judges are given regular consulting fees by powerful firms to ensure preferential treatment in the future.

For such situations, the system of checks and balances greatly inhibits the potential for corruption. Arbiters are highly incentivized to maintain probity, since their evidence-of-work post will be policed by the entire bench of arbiters with the threat of loss of availability stake. If that is not enough to dissuade corruption, the potential of diminishing the value of all of their reputation is high if they manage to hurt the reputation of the expertise tag.

Further, smart contracts written as suggested above give insurance an unfair settlement will never occur if 1\) anonymous arbiters are randomly chosen according to the weight of their availability stakes, 2\) arbiters are required to post evidence-of-work posts for evaluation by the forum, 3\) claimants are given automatic space in the post for comments, and 4\) a system of appeals is included. In this case, the policing of unfair adjudication is automatic, and the existence of appeals severely weakens the power of bribery.

#### Freedom of Contract

Distributed Jurisdiction epitomizes the principles associated with the freedom of contract. Smart contracting parties may choose contractual terms to incentivize contract formation or protect themselves from unwanted outcomes, especially in an anonymous contracting environment. Such choices may not always be the most economical but may protect parties to smart contracts. Below we list some forms of contractual terms that parties to smart contracts may consider. 

**Symmetric encumbrances**

Once a break clause is triggered, the contract in question is suspended in its current state.  In the crypto economy, where the anonymity of one or both parties is to be expected, the assets in dispute \(money, property, reputation, etc.\) need to be bound in the smart contract. In the blockchain environment it is impractical to seek assets from an anonymous party who may have transferred the assets to new anonymous parties during the interim. Further, it would be damaging to the business platform to make the attempt to retrieve assets of a dispute from outside anonymous parties further down the transaction tree.

Therefore, it is incumbent upon the parties not to enter into an asymmetric contract of bound assets, lest one party may unfairly exert power over the other by encumbering assets in a dispute.

For a party to a smart contract that provides services, for instance, symmetric encumbrance may mean that the service provider stakes sem tokens. Thus, for simple contracts, the Distributed Jurisdiction may be seen as an efficient solution for bringing an escrow service to transactions, small and large.

**Plaintiff stake**

To discourage abuse of the remediation process, it is expected \(but not necessary\) that a plaintiff will add a fee to the contract, called a plaintiff stake, in order to trigger the break clause. In the event of a frivolous dispute, the plaintiff’s stake will be disbursed by the arbiter between the defendant and the Distributed Jurisdiction platform. The size of the stake will be specified by the smart contract, determined previously by the parties.

**Human language**

In order to use a human arbiter, it is expected \(but not necessary\) that many contracting parties will attach a human language version of the contract to clarify intent between parties and for the arbiter’s use in the case of a dispute, as in a Ricardian contract.  


