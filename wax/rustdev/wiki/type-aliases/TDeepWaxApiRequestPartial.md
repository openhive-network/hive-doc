[@hiveio/wax](../globals) / TDeepWaxApiRequestPartial

# Type Alias: TDeepWaxApiRequestPartial\<T\>

> **TDeepWaxApiRequestPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: TDeepWaxApiRequestPartial<T[P]> }` & `Omit`\<[`TWaxApiRequest`](./TWaxApiRequest)\<`any`, `any`\>, `"params"` \| `"result"`\> : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/interfaces.ts:1123](https://gitlab.syncad.com/hive/wax/-/blob/91e524c19e634d1be57a3695af351d55611876c7/ts/wasm/lib/detailed/interfaces.ts#L1123)
