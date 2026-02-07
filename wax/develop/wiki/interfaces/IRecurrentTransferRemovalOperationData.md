[@hiveio/wax](../globals) / IRecurrentTransferRemovalOperationData

# Interface: IRecurrentTransferRemovalOperationData

## Extends

- [`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData)

## Properties

### from

> **from**: `string`

Account to transfer asset from.

#### Inherited from

[`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData).[`from`](./IRecurrentTransferBaseData#from)

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/c159167d6b6a946ec4584e0166aad2fa59a675fb/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L12)

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

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:24](https://gitlab.syncad.com/hive/wax/-/blob/c159167d6b6a946ec4584e0166aad2fa59a675fb/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L24)

***

### to

> **to**: `string`

Account to transfer asset to. Cannot set a transfer to yourself.

#### Inherited from

[`IRecurrentTransferBaseData`](./IRecurrentTransferBaseData).[`to`](./IRecurrentTransferBaseData#to)

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/c159167d6b6a946ec4584e0166aad2fa59a675fb/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L16)
