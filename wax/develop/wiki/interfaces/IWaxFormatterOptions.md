[@hiveio/wax](../globals) / IWaxFormatterOptions

# Interface: IWaxFormatterOptions

Defined in: [wasm/lib/detailed/formatters/types.ts:21](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L21)

## Properties

### asset

> **asset**: `object`

Defined in: [wasm/lib/detailed/formatters/types.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L22)

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

> `optional` **locales?**: `string` \| `string`[]

Locales to be used when formatting the amount of the asset (defaults to the currently used locale by the user)

##### Default

```ts
undefined
```

***

### createDefaultFormatters

> **createDefaultFormatters**: `boolean`

Defined in: [wasm/lib/detailed/formatters/types.ts:61](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L61)

Initializes formatter class with default wax formatters

#### Default

```ts
true
```

***

### transaction

> **transaction**: `object`

Defined in: [wasm/lib/detailed/formatters/types.ts:48](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/formatters/types.ts#L48)

#### displayAsId

> **displayAsId**: `boolean`

Displays transaction as its id (new format) instead of an object

##### Default

```ts
true
```
