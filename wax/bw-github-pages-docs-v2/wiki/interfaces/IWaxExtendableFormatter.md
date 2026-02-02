[@hiveio/wax](../globals) / IWaxExtendableFormatter

# Interface: IWaxExtendableFormatter

Classes implementing this interface denote that they are ready to handle tagged templates

## Extends

- [`IWaxFormatter`](./IWaxFormatter)

## Properties

### options

> `readonly` **options**: [`DeepReadonlyObject`](../type-aliases/DeepReadonlyObject)\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

Options for the formatter

#### Inherited from

[`IWaxFormatter`](./IWaxFormatter).[`options`](./IWaxFormatter#options)

#### Defined in

[wasm/lib/detailed/formatters/types.ts:152](https://gitlab.syncad.com/hive/wax/-/blob/8f4868a84978a3f8c750536f945a2a0ec7470397/ts/wasm/lib/detailed/formatters/types.ts#L152)

## Methods

### extend()

#### Call Signature

> **extend**(`formatterConstructor`, `options`?): [`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

Allows users to extend the default wax formatter using custom user-defined formatters with [WaxFormattable](../functions/WaxFormattable)

##### Parameters

###### formatterConstructor

[`TWaxCustomFormatterConstructor`](../type-aliases/TWaxCustomFormatterConstructor)

constructable formatter object

###### options?

`Partial`\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

formatter options

##### Returns

[`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

extended formatter class

##### Defined in

[wasm/lib/detailed/formatters/types.ts:176](https://gitlab.syncad.com/hive/wax/-/blob/8f4868a84978a3f8c750536f945a2a0ec7470397/ts/wasm/lib/detailed/formatters/types.ts#L176)

#### Call Signature

> **extend**(`options`?): [`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

Allows users to extend the default wax formatter using given options

##### Parameters

###### options?

`Partial`\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

formatter options

##### Returns

[`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

extended formatter class

##### Defined in

[wasm/lib/detailed/formatters/types.ts:184](https://gitlab.syncad.com/hive/wax/-/blob/8f4868a84978a3f8c750536f945a2a0ec7470397/ts/wasm/lib/detailed/formatters/types.ts#L184)

***

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

#### Inherited from

[`IWaxFormatter`](./IWaxFormatter).[`format`](./IWaxFormatter#format)

#### Defined in

[wasm/lib/detailed/formatters/types.ts:147](https://gitlab.syncad.com/hive/wax/-/blob/8f4868a84978a3f8c750536f945a2a0ec7470397/ts/wasm/lib/detailed/formatters/types.ts#L147)

***

### formatNumber()

> **formatNumber**(`amount`, `precision`?, `locales`?): `string`

Formats numbers in given format

#### Parameters

##### amount

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

number to be formatted

##### precision?

`number`

the exact precision of the given number (defaults to undefined - dynamic precision)

##### locales?

A string with a BCP 47 language, or an array of such locale identifiers (defaults to undefined - current locale)

`string` | `string`[]

#### Returns

`string`

formatted number

#### Defined in

[wasm/lib/detailed/formatters/types.ts:195](https://gitlab.syncad.com/hive/wax/-/blob/8f4868a84978a3f8c750536f945a2a0ec7470397/ts/wasm/lib/detailed/formatters/types.ts#L195)

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

#### Inherited from

[`IWaxFormatter`](./IWaxFormatter).[`waxify`](./IWaxFormatter#waxify)

#### Defined in

[wasm/lib/detailed/formatters/types.ts:133](https://gitlab.syncad.com/hive/wax/-/blob/8f4868a84978a3f8c750536f945a2a0ec7470397/ts/wasm/lib/detailed/formatters/types.ts#L133)
