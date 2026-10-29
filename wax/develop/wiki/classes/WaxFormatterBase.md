[@hiveio/wax](../globals) / WaxFormatterBase

# Abstract Class: WaxFormatterBase

Defined in: [wasm/lib/detailed/formatters/base.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/base.ts#L16)

Classes implementing this interface denote that they are ready to handle tagged templates

## Extended by

- [`WaxFormatter`](../interfaces/WaxFormatter)

## Implements

- [`IWaxFormatter`](../interfaces/IWaxFormatter)

## Constructors

### Constructor

> **new WaxFormatterBase**(`options?`): `WaxFormatterBase`

Defined in: [wasm/lib/detailed/formatters/base.ts:19](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/base.ts#L19)

#### Parameters

##### options?

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

`WaxFormatterBase`

## Properties

### options

> `readonly` **options**: [`IWaxFormatterOptions`](../interfaces/IWaxFormatterOptions)

Defined in: [wasm/lib/detailed/formatters/base.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/base.ts#L17)

Options for the formatter

#### Implementation of

[`IWaxFormatter`](../interfaces/IWaxFormatter).[`options`](../interfaces/IWaxFormatter#options)

## Methods

### format()

> **format**\<`I`, `R`\>(`data`): `R`

Defined in: [wasm/lib/detailed/formatters/base.ts:72](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/base.ts#L72)

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

[`IWaxFormatter`](../interfaces/IWaxFormatter).[`format`](../interfaces/IWaxFormatter#format)

***

### handleProperty()

> `abstract` `protected` **handleProperty**(`source`, `target`, `property`): `any`

Defined in: [wasm/lib/detailed/formatters/base.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/base.ts#L27)

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

### waxify()

> **waxify**(`strings`, ...`args`): `string`

Defined in: [wasm/lib/detailed/formatters/base.ts:76](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/formatters/base.ts#L76)

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

[`IWaxFormatter`](../interfaces/IWaxFormatter).[`waxify`](../interfaces/IWaxFormatter#waxify)
