[@hiveio/wax](../globals) / proposal\_fee

# Interface: proposal\_fee

Defined in: wasm/lib/proto/proposal\_fee.ts:10

Related to create_proposal_operation.
Generated every time above operation is executed. Supplements it with paid fee.

## Properties

### creator

> **creator**: `string`

Defined in: wasm/lib/proto/proposal\_fee.ts:12

#### Param

**creator**

user that created proposal (source of fee)

***

### fee

> **fee**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/proposal\_fee.ts:18

#### Param

**fee**

(HBD) amount paid for proposal [should actually be part of create_proposal_operation but it's too late now]

***

### proposal\_id

> **proposal\_id**: `number`

Defined in: wasm/lib/proto/proposal\_fee.ts:16

#### Param

**proposal\_id**

id of proposal

***

### treasury

> **treasury**: `string`

Defined in: wasm/lib/proto/proposal\_fee.ts:14

#### Param

**treasury**

treasury account (receiver of fee)
