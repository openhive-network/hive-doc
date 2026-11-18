[@hiveio/wax](../globals) / TWaxExtended

# Type Alias: TWaxExtended\<YourApi, PreviousCHain\>

> **TWaxExtended**\<`YourApi`, `PreviousCHain`\> = `PreviousCHain` & `object`

Defined in: [wasm/lib/detailed/interfaces.ts:1238](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1238)

## Type Parameters

### YourApi

`YourApi`

### PreviousCHain

`PreviousCHain` *extends* [`IHiveChainInterface`](../interfaces/IHiveChainInterface) = [`IHiveChainInterface`](../interfaces/IHiveChainInterface)

## Type Declaration

### api

> `readonly` **api**: [`TDefaultJsonRpcApi`](./TDefaultJsonRpcApi) & [`YourApiData`](./YourApiData)\<`YourApi`\>
