[@hiveio/wax](../globals) / TWaxExtended

# Type Alias: TWaxExtended\<YourApi, PreviousCHain\>

> **TWaxExtended**\<`YourApi`, `PreviousCHain`\> = `PreviousCHain` & `object`

Defined in: [wasm/lib/detailed/interfaces.ts:1208](https://gitlab.syncad.com/hive/wax/-/blob/b01b7edf441b2e4ae66d53ccdeaa3b4aec519fbb/ts/wasm/lib/detailed/interfaces.ts#L1208)

## Type Parameters

### YourApi

`YourApi`

### PreviousCHain

`PreviousCHain` *extends* [`IHiveChainInterface`](../interfaces/IHiveChainInterface) = [`IHiveChainInterface`](../interfaces/IHiveChainInterface)

## Type Declaration

### api

> `readonly` **api**: [`TDefaultJsonRpcApi`](./TDefaultJsonRpcApi) & [`YourApiData`](./YourApiData)\<`YourApi`\>
