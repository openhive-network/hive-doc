[@hiveio/wax](../globals) / DeepPartial

# Type Alias: DeepPartial\<T\>

> **DeepPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: DeepPartial<T[P]> }` : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/formatters/types.ts:5](https://gitlab.syncad.com/hive/wax/-/blob/ac0ea25b3e26f059ca8c3033877d3dc56983d37a/ts/wasm/lib/detailed/formatters/types.ts#L5)
