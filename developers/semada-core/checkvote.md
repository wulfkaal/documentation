# checkVote

```text
function checkVote(uint256 proposalIndex) public
```

* Votes for key `proposalIndex` in `validationPool` are tallied by summing `rep` by "yes" and "no" votes.
* If "yes" vote wins 
  * Transfer REP staked for each "yes" vote to the `from` address on the vote
  * Transfer REP staked for each "no" vote pro-rata to DAO members \(in ERC-20 contract\) based on REP held.
* If "no" vote wins
  * Transfer REP staked for each "yes" vote pro-rata to DAO members \(in ERC-20 contract\) based on REP held.
  * Burn REP staked for "no" vote on null address. This is the newly minted 50% of REP that was staked against null address when proposal was added to `validationPool`.

