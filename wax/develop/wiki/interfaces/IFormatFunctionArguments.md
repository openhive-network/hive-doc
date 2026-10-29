[@hiveio/wax](../globals) / IFormatFunctionArguments

# Interface: IFormatFunctionArguments\<TSource, TTarget\>

Defined in: [wasm/lib/detailed/formatters/types.ts:64](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/types.ts#L64)

## Type Parameters

### TSource

`TSource` = `object`

### TTarget

`TTarget` = `any`

## Properties

### options

> `readonly` **options**: [`DeepReadonly`](../type-aliases/DeepReadonly)\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

Defined in: [wasm/lib/detailed/formatters/types.ts:71](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/types.ts#L71)

Formatter options

***

### source

> `readonly` **source**: [`DeepReadonly`](../type-aliases/DeepReadonly)\<`TSource`\>

Defined in: [wasm/lib/detailed/formatters/types.ts:79](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/types.ts#L79)

Source readonly unchanged input value for parsing raw data

***

### target

> **target**: `TTarget`

Defined in: [wasm/lib/detailed/formatters/types.ts:86](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/types.ts#L86)

Target formatter data that might have been previously changed by other formatters
