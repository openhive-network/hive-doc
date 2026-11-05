[@hiveio/wax](../globals) / DeepPartial

# Type Alias: DeepPartial\<T\>

> **DeepPartial**\<`T`\> = `T` *extends* `object` ? `{ [P in keyof T]?: DeepPartial<T[P]> }` : `T`

Defined in: [wasm/lib/detailed/formatters/types.ts:5](https://gitlab.syncad.com/hive/wax/-/blob/1a91d054cf9d01385db4d6224262f77abf1c86b2/ts/wasm/lib/detailed/formatters/types.ts#L5)

## Type Parameters

### T

`T`
