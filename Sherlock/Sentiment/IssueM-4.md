# Issue M-4: 
## [M-04] No check if Arbitrum L2 sequencer is down in Chainlink feeds
### Source: https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/16
---
### Found by
0xdeadbeef

### Summary
Using Chainlink in L2 chains such as Arbitrum requires to check if the sequencer is down to avoid prices from looking like they are fresh although they are not.

The bug could be leveraged by malicious actors to take advantage of the sequencer downtime.

### Vulnerability Detail
The new GLPOracle is used the get the the price of GLP. There is no check that the sequencer is down:<br>
https://github.com/sherlock-audit/2023-01-sentiment/blob/main/oracle/src/gmx/GLPOracle.sol#L47
```Solidity
    function getEthPrice() internal view returns (uint) {
        (, int answer,, uint updatedAt,) =
            ethUsdPriceFeed.latestRoundData();

        if (block.timestamp - updatedAt >= 86400)
            revert Errors.StalePrice(address(0), address(ethUsdPriceFeed));

        if (answer <= 0)
            revert Errors.NegativePrice(address(0), address(ethUsdPriceFeed));

        return uint(answer);
    }
```
### Impact
The impact depends on the usage of the GLP.
If it is used as part of the collateral for lenders:

- Users can get better borrows if the price is above the actual price
- Users can avoid liquidations if the price is under the actual price
### Code Snippet
### Tool used
VS Code
Manual Review

### Recommendation
It is recommended to follow the code example of Chainlink:<br>
https://docs.chain.link/data-feeds/l2-sequencer-feeds#example-code

### Discussion
zobront

Fix confirmed.
