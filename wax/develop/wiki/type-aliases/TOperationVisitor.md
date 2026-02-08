[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\>: `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

## Type Parameters

• **R** = `void`

## Defined in

[wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L14)
