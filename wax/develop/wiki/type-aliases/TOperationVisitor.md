[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\> = `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

Defined in: [wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/visitor.ts#L14)

## Type Parameters

### R

`R` = `void`
