[@hiveio/wax](../globals) / DeepReadonly

# Type Alias: DeepReadonly\<T\>

> **DeepReadonly**\<`T`\> = `T` *extends* infer R[] ? [`DeepReadonlyArray`](../interfaces/DeepReadonlyArray)\<`R`\> : `T` *extends* `Function` ? `T` : `T` *extends* `object` ? [`DeepReadonlyObject`](./DeepReadonlyObject)\<`T`\> : `T`

Defined in: [wasm/lib/detailed/formatters/types.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/b01b7edf441b2e4ae66d53ccdeaa3b4aec519fbb/ts/wasm/lib/detailed/formatters/types.ts#L9)

## Type Parameters

### T

`T`
