---
slug: /react.usetoken
title: useToken() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useToken() function

Hook for getting an instance of a `Token` contract. This contract supports ERC20 compliant tokens.

## Example

```javascript
import { useToken } from '@thirdweb-dev/react'

export default function Component() {
  const token = useToken("<YOUR-CONTRACT-ADDRESS>")

  // Now you can use the token contract in the rest of the component

  // For example, this function will get the connected wallets token balance
  async function balance() {
    const balance = await token.balance()
    return balance
  }

  ...
}
```

**Signature:**

```typescript
export declare function useToken(contractAddress?: string): Token | undefined;
```

## Parameters

| Parameter       | Type   | Description                                                                           |
| --------------- | ------ | ------------------------------------------------------------------------------------- |
| contractAddress | string | <i>(Optional)</i> the address of the Token contract, found in your thirdweb dashboard |

**Returns:**

Token \| undefined
