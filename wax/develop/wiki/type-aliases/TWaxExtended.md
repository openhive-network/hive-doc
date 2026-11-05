[@hiveio/wax](../globals) / TWaxExtended

# Type Alias: TWaxExtended\<YourApi, PreviousCHain\>

> **TWaxExtended**\<`YourApi`, `PreviousCHain`\> = `PreviousCHain` & `object`

Defined in: [wasm/lib/detailed/interfaces.ts:1208](https://gitlab.syncad.com/hive/wax/-/blob/1a91d054cf9d01385db4d6224262f77abf1c86b2/ts/wasm/lib/detailed/interfaces.ts#L1208)

## Type Parameters

### YourApi

`YourApi`

### PreviousCHain

`PreviousCHain` *extends* [`IHiveChainInterface`](../interfaces/IHiveChainInterface) = [`IHiveChainInterface`](../interfaces/IHiveChainInterface)

## Type Declaration

### api

> `readonly` **api**: [`TDefaultJsonRpcApi`](./TDefaultJsonRpcApi) & [`YourApiData`](./YourApiData)\<`YourApi`\>
