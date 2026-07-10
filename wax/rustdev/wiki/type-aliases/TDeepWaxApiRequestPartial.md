[@hiveio/wax](../globals) / TDeepWaxApiRequestPartial

# Type Alias: TDeepWaxApiRequestPartial\<T\>

> **TDeepWaxApiRequestPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: TDeepWaxApiRequestPartial<T[P]> }` & `Omit`\<[`TWaxApiRequest`](./TWaxApiRequest)\<`any`, `any`\>, `"params"` \| `"result"`\> : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/interfaces.ts:1123](https://gitlab.syncad.com/hive/wax/-/blob/01139ad1e8636f968fe3751f59b69c3a0bb4bb0c/ts/wasm/lib/detailed/interfaces.ts#L1123)
