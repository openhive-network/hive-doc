[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\> = `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

Defined in: [wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L14)

## Type Parameters

### R

`R` = `void`
