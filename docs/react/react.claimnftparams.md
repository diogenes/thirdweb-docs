---
slug: /react.claimnftparams
title: ClaimNFTParams type
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## ClaimNFTParams type

> This feature is currently in beta and may change based on feedback that we receive.

The params for the [useClaimNFT()](./react.useclaimnft.md) hook mutation.

**Signature:**

```typescript
export declare type ClaimNFTParams<TContract extends DropContract> =
  TContract extends Erc1155
    ? {
        to: WalletAddress;
        tokenId: BigNumberish;
        quantity: BigNumberish;
        checkERC20Allowance?: boolean;
      }
    : {
        to: WalletAddress;
        quantity: BigNumberish;
        checkERC20Allowance?: boolean;
      };
```

**References:** [DropContract](./react.dropcontract.md), [WalletAddress](./react.walletaddress.md)
