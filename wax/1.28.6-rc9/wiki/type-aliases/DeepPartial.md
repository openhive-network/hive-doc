[@hiveio/wax](../globals) / DeepPartial

# Type Alias: DeepPartial\<T\>

> **DeepPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: DeepPartial<T[P]> }` : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/formatters/types.ts:5](https://gitlab.syncad.com/hive/wax/-/blob/808c2006f3c59ae1da24855e052c95bb7c70fc86/ts/wasm/lib/detailed/formatters/types.ts#L5)
