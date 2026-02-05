[@hiveio/wax](../globals) / IWaxFormatterOptions

# Interface: IWaxFormatterOptions

## Properties

### asset

> **asset**: `object`

#### appendTokenName

> **appendTokenName**: `boolean`

Appends token name after asset amount (e.g. `1.100 HIVE`)

##### Default

```ts
true
```

#### displayAsNai

> **displayAsNai**: `boolean`

Displays assets in NAI form instead of the human-readable form

##### Default

```ts
false
```

#### formatAmount

> **formatAmount**: `boolean`

Formats the output amount in human-readable format based on current localization settings of the user (e.g. `100'000'000.100 HIVE`)

##### Default

```ts
true
```

#### locales?

> `optional` **locales**: `string` \| `string`[]

Locales to be used when formatting the amount of the asset (defaults to the currently used locale by the user)

##### Default

```ts
undefined
```

#### Defined in

[wasm/lib/detailed/formatters/types.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/8ad2b63c881a2d911b31e0c06383e6fc0fe73d22/ts/wasm/lib/detailed/formatters/types.ts#L22)

***

### createDefaultFormatters

> **createDefaultFormatters**: `boolean`

Initializes formatter class with default wax formatters

#### Default

```ts
true
```

#### Defined in

[wasm/lib/detailed/formatters/types.ts:61](https://gitlab.syncad.com/hive/wax/-/blob/8ad2b63c881a2d911b31e0c06383e6fc0fe73d22/ts/wasm/lib/detailed/formatters/types.ts#L61)

***

### transaction

> **transaction**: `object`

#### displayAsId

> **displayAsId**: `boolean`

Displays transaction as its id (new format) instead of an object

##### Default

```ts
true
```

#### Defined in

[wasm/lib/detailed/formatters/types.ts:48](https://gitlab.syncad.com/hive/wax/-/blob/8ad2b63c881a2d911b31e0c06383e6fc0fe73d22/ts/wasm/lib/detailed/formatters/types.ts#L48)
