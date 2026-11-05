[@hiveio/wax](../globals) / TDeepWaxApiRequestPartial

# Type Alias: TDeepWaxApiRequestPartial\<T\>

> **TDeepWaxApiRequestPartial**\<`T`\> = `T` *extends* `object` ? `{ [P in keyof T]?: TDeepWaxApiRequestPartial<T[P]> }` & `Omit`\<[`TWaxApiRequest`](./TWaxApiRequest)\<`any`, `any`\>, `"params"` \| `"result"`\> : `T`

Defined in: [wasm/lib/detailed/interfaces.ts:1123](https://gitlab.syncad.com/hive/wax/-/blob/d577f4753a0f64c8d44c7401c48b895fc4c26f93/ts/wasm/lib/detailed/interfaces.ts#L1123)

## Type Parameters

### T

`T`
