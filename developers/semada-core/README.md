# Semada Core

Semada Core is a single smart contract that contains the following features:

* Maintains the validation pool
* Proposal forum 
* Minting of REP
* Distribution of SEM salary

#### Properties

`mapping(string => address) rep`

`uint256 proposalIndex`

`mapping(uint256 => pool) validationPool`

`uint256 minimumFee`

#### Structs

```text
struct pool {
  address from;
  string tokenSymbol;
  uint256 timeout;
  string evidence;
  vote[];
}
```

```text
struct vote {
  address from;
  uint 256 rep;
  bool vote;
}
```

