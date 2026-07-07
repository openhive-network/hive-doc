[@hiveio/wax](../globals) / proposal\_fee

# Interface: proposal\_fee

Related to create_proposal_operation.
Generated every time above operation is executed. Supplements it with paid fee.

## Properties

### creator

> **creator**: `string`

#### Param

user that created proposal (source of fee)

#### Defined in

wasm/lib/proto/proposal\_fee.ts:12

***

### fee

> **fee**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) amount paid for proposal [should actually be part of create_proposal_operation but it's too late now]

#### Defined in

wasm/lib/proto/proposal\_fee.ts:18

***

### proposal\_id

> **proposal\_id**: `number`

#### Param

id of proposal

#### Defined in

wasm/lib/proto/proposal\_fee.ts:16

***

### treasury

> **treasury**: `string`

#### Param

treasury account (receiver of fee)

#### Defined in

wasm/lib/proto/proposal\_fee.ts:14
