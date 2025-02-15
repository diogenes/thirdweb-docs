---
slug: /react.usecontractdata
title: useContractData() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useContractData() function

> This feature is currently in beta and may change based on feedback that we receive.

Use this to get data from a contract read-function call.

## Example

```javascript
const { contract } = useContract("{{contract_address}}");
const { data, isLoading, error } = useContractData(
  contract,
  "functionName",
  ...args,
);
```

**Signature:**

```typescript
export declare function useContractData(
  contract: RequiredParam<ReturnType<typeof useContract>["contract"]>,
  functionName: RequiredParam<string>,
  ...args: unknown[] | [...unknown[], CallOverrides]
): import("@tanstack/react-query").UseQueryResult<any, unknown>;
```

## Parameters

| Parameter    | Type                                                                                                | Description                                                                                        |
| ------------ | --------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| contract     | [RequiredParam](./react.requiredparam.md)&lt;ReturnType&lt;typeof useContract&gt;\["contract"\]&gt; | the contract instance of the contract to call a function on                                        |
| functionName | [RequiredParam](./react.requiredparam.md)&lt;string&gt;                                             | the name of the function to call                                                                   |
| args         | unknown\[\] &#124; \[...unknown\[\], CallOverrides\]                                                | The arguments to pass to the function (if any), with optional call arguments as the last parameter |

**Returns:**

import("@tanstack/react-query").UseQueryResult&lt;any, unknown&gt;

a response object that includes the data returned by the function call
