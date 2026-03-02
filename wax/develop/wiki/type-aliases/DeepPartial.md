[@hiveio/wax](../globals) / DeepPartial

# Type Alias: DeepPartial\<T\>

> **DeepPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: DeepPartial<T[P]> }` : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/formatters/types.ts:5](https://gitlab.syncad.com/hive/wax/-/blob/3997c7919fd81ba2e74d57d20d575f6f240bbd7b/ts/wasm/lib/detailed/formatters/types.ts#L5)
