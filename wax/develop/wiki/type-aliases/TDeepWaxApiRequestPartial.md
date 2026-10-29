[@hiveio/wax](../globals) / TDeepWaxApiRequestPartial

# Type Alias: TDeepWaxApiRequestPartial\<T\>

> **TDeepWaxApiRequestPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: TDeepWaxApiRequestPartial<T[P]> }` & `Omit`\<[`TWaxApiRequest`](./TWaxApiRequest)\<`any`, `any`\>, `"params"` \| `"result"`\> : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/interfaces.ts:1123](https://gitlab.syncad.com/hive/wax/-/blob/f133f2ed0d45e5b77b23fe13820ee7175aafab0f/ts/wasm/lib/detailed/interfaces.ts#L1123)
