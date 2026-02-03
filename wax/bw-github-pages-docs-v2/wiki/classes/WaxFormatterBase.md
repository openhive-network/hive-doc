[@hiveio/wax](../globals) / WaxFormatterBase

# Class: `abstract` WaxFormatterBase

Classes implementing this interface denote that they are ready to handle tagged templates

## Extended by

- [`WaxFormatter`](./WaxFormatter)

## Implements

- [`IWaxFormatter`](../interfaces/IWaxFormatter)

## Constructors

### new WaxFormatterBase()

> **new WaxFormatterBase**(`options`?): [`WaxFormatterBase`](./WaxFormatterBase)

#### Parameters

##### options?

###### asset

\{`appendTokenName`: `boolean`;`displayAsNai`: `boolean`;`formatAmount`: `boolean`;`locales`: `string` \| (`undefined` \| `string`)[]; \}

###### asset.appendTokenName

`boolean`

Appends token name after asset amount (e.g. `1.100 HIVE`)

**Default**

```ts
true
```

###### asset.displayAsNai

`boolean`

Displays assets in NAI form instead of the human-readable form

**Default**

```ts
false
```

###### asset.formatAmount

`boolean`

Formats the output amount in human-readable format based on current localization settings of the user (e.g. `100'000'000.100 HIVE`)

**Default**

```ts
true
```

###### asset.locales

`string` \| (`undefined` \| `string`)[]

Locales to be used when formatting the amount of the asset (defaults to the currently used locale by the user)

**Default**

```ts
undefined
```

###### createDefaultFormatters

`boolean`

Initializes formatter class with default wax formatters

**Default**

```ts
true
```

###### transaction

\{`displayAsId`: `boolean`; \}

###### transaction.displayAsId

`boolean`

Displays transaction as its id (new format) instead of an object

**Default**

```ts
true
```

#### Returns

[`WaxFormatterBase`](./WaxFormatterBase)

#### Defined in

[wasm/lib/detailed/formatters/base.ts:19](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/formatters/base.ts#L19)

## Properties

### options

> `readonly` **options**: [`IWaxFormatterOptions`](../interfaces/IWaxFormatterOptions)

Options for the formatter

#### Implementation of

[`IWaxFormatter`](../interfaces/IWaxFormatter).[`options`](../interfaces/IWaxFormatter#options)

#### Defined in

[wasm/lib/detailed/formatters/base.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/formatters/base.ts#L17)

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

#### Implementation of

[`IWaxFormatter`](../interfaces/IWaxFormatter).[`format`](../interfaces/IWaxFormatter#format)

#### Defined in

[wasm/lib/detailed/formatters/base.ts:72](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/formatters/base.ts#L72)

***

### handleProperty()

> `abstract` `protected` **handleProperty**(`source`, `target`, `property`): `any`

#### Parameters

##### source

`object`

##### target

`any`

##### property

`string`

#### Returns

`any`

#### Defined in

[wasm/lib/detailed/formatters/base.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/formatters/base.ts#L27)

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

#### Implementation of

[`IWaxFormatter`](../interfaces/IWaxFormatter).[`waxify`](../interfaces/IWaxFormatter#waxify)

#### Defined in

[wasm/lib/detailed/formatters/base.ts:76](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/formatters/base.ts#L76)
