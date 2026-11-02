[@hiveio/wax](../globals) / TWaxRestExtended

# Type Alias: TWaxRestExtended\<YourRestApi, PreviousCHain\>

> **TWaxRestExtended**\<`YourRestApi`, `PreviousCHain`\> = `PreviousCHain` & `object`

Defined in: [wasm/lib/detailed/interfaces.ts:1210](https://gitlab.syncad.com/hive/wax/-/blob/b01b7edf441b2e4ae66d53ccdeaa3b4aec519fbb/ts/wasm/lib/detailed/interfaces.ts#L1210)

## Type Parameters

### YourRestApi

`YourRestApi`

### PreviousCHain

`PreviousCHain` *extends* [`IHiveChainInterface`](../interfaces/IHiveChainInterface) = [`IHiveChainInterface`](../interfaces/IHiveChainInterface)

## Type Declaration

### restApi

> `readonly` **restApi**: [`TDefaultRestApi`](./TDefaultRestApi) & [`YourApiData`](./YourApiData)\<`YourRestApi`\>
