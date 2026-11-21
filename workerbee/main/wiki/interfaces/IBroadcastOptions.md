[@hiveio/workerbee](../globals) / IBroadcastOptions

# Interface: IBroadcastOptions

Defined in: [src/interfaces.ts:9](https://gitlab.syncad.com/hive/workerbee/-/blob/bc217d4103c521db7966585fc06621a710c6556e/src/interfaces.ts#L9)

## Properties

### expireInMs?

> `optional` **expireInMs?**: `number`

Defined in: [src/interfaces.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/bc217d4103c521db7966585fc06621a710c6556e/src/interfaces.ts#L24)

Time in milliseconds after which the transaction will be considered expired

#### Default

```ts
6000
```

***

### verifySignatures?

> `optional` **verifySignatures?**: `boolean`

Defined in: [src/interfaces.ts:16](https://gitlab.syncad.com/hive/workerbee/-/blob/bc217d4103c521db7966585fc06621a710c6556e/src/interfaces.ts#L16)

If true, the bot will verify if the signatures in the transaction, applied on chain match the local ones

#### Default

```ts
false
```
