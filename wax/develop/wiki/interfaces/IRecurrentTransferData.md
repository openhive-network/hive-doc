[@hiveio/wax](../globals) / IRecurrentTransferData

# Interface: IRecurrentTransferData

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L27)

## Extends

- [`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData)

## Properties

### amount

> **amount**: [`asset`](./asset)

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L32)

The amount of asset to transfer.
Allowed assets: **HIVE** and **HBD**.

***

### executions?

> `optional` **executions?**: `number`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L53)

How many times the recurrent payment will be executed.
Executions must be at least 2, if you set executions to 1 the recurrent transfer will not be executed.

#### Default

```ts
2
```

***

### from

> **from**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L12)

Account to transfer asset from.

#### Inherited from

[`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData).[`from`](./IRecurrentTransferBaseData#from)

***

### memo?

> `optional` **memo?**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L38)

Must be shorter than 2048 characters.

#### Default

```ts
""
```

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

#### Inherited from

[`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData).[`pairId`](./IRecurrentTransferBaseData#pairid)

***

### recurrence?

> `optional` **recurrence?**: `number`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:46](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L46)

How often will the payment be triggered, unit: hours.
The first transfer is executed immediately.
The minimum value of the parameter is 24 h.

#### Default

```ts
24
```

***

### to

> **to**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L16)

Account to transfer asset to. Cannot set a transfer to yourself.

#### Inherited from

[`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData).[`to`](./IRecurrentTransferBaseData#to)
