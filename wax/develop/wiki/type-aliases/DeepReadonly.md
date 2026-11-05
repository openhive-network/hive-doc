[@hiveio/wax](../globals) / DeepReadonly

# Type Alias: DeepReadonly\<T\>

> **DeepReadonly**\<`T`\> = `T` *extends* infer R[] ? [`DeepReadonlyArray`](../interfaces/DeepReadonlyArray)\<`R`\> : `T` *extends* `Function` ? `T` : `T` *extends* `object` ? [`DeepReadonlyObject`](./DeepReadonlyObject)\<`T`\> : `T`

Defined in: [wasm/lib/detailed/formatters/types.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/d577f4753a0f64c8d44c7401c48b895fc4c26f93/ts/wasm/lib/detailed/formatters/types.ts#L9)

## Type Parameters

### T

`T`
