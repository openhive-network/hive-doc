[@hiveio/wax](../globals) / IRecurrentTransferBaseData

# Interface: IRecurrentTransferBaseData

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:8](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L8)

## Extended by

- [`IRecurrentTransferData`](./IRecurrentTransferData)
- [`IRecurrentTransferRemovalOperationData`](./IRecurrentTransferRemovalOperationData)

## Properties

### from

> **from**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L12)

Account to transfer asset from.

***

### pairId?

> `optional` **pairId?**: `number`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:24](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L24)

Since HF 28, if user has more than one recurrent transfer to the same receiver
or if user creates the recurrent transfer using pairId, user has to specify the pairId
in order to update or remove the defined recurrent transfer.

#### Default

```ts
0
```

***

### to

> **to**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L16)

Account to transfer asset to. Cannot set a transfer to yourself.
