[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\>: `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

## Type Parameters

• **R** = `void`

## Defined in

[wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/99f67a8c04ccce81c4687346434ed0802c9d7d6a/ts/wasm/lib/detailed/visitor.ts#L14)
