[@hiveio/wax](../globals) / TOperationVisitor

# Type Alias: TOperationVisitor\<R\>

> **TOperationVisitor**\<`R`\> = `{ [K in keyof Required<operation>]?: (op: Required<operation>[K]) => R }`

Defined in: [wasm/lib/detailed/visitor.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/1a91d054cf9d01385db4d6224262f77abf1c86b2/ts/wasm/lib/detailed/visitor.ts#L14)

## Type Parameters

### R

`R` = `void`
