[@hiveio/wax](../globals) / IWaxFormatter

# Interface: IWaxFormatter

Classes implementing this interface denote that they are ready to handle tagged templates

## Extended by

- [`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

## Properties

### options

> `readonly` **options**: [`DeepReadonlyObject`](../type-aliases/DeepReadonlyObject)\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

Options for the formatter

#### Defined in

[wasm/lib/detailed/formatters/types.ts:152](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/formatters/types.ts#L152)

## Methods

### format()

> **format**\<`I`, `R`\>(`data`): `R`

Formats given data based on formatter options

#### Type Parameters

• **I** = `any`

• **R** = `any`

#### Parameters

##### data

`I`

raw data

#### Returns

`R`

formatted data

#### Example

```typescript
formatter.format(naiObject);
```

#### Defined in

[wasm/lib/detailed/formatters/types.ts:147](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/formatters/types.ts#L147)

***

### waxify()

> **waxify**(`strings`, ...`args`): `string`

Formats given text based on arguments structure

#### Parameters

##### strings

`TemplateStringsArray`

raw strings

##### args

...`unknown`[]

arguments to be parsed using custom wax formatters

#### Returns

`string`

formatted data

#### Example

```typescript
formatter.waxify`Hello, ${"alice"}! My account value is ${naiObject}`
```

#### Defined in

[wasm/lib/detailed/formatters/types.ts:133](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/formatters/types.ts#L133)
