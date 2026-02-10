[@hiveio/wax](../globals) / WaxFormatter

# Class: WaxFormatter

Classes implementing this interface denote that they are ready to handle tagged templates

## Extends

- [`WaxFormatterBase`](./WaxFormatterBase)

## Implements

- [`IWaxExtendableFormatter`](../interfaces/IWaxExtendableFormatter)

## Properties

### options

> `readonly` **options**: [`IWaxFormatterOptions`](../interfaces/IWaxFormatterOptions)

Options for the formatter

#### Implementation of

[`IWaxExtendableFormatter`](../interfaces/IWaxExtendableFormatter).[`options`](../interfaces/IWaxExtendableFormatter#options)

#### Inherited from

[`WaxFormatterBase`](./WaxFormatterBase).[`options`](./WaxFormatterBase#options)

#### Defined in

[wasm/lib/detailed/formatters/base.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/base.ts#L17)

***

### wax

> `protected` `readonly` **wax**: [`IWaxBaseInterface`](../interfaces/IWaxBaseInterface)

#### Defined in

[wasm/lib/detailed/formatters/waxify.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/waxify.ts#L25)

## Methods

### extend()

> **extend**(`formatterConstructor`, `options`?): [`WaxFormatter`](./WaxFormatter)

Allows users to extend the default wax formatter using custom user-defined formatters with [WaxFormattable](../functions/WaxFormattable)

#### Parameters

##### formatterConstructor

constructable formatter object

[`TWaxCustomFormatterConstructor`](../type-aliases/TWaxCustomFormatterConstructor) |

\{`asset`: \{`appendTokenName`: `boolean`;`displayAsNai`: `boolean`;`formatAmount`: `boolean`;`locales`: `string` \| (`undefined` \| `string`)[]; \};`createDefaultFormatters`: `boolean`;`transaction`: \{`displayAsId`: `boolean`; \}; \}

constructable formatter object

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

##### options?

formatter options

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

[`WaxFormatter`](./WaxFormatter)

extended formatter class

#### Implementation of

[`IWaxExtendableFormatter`](../interfaces/IWaxExtendableFormatter).[`extend`](../interfaces/IWaxExtendableFormatter#extend)

#### Defined in

[wasm/lib/detailed/formatters/waxify.ts:87](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/waxify.ts#L87)

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

#### Implementation of

[`IWaxExtendableFormatter`](../interfaces/IWaxExtendableFormatter).[`format`](../interfaces/IWaxExtendableFormatter#format)

#### Inherited from

[`WaxFormatterBase`](./WaxFormatterBase).[`format`](./WaxFormatterBase#format)

#### Defined in

[wasm/lib/detailed/formatters/base.ts:72](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/base.ts#L72)

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

#### Implementation of

[`IWaxExtendableFormatter`](../interfaces/IWaxExtendableFormatter).[`formatNumber`](../interfaces/IWaxExtendableFormatter#formatnumber)

#### Defined in

[wasm/lib/detailed/formatters/waxify.ts:60](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/waxify.ts#L60)

***

### handleInstanceOf()

> `protected` **handleInstanceOf**(`source`, `target`, `property`): `any`

**`Internal`**

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

[wasm/lib/detailed/formatters/waxify.ts:152](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/waxify.ts#L152)

***

### handleProperty()

> `protected` **handleProperty**(`source`, `target`, `property`): `any`

**`Internal`**

#### Parameters

##### source

`object`

##### target

`any`

##### property

`string`

#### Returns

`any`

#### Overrides

[`WaxFormatterBase`](./WaxFormatterBase).[`handleProperty`](./WaxFormatterBase#handleproperty)

#### Defined in

[wasm/lib/detailed/formatters/waxify.ts:171](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/waxify.ts#L171)

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

[`IWaxExtendableFormatter`](../interfaces/IWaxExtendableFormatter).[`waxify`](../interfaces/IWaxExtendableFormatter#waxify)

#### Inherited from

[`WaxFormatterBase`](./WaxFormatterBase).[`waxify`](./WaxFormatterBase#waxify)

#### Defined in

[wasm/lib/detailed/formatters/base.ts:76](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/base.ts#L76)

***

### create()

> `static` **create**(`wax`, `options`?): [`WaxFormatter`](./WaxFormatter)

#### Parameters

##### wax

[`IWaxBaseInterface`](../interfaces/IWaxBaseInterface)

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

[`WaxFormatter`](./WaxFormatter)

#### Defined in

[wasm/lib/detailed/formatters/waxify.ts:29](https://gitlab.syncad.com/hive/wax/-/blob/68db572d2ebdd2976b5087d2dfe4685e5857b850/ts/wasm/lib/detailed/formatters/waxify.ts#L29)
