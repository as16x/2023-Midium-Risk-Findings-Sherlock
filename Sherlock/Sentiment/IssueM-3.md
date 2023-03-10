# Issue M-3: 
## [M-02] `PreviewRedeem` may under-price the value of the asset
### Source: https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/19
---
### Found by
---
GalloDaSballo

### Summary
---
previewRedeem will return an incorrect result based on `address(0)`

If you get the partnership the fee changes, the address could change the value
This may enable: Unfairer (bps wise), liquidations when they shouldn't happen, also will enable marginally higher profit for liquidators as they may be able to benefit from the reduction of the fee

### Vulnerability Detail
---
### Impact
---
A user may get liquidated earlier, and the accounting would be incorrect

### Code Snippet
---
https://arbiscan.io/address/0x13f0d29b5b83654a200e4540066713d50547606e#code
```Solidity
  function previewRedeem(address _addr, uint256 _shares)
    external
    view
    returns (
      uint256 _exitFeeLessRebate,
      uint256 _rebateAmount,
      uint256 _assetsLessFee
    )
  {
    PartnerInfo memory partner = partners[_addr];
    uint256 exitFee = partner.isActive ? partner.exitFee : defaultExitFee;
    uint256 rebate = partner.isActive ? partner.rebate : defaultVaultRebate;
    uint256 assets = IERC4626(vault).previewRedeem(_shares);

    uint256 _exitFee;
    (_exitFee, _assetsLessFee) = _calculateFee(assets, exitFee);
    (_rebateAmount, _exitFeeLessRebate) = _calculateFee(_exitFee, rebate);
  }
 ```
### Tool used
Manual Review

### Recommendation
Use the account to determine the price
