[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\>: `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

## Type Parameters

• **R** = `void`

## Defined in

[wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/cf6608b95d72b7ca1e7b50031e8dc670f196e613/ts/wasm/lib/detailed/visitor.ts#L14)
