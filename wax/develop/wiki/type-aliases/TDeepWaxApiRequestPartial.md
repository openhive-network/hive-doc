[@hiveio/wax](../globals) / TDeepWaxApiRequestPartial

# Type Alias: TDeepWaxApiRequestPartial\<T\>

> **TDeepWaxApiRequestPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: TDeepWaxApiRequestPartial<T[P]> }` & `Omit`\<[`TWaxApiRequest`](./TWaxApiRequest)\<`any`, `any`\>, `"params"` \| `"result"`\> : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/interfaces.ts:1145](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/interfaces.ts#L1145)
