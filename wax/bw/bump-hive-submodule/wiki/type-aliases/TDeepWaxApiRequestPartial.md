[@hiveio/wax](../globals) / TDeepWaxApiRequestPartial

# Type Alias: TDeepWaxApiRequestPartial\<T\>

> **TDeepWaxApiRequestPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: TDeepWaxApiRequestPartial<T[P]> }` & `Omit`\<[`TWaxApiRequest`](./TWaxApiRequest)\<`any`, `any`\>, `"params"` \| `"result"`\> : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/interfaces.ts:1145](https://gitlab.syncad.com/hive/wax/-/blob/46a2bef62df2021135bf9584986ab43b1291f6fa/ts/wasm/lib/detailed/interfaces.ts#L1145)
