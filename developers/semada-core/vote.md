# vote

`function vote(uint256 proposalIndex, address from, uint256 rep, bool vote) public`

Adds vote to `validationPool` mapping for key: `proposalIndex` and adds to the `votes` array a new `vote` struct:

```text
{
address: from,
rep: rep,
vote: vote
}
```





