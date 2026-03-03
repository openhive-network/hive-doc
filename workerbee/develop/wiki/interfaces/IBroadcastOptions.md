[@hiveio/workerbee](../globals) / IBroadcastOptions

# Interface: IBroadcastOptions

## Properties

### expireInMs?

> `optional` **expireInMs**: `number`

Time in milliseconds after which the transaction will be considered expired

#### Default

```ts
6000
```

#### Defined in

[src/interfaces.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/5eab2cad232636d85f195a53901c1212e06f9bee/src/interfaces.ts#L24)

***

### verifySignatures?

> `optional` **verifySignatures**: `boolean`

If true, the bot will verify if the signatures in the transaction, applied on chain match the local ones

#### Default

```ts
false
```

#### Defined in

[src/interfaces.ts:16](https://gitlab.syncad.com/hive/workerbee/-/blob/5eab2cad232636d85f195a53901c1212e06f9bee/src/interfaces.ts#L16)
