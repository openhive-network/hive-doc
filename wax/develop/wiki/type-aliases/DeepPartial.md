[@hiveio/wax](../globals) / DeepPartial

# Type Alias: DeepPartial\<T\>

> **DeepPartial**\<`T`\> = `T` *extends* `object` ? `{ [P in keyof T]?: DeepPartial<T[P]> }` : `T`

Defined in: [wasm/lib/detailed/formatters/types.ts:5](https://gitlab.syncad.com/hive/wax/-/blob/d577f4753a0f64c8d44c7401c48b895fc4c26f93/ts/wasm/lib/detailed/formatters/types.ts#L5)

## Type Parameters

### T

`T`
