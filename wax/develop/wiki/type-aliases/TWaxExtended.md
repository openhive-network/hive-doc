[@hiveio/wax](../globals) / TWaxExtended

# Type Alias: TWaxExtended\<YourApi, PreviousCHain\>

> **TWaxExtended**\<`YourApi`, `PreviousCHain`\> = `PreviousCHain` & `object`

Defined in: [wasm/lib/detailed/interfaces.ts:1208](https://gitlab.syncad.com/hive/wax/-/blob/d577f4753a0f64c8d44c7401c48b895fc4c26f93/ts/wasm/lib/detailed/interfaces.ts#L1208)

## Type Parameters

### YourApi

`YourApi`

### PreviousCHain

`PreviousCHain` *extends* [`IHiveChainInterface`](../interfaces/IHiveChainInterface) = [`IHiveChainInterface`](../interfaces/IHiveChainInterface)

## Type Declaration

### api

> `readonly` **api**: [`TDefaultJsonRpcApi`](./TDefaultJsonRpcApi) & [`YourApiData`](./YourApiData)\<`YourApi`\>
