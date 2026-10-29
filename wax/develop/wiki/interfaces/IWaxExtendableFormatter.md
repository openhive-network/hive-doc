[@hiveio/wax](../globals) / IWaxExtendableFormatter

# Interface: IWaxExtendableFormatter

Defined in: [wasm/lib/detailed/formatters/types.ts:168](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L168)

Classes implementing this interface denote that they are ready to handle tagged templates

## Extends

- [`IWaxFormatter`](./IWaxFormatter)

## Properties

### options

> `readonly` **options**: [`DeepReadonly`](../type-aliases/DeepReadonly)\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

Defined in: [wasm/lib/detailed/formatters/types.ts:152](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L152)

Options for the formatter

#### Inherited from

[`IWaxFormatter`](./IWaxFormatter).[`options`](./IWaxFormatter#options)

## Methods

### extend()

#### Call Signature

> **extend**(`formatterConstructor`, `options?`): `IWaxExtendableFormatter`

Defined in: [wasm/lib/detailed/formatters/types.ts:176](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L176)

Allows users to extend the default wax formatter using custom user-defined formatters with [WaxFormattable](../functions/WaxFormattable)

##### Parameters

###### formatterConstructor

[`TWaxCustomFormatterConstructor`](../type-aliases/TWaxCustomFormatterConstructor)

constructable formatter object

###### options?

`Partial`\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

formatter options

##### Returns

`IWaxExtendableFormatter`

extended formatter class

#### Call Signature

> **extend**(`options?`): `IWaxExtendableFormatter`

Defined in: [wasm/lib/detailed/formatters/types.ts:184](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L184)

Allows users to extend the default wax formatter using given options

##### Parameters

###### options?

`Partial`\<[`IWaxFormatterOptions`](./IWaxFormatterOptions)\>

formatter options

##### Returns

`IWaxExtendableFormatter`

extended formatter class

***

### format()

> **format**\<`I`, `R`\>(`data`): `R`

Defined in: [wasm/lib/detailed/formatters/types.ts:147](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L147)

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

#### Inherited from

[`IWaxFormatter`](./IWaxFormatter).[`format`](./IWaxFormatter#format)

***

### formatNumber()

> **formatNumber**(`amount`, `precision?`, `locales?`): `string`

Defined in: [wasm/lib/detailed/formatters/types.ts:195](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L195)

Formats numbers in given format

#### Parameters

##### amount

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

number to be formatted

##### precision?

`number`

the exact precision of the given number (defaults to undefined - dynamic precision)

##### locales?

`string` \| `string`[]

A string with a BCP 47 language, or an array of such locale identifiers (defaults to undefined - current locale)

#### Returns

`string`

formatted number

***

### waxify()

> **waxify**(`strings`, ...`args`): `string`

Defined in: [wasm/lib/detailed/formatters/types.ts:133](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L133)

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

#### Inherited from

[`IWaxFormatter`](./IWaxFormatter).[`waxify`](./IWaxFormatter#waxify)
