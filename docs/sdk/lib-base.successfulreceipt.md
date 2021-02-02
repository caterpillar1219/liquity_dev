<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@liquity/lib-base](./lib-base.md) &gt; [SuccessfulReceipt](./lib-base.successfulreceipt.md)

## SuccessfulReceipt type

Indicates that the transaction has been mined, but it failed.

<b>Signature:</b>

```typescript
export declare type SuccessfulReceipt<R = unknown, D = unknown> = {
    status: "succeeded";
    rawReceipt: R;
    details: D;
};
```

## Remarks

The `rawReceipt` property is an implementation-specific transaction receipt object.

The `details` property may contain more information about the transaction. See the return types of [TransactableLiquity](./lib-base.transactableliquity.md) functions for the exact contents of `details` for each type of Liquity transaction.

Returned by [SentLiquityTransaction.getReceipt()](./lib-base.sentliquitytransaction.getreceipt.md) and [SentLiquityTransaction.waitForReceipt()](./lib-base.sentliquitytransaction.waitforreceipt.md)<!-- -->.
