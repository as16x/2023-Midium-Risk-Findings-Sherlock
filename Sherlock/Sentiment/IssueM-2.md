# Issue M-2: 
## [M-02] Risk with Liquidation - Because of partnership requirement, caller may be unable to redeem during liquidation making it less likely for them to be willing to perform the liquidation
### Source: https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/20
---
### Found by
---
GalloDaSballo

### Summary
---
Due to the approval system with pvGLP, liquidations may be less likely

Vulnerability Detail
---
In times of intense price action, a liquidation may have to be performed on pvGLP.

The protocol will offer `liquidate` which will sweep funds out, this is fine and will work as intended because it relies on `transferFrom`.

However, a liquidator will receive the vault token, and may be unable to redeem it.

That's because redemptions have to be performed via `plvGLP depositor` which may not have approved the liquidators account.

This will make it less likely for liquidators to perform the operation as it may force either a manual operation (redemption can be performed by any EOA), or it will require further setup, reducing the number of operators willing to perform the liquidation in the time of need.

### Impact
---
```Solidity
Code Snippet
  function _isEligibleSender() private view {
    if (
      msg.sender != tx.origin && whitelist.isWhitelisted(msg.sender) == false && partners[msg.sender].isActive == false
    ) revert UNAUTHORIZED();
  }
 ```
### Tool used
---
Manual Review

### Recommendation
---
### Discussion
---
r0ohafza

Will be communication with the plutus team and update here accordingly to validate the issue.

zobront

Will be communication with the plutus team and update here accordingly to validate the issue.

This seems to just be missing the fact that Sentiment accounts return true for whitelist.isWhitelisted(), so this isn't an issue.

r0ohafza

Will be communication with the plutus team and update here accordingly to validate the issue.

This seems to just be missing the fact that Sentiment accounts return true for whitelist.isWhitelisted(), so this isn't an issue.

The scenario you are referring to is of an account withdraw/redeem, but when an account is liquidated all plvGLP shares are transferred to the liquidator. This liquidator will not be able to redeem the shares and repay a flashloan used to repay the account debt.

hrishibhat

Considering this issue as a valid medium.
