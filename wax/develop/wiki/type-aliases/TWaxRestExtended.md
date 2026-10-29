[@hiveio/wax](../globals) / TWaxRestExtended

# Type Alias: TWaxRestExtended\<YourRestApi, PreviousCHain\>

> **TWaxRestExtended**\<`YourRestApi`, `PreviousCHain`\> = `PreviousCHain` & `object`

Defined in: [wasm/lib/detailed/interfaces.ts:1210](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L1210)

## Type Parameters

### YourRestApi

`YourRestApi`

### PreviousCHain

`PreviousCHain` *extends* [`IHiveChainInterface`](../interfaces/IHiveChainInterface) = [`IHiveChainInterface`](../interfaces/IHiveChainInterface)

## Type Declaration

### restApi

> `readonly` **restApi**: [`TDefaultRestApi`](./TDefaultRestApi) & [`YourApiData`](./YourApiData)\<`YourRestApi`\>
