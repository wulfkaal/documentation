# newProposal

```text
function newProposal(string tokenSymbol, string evidence) public payable
```

* Opens a validation pool by incrementing `proposalIndex` and adding an entry to `validationPool` mapping with key: `proposalIndex` and value: new `pool` struct:

  ```text
  struct pool {
    address from;
    string tokenSymbol;
    uint256 timeout;
    string evidence;
    vote[];
  }
  ```

* REP is minted in ERC-20 contract equal to the SEM fee sent to function
* `vote(uint256 proposalIndex, address sender, uint256 rep, bool vote)` is called with 50% of newly minted REP and "yes" vote staked to `sender` address.
* `vote(uint256 proposalIndex, address sender, uint256 rep, bool vote)` is called with 50% of newly minted REP and "no" vote staked to null address.
* Voting begins by existing DAO members.
* `checkVote(uint256 proposalIndex)` is called by DApp after the timeout has elapsed.
* Voting proceeds and REP is transferred based on outcome after timeout by calling `checkVote(uint256 proposalIndex)`

