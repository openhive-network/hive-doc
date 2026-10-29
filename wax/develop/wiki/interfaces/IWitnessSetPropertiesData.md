[@hiveio/wax](../globals) / IWitnessSetPropertiesData

# Interface: IWitnessSetPropertiesData

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:10](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L10)

## Properties

### accountCreationFee?

> `optional` **accountCreationFee?**: [`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:26](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L26)

The account creation fee.

***

### accountSubsidyBudget?

> `optional` **accountSubsidyBudget?**: `number`

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:46](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L46)

The account subsidy budget.

***

### accountSubsidyDecay?

> `optional` **accountSubsidyDecay?**: `number`

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:50](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L50)

The account subsidy decay.

***

### hbdExchangeRate?

> `optional` **hbdExchangeRate?**: `object`

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L34)

The HBD exchange rate.

#### base

> **base**: [`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

#### quote

> **quote**: [`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

***

### hbdInterestRate?

> `optional` **hbdInterestRate?**: `number`

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:42](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L42)

The HBD interest rate.

***

### maximumBlockSize?

> `optional` **maximumBlockSize?**: `number`

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L38)

The maximum block size.

***

### newSigningKey?

> `optional` **newSigningKey?**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L22)

The new signing key of the witness.

***

### owner

> **owner**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L14)

Witness account name.

***

### url?

> `optional` **url?**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:30](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L30)

The URL of the witness.

***

### witnessSigningKey

> **witnessSigningKey**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/witness\_set\_properties.ts:18](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/witness_set_properties.ts#L18)

The public key of the witness.
