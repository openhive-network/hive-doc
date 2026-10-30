[@hiveio/wax](../globals) / WaxFormatter

# Interface: WaxFormatter

Defined in: [wasm/lib/detailed/formatters/waxify.ts:21](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/formatters/waxify.ts#L21)

Classes implementing this interface denote that they are ready to handle tagged templates

## Extends

- [`WaxFormatterBase`](../classes/WaxFormatterBase)

## Implements

- [`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

## Properties

### options

> `readonly` **options**: [`IWaxFormatterOptions`](./IWaxFormatterOptions)

Defined in: [wasm/lib/detailed/formatters/base.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/formatters/base.ts#L17)

Options for the formatter

#### Implementation of

`IWaxExtendableFormatter.options`

#### Inherited from

[`WaxFormatterBase`](../classes/WaxFormatterBase).[`options`](../classes/WaxFormatterBase#options)

***

### wax

> `protected` `readonly` **wax**: [`IWaxBaseInterface`](./IWaxBaseInterface)

Defined in: [wasm/lib/detailed/formatters/waxify.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/formatters/waxify.ts#L25)

## Methods

### extend()

> **extend**(`formatterConstructor`, `options?`): `WaxFormatter`

Defined in: [wasm/lib/detailed/formatters/waxify.ts:87](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/formatters/waxify.ts#L87)

Allows users to extend the default wax formatter using custom user-defined formatters with [WaxFormattable](../functions/WaxFormattable)

#### Parameters

##### formatterConstructor

[`TWaxCustomFormatterConstructor`](../type-aliases/TWaxCustomFormatterConstructor) \| \{ `asset?`: \{ `appendTokenName?`: `boolean`; `displayAsNai?`: `boolean`; `formatAmount?`: `boolean`; `locales?`: `string` \| (`string` \| `undefined`)[]; \}; `createDefaultFormatters?`: `boolean`; `transaction?`: \{ `displayAsId?`: `boolean`; \}; \}

constructable formatter object

[`TWaxCustomFormatterConstructor`](../type-aliases/TWaxCustomFormatterConstructor)

***

###### Type Literal

\{ `asset?`: \{ `appendTokenName?`: `boolean`; `displayAsNai?`: `boolean`; `formatAmount?`: `boolean`; `locales?`: `string` \| (`string` \| `undefined`)[]; \}; `createDefaultFormatters?`: `boolean`; `transaction?`: \{ `displayAsId?`: `boolean`; \}; \}

constructable formatter object

###### asset?

\{ `appendTokenName?`: `boolean`; `displayAsNai?`: `boolean`; `formatAmount?`: `boolean`; `locales?`: `string` \| (`string` \| `undefined`)[]; \}

###### asset.appendTokenName?

`boolean`

Appends token name after asset amount (e.g. `1.100 HIVE`)

**Default**

```ts
true
```

###### asset.displayAsNai?

`boolean`

Displays assets in NAI form instead of the human-readable form

**Default**

```ts
false
```

###### asset.formatAmount?

`boolean`

Formats the output amount in human-readable format based on current localization settings of the user (e.g. `100'000'000.100 HIVE`)

**Default**

```ts
true
```

###### asset.locales?

`string` \| (`string` \| `undefined`)[]

Locales to be used when formatting the amount of the asset (defaults to the currently used locale by the user)

**Default**

```ts
undefined
```

###### createDefaultFormatters?

`boolean`

Initializes formatter class with default wax formatters

**Default**

```ts
true
```

###### transaction?

\{ `displayAsId?`: `boolean`; \}

###### transaction.displayAsId?

`boolean`

Displays transaction as its id (new format) instead of an object

**Default**

```ts
true
```

##### options?

formatter options

###### asset?

\{ `appendTokenName?`: `boolean`; `displayAsNai?`: `boolean`; `formatAmount?`: `boolean`; `locales?`: `string` \| (`string` \| `undefined`)[]; \}

###### asset.appendTokenName?

`boolean`

Appends token name after asset amount (e.g. `1.100 HIVE`)

**Default**

```ts
true
```

###### asset.displayAsNai?

`boolean`

Displays assets in NAI form instead of the human-readable form

**Default**

```ts
false
```

###### asset.formatAmount?

`boolean`

Formats the output amount in human-readable format based on current localization settings of the user (e.g. `100'000'000.100 HIVE`)

**Default**

```ts
true
```

###### asset.locales?

`string` \| (`string` \| `undefined`)[]

Locales to be used when formatting the amount of the asset (defaults to the currently used locale by the user)

**Default**

```ts
undefined
```

###### createDefaultFormatters?

`boolean`

Initializes formatter class with default wax formatters

**Default**

```ts
true
```

###### transaction?

\{ `displayAsId?`: `boolean`; \}

###### transaction.displayAsId?

`boolean`

Displays transaction as its id (new format) instead of an object

**Default**

```ts
true
```

#### Returns

`WaxFormatter`

extended formatter class

#### Implementation of

`IWaxExtendableFormatter.extend`

***

### format()

> **format**\<`I`, `R`\>(`data`): `R`

Defined in: [wasm/lib/detailed/formatters/base.ts:72](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/formatters/base.ts#L72)

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

#### Implementation of

`IWaxExtendableFormatter.format`

#### Inherited from

[`WaxFormatterBase`](../classes/WaxFormatterBase).[`format`](../classes/WaxFormatterBase#format)

***

### formatNumber()

> **formatNumber**(`amount`, `precision?`, `locales?`): `string`

Defined in: [wasm/lib/detailed/formatters/waxify.ts:60](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/formatters/waxify.ts#L60)

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

#### Implementation of

`IWaxExtendableFormatter.formatNumber`

***

### handleInstanceOf()

> `protected` **handleInstanceOf**(`source`, `target`, `property`): `any`

Defined in: [wasm/lib/detailed/formatters/waxify.ts:152](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/formatters/waxify.ts#L152)

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

***

### handleProperty()

> `protected` **handleProperty**(`source`, `target`, `property`): `any`

Defined in: [wasm/lib/detailed/formatters/waxify.ts:171](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/formatters/waxify.ts#L171)

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

[`WaxFormatterBase`](../classes/WaxFormatterBase).[`handleProperty`](../classes/WaxFormatterBase#handleproperty)

***

### waxify()

> **waxify**(`strings`, ...`args`): `string`

Defined in: [wasm/lib/detailed/formatters/base.ts:76](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/formatters/base.ts#L76)

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

#### Implementation of

`IWaxExtendableFormatter.waxify`

#### Inherited from

[`WaxFormatterBase`](../classes/WaxFormatterBase).[`waxify`](../classes/WaxFormatterBase#waxify)
