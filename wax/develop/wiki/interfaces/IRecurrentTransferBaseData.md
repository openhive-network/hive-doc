[@hiveio/wax](../globals) / IRecurrentTransferBaseData

# Interface: IRecurrentTransferBaseData

## Extended by

- [`IRecurrentTransferData`](./IRecurrentTransferData)
- [`IRecurrentTransferRemovalOperationData`](./IRecurrentTransferRemovalOperationData)

## Properties

### from

> **from**: `string`

Account to transfer asset from.

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/a510b47435a15d0d51739b35f2f02fbd490eb5ac/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L12)

***

### pairId?

> `optional` **pairId**: `number`

Since HF 28, if user has more than one recurrent transfer to the same receiver
or if user creates the recurrent transfer using pairId, user has to specify the pairId
in order to update or remove the defined recurrent transfer.

#### Default

```ts
0
```

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:24](https://gitlab.syncad.com/hive/wax/-/blob/a510b47435a15d0d51739b35f2f02fbd490eb5ac/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L24)

***

### to

> **to**: `string`

Account to transfer asset to. Cannot set a transfer to yourself.

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/a510b47435a15d0d51739b35f2f02fbd490eb5ac/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L16)
