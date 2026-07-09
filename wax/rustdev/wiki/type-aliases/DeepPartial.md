[@hiveio/wax](../globals) / DeepPartial

# Type Alias: DeepPartial\<T\>

> **DeepPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: DeepPartial<T[P]> }` : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/formatters/types.ts:5](https://gitlab.syncad.com/hive/wax/-/blob/9adbfa354c1af2d37ea076dd639e5a0eb429f44b/ts/wasm/lib/detailed/formatters/types.ts#L5)
