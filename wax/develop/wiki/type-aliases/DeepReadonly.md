[@hiveio/wax](../globals) / DeepReadonly

# Type Alias: DeepReadonly\<T\>

> **DeepReadonly**\<`T`\>: `T` *extends* infer R[] ? [`DeepReadonlyArray`](../interfaces/DeepReadonlyArray)\<`R`\> : `T` *extends* `Function` ? `T` : `T` *extends* `object` ? [`DeepReadonlyObject`](./DeepReadonlyObject)\<`T`\> : `T`

## Type Parameters

• **T**

## Defined in

[wasm/lib/detailed/formatters/types.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/types.ts#L9)
