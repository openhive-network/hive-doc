[@hiveio/wax](../globals) / DeepPartial

# Type Alias: DeepPartial\<T\>

> **DeepPartial**\<`T`\>: `T` *extends* `object` ? `{ [P in keyof T]?: DeepPartial<T[P]> }` : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/formatters/types.ts:5](https://gitlab.syncad.com/hive/wax/-/blob/85fd5270526c5a18b82df1989bfd5ab402e6c9b5/ts/wasm/lib/detailed/formatters/types.ts#L5)
