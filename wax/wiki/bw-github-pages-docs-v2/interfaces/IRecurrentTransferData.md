[@hiveio/wax](../globals) / IRecurrentTransferData

# Interface: IRecurrentTransferData

## Extends

- [`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData)

## Properties

### amount

> **amount**: [`asset`](./asset)

The amount of asset to transfer.
Allowed assets: **HIVE** and **HBD**.

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L32)

***

### executions?

> `optional` **executions**: `number`

How many times the recurrent payment will be executed.
Executions must be at least 2, if you set executions to 1 the recurrent transfer will not be executed.

#### Default

```ts
2
```

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L53)

***

### from

> **from**: `string`

Account to transfer asset from.

#### Inherited from

[`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData).[`from`](./IRecurrentTransferBaseData#from)

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L12)

***

### memo?

> `optional` **memo**: `string`

Must be shorter than 2048 characters.

#### Default

```ts
""
```

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L38)

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

#### Inherited from

[`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData).[`pairId`](./IRecurrentTransferBaseData#pairid)

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:24](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L24)

***

### recurrence?

> `optional` **recurrence**: `number`

How often will the payment be triggered, unit: hours.
The first transfer is executed immediately.
The minimum value of the parameter is 24 h.

#### Default

```ts
24
```

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:46](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L46)

***

### to

> **to**: `string`

Account to transfer asset to. Cannot set a transfer to yourself.

#### Inherited from

[`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData).[`to`](./IRecurrentTransferBaseData#to)

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L16)
