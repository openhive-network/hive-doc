[@hiveio/wax](../globals) / witness\_set\_properties

# Interface: witness\_set\_properties

This is an operation for witnesses.
This is one of the two operations allowing to update witness properties (@see witness_update_operation).
The whole list of properties is available here:
https://gitlab.syncad.com/hive/hive/-/blob/master/doc/witness_parameters.md.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/42_witness_set_properties.md?ref_type=heads

## Properties

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

#### Param

#### Defined in

wasm/lib/proto/witness\_set\_properties.ts:24

***

### owner

> **owner**: `string`

#### Param

Witness account name.

#### Defined in

wasm/lib/proto/witness\_set\_properties.ts:16

***

### props

> **props**: `object`

#### Index Signature

 \[`key`: `string`\]: `string`

#### Param

There are the following properties available in the {props}:
                                     account_creation_fee, account_subsidy_budget, account_subsidy_decay,
                                     maximum_block_size, hbd_interest_rate. hbd_exchange_rate, url and new_signing_key.

#### Defined in

wasm/lib/proto/witness\_set\_properties.ts:22
