[@hiveio/wax](../globals) / witness\_update

# Interface: witness\_update

Defined in: wasm/lib/proto/witness\_update.ts:16

The operation witness_update_operation may be used to become a new witness or to update witness properties.
There are two operations that allow to update witness properties witness_update_operation and witness_set_properties_operation.
In order to update witness properties it is recommended to use witness_set_properties_operation.

If a user wants to become a witness, the operation witness_update_operation should be created.
If the witness doesn't want to be a witness any more, the operation witness_update_operation with empty { block_signing_key }
should be created.

## Properties

### block\_signing\_key

> **block\_signing\_key**: `string`

Defined in: wasm/lib/proto/witness\_update.ts:22

#### Param

**block\_signing\_key**

Public block signing key.

***

### fee

> **fee**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/witness\_update.ts:31

#### Param

**fee**

The asset is validated (the format should be correct and should be expressed in Hive),
                     but the fee is currently ignored.

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/witness\_update.ts:18

#### Param

**owner**

The witness who wants to update properties or a user who wants to become a witness.

***

### props

> **props**: [`legacy_chain_properties`](./legacy_chain_properties) \| `undefined`

Defined in: wasm/lib/proto/witness\_update.ts:24

#### Param

**props**

***

### url

> **url**: `string`

Defined in: wasm/lib/proto/witness\_update.ts:20

#### Param

**url**

url to information about witness.
