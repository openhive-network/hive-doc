[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\> = `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

Defined in: [wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/d577f4753a0f64c8d44c7401c48b895fc4c26f93/ts/wasm/lib/detailed/visitor.ts#L14)

## Type Parameters

### R

`R` = `void`
