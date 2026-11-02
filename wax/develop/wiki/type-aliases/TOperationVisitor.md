[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\> = `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

Defined in: [wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/b01b7edf441b2e4ae66d53ccdeaa3b4aec519fbb/ts/wasm/lib/detailed/visitor.ts#L14)

## Type Parameters

### R

`R` = `void`
