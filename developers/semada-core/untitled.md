# joinDao



```text
function joinDao(string tokenSymbol) public payable
```

Checks `rep` mapping for a key matching `tokenSymbol` . 

If `tokenSymbol` does not exist:

* Deploys a new ERC-20 contract representing REP tokens for the given DAO token symbol.
* New token smart contract address is added to `rep` mapping with key: `tokenSymbol` and value: `address`.
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
* `checkVote(uint256 proposalIndex)` is called by DApp after the timeout has elapsed. Because there is only one address that can vote \(the originator of the DAO\), the "yes" vote wins.
* The "yes" vote wins the tie of staked REP.
* 50% of REP from "yes" and 50% of "no" is transferred to the `sender` .



If `tokenSymbol` does exist:

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
* `checkVote(uint256 proposalIndex)` is called by DApp after the timeout has elapsed.
* Voting proceeds and REP is transferred based on outcome after timeout by calling `checkVote(uint256 proposalIndex)`

#### Exceptions

_SEM sent too low:_ If SEM is lower than `minimumFee`

 

