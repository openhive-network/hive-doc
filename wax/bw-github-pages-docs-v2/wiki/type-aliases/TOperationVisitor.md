[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\>: `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

## Type Parameters

• **R** = `void`

## Defined in

[wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/8ad2b63c881a2d911b31e0c06383e6fc0fe73d22/ts/wasm/lib/detailed/visitor.ts#L14)
