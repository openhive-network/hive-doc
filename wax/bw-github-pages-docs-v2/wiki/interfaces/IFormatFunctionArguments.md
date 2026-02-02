[@hiveio/wax](../globals) / IFormatFunctionArguments

# Interface: IFormatFunctionArguments\<TSource, TTarget\>

## Type Parameters

• **TSource** = `object`

• **TTarget** = `any`

## Properties

### options

> `readonly` **options**: [`DeepReadonlyObject`](../type-aliases/DeepReadonlyObject)\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

Formatter options

#### Defined in

[wasm/lib/detailed/formatters/types.ts:71](https://gitlab.syncad.com/hive/wax/-/blob/68ec4e7437e5f2c8b344551ab8912a85d3c584ec/ts/wasm/lib/detailed/formatters/types.ts#L71)

***

### source

> `readonly` **source**: [`DeepReadonly`](../type-aliases/DeepReadonly)\<`TSource`\>

Source readonly unchanged input value for parsing raw data

#### Defined in

[wasm/lib/detailed/formatters/types.ts:79](https://gitlab.syncad.com/hive/wax/-/blob/68ec4e7437e5f2c8b344551ab8912a85d3c584ec/ts/wasm/lib/detailed/formatters/types.ts#L79)

***

### target

> **target**: `TTarget`

Target formatter data that might have been previously changed by other formatters

#### Defined in

[wasm/lib/detailed/formatters/types.ts:86](https://gitlab.syncad.com/hive/wax/-/blob/68ec4e7437e5f2c8b344551ab8912a85d3c584ec/ts/wasm/lib/detailed/formatters/types.ts#L86)
