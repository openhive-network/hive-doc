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

[src/interfaces.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/interfaces.ts#L24)

***

### verifySignatures?

> `optional` **verifySignatures**: `boolean`

If true, the bot will verify if the signatures in the transaction, applied on chain match the local ones

#### Default

```ts
false
```

#### Defined in

[src/interfaces.ts:16](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/interfaces.ts#L16)
