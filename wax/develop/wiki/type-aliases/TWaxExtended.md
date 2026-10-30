[@hiveio/wax](../globals) / TWaxExtended

# Type Alias: TWaxExtended\<YourApi, PreviousCHain\>

> **TWaxExtended**\<`YourApi`, `PreviousCHain`\> = `PreviousCHain` & `object`

Defined in: [wasm/lib/detailed/interfaces.ts:1208](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/interfaces.ts#L1208)

## Type Parameters

### YourApi

`YourApi`

### PreviousCHain

`PreviousCHain` *extends* [`IHiveChainInterface`](../interfaces/IHiveChainInterface) = [`IHiveChainInterface`](../interfaces/IHiveChainInterface)

## Type Declaration

### api

> `readonly` **api**: [`TDefaultJsonRpcApi`](./TDefaultJsonRpcApi) & [`YourApiData`](./YourApiData)\<`YourApi`\>
