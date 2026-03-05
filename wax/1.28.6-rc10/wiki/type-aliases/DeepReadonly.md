[@hiveio/wax](../globals) / DeepReadonly

# Type Alias: DeepReadonly\<T\>

> **DeepReadonly**\<`T`\>: `T` *extends* infer R[] ? [`DeepReadonlyArray`](../interfaces/DeepReadonlyArray)\<`R`\> : `T` *extends* `Function` ? `T` : `T` *extends* `object` ? [`DeepReadonlyObject`](./DeepReadonlyObject)\<`T`\> : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/formatters/types.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/d6522a3e1a025201fe9fbb1c3e29eac231eab332/ts/wasm/lib/detailed/formatters/types.ts#L9)
