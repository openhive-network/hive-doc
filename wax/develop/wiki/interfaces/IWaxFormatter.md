[@hiveio/wax](../globals) / IWaxFormatter

# Interface: IWaxFormatter

Defined in: [wasm/lib/detailed/formatters/types.ts:119](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/types.ts#L119)

Classes implementing this interface denote that they are ready to handle tagged templates

## Extended by

- [`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

## Properties

### options

> `readonly` **options**: [`DeepReadonly`](../type-aliases/DeepReadonly)\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

Defined in: [wasm/lib/detailed/formatters/types.ts:152](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/types.ts#L152)

Options for the formatter

## Methods

### format()

> **format**\<`I`, `R`\>(`data`): `R`

Defined in: [wasm/lib/detailed/formatters/types.ts:147](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/types.ts#L147)

Formats given data based on formatter options

#### Type Parameters

##### I

`I` = `any`

##### R

`R` = `any`

#### Parameters

##### data

`I`

raw data

#### Returns

`R`

formatted data

#### Example

**Formatting data**

```typescript
formatter.format(naiObject);
```

***

### waxify()

> **waxify**(`strings`, ...`args`): `string`

Defined in: [wasm/lib/detailed/formatters/types.ts:133](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/types.ts#L133)

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

**Formatting data**

```typescript
formatter.waxify`Hello, ${"alice"}! My account value is ${naiObject}`
```
