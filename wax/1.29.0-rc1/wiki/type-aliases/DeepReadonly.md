[@hiveio/wax](../globals) / DeepReadonly

# Type Alias: DeepReadonly\<T\>

> **DeepReadonly**\<`T`\>: `T` *extends* infer R[] ? [`DeepReadonlyArray`](../interfaces/DeepReadonlyArray)\<`R`\> : `T` *extends* `Function` ? `T` : `T` *extends* `object` ? [`DeepReadonlyObject`](./DeepReadonlyObject)\<`T`\> : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/formatters/types.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/3335470bc2a18357bb00b92dad6ea055e3a2edc9/ts/wasm/lib/detailed/formatters/types.ts#L9)
