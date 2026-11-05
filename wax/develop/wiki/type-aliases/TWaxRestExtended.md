[@hiveio/wax](../globals) / TWaxRestExtended

# Type Alias: TWaxRestExtended\<YourRestApi, PreviousCHain\>

> **TWaxRestExtended**\<`YourRestApi`, `PreviousCHain`\> = `PreviousCHain` & `object`

Defined in: [wasm/lib/detailed/interfaces.ts:1210](https://gitlab.syncad.com/hive/wax/-/blob/1a91d054cf9d01385db4d6224262f77abf1c86b2/ts/wasm/lib/detailed/interfaces.ts#L1210)

## Type Parameters

### YourRestApi

`YourRestApi`

### PreviousCHain

`PreviousCHain` *extends* [`IHiveChainInterface`](../interfaces/IHiveChainInterface) = [`IHiveChainInterface`](../interfaces/IHiveChainInterface)

## Type Declaration

### restApi

> `readonly` **restApi**: [`TDefaultRestApi`](./TDefaultRestApi) & [`YourApiData`](./YourApiData)\<`YourRestApi`\>
