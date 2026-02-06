[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\>: `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

## Type Parameters

• **R** = `void`

## Defined in

[wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/fd756288e9a34740db6a53e19d17ae5e94b49e4a/ts/wasm/lib/detailed/visitor.ts#L14)
