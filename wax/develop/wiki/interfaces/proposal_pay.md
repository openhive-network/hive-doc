[@hiveio/wax](../globals) / proposal\_pay

# Interface: proposal\_pay

Defined in: wasm/lib/proto/proposal\_pay.ts:11

Related to create_proposal_operation.
Generated during block processing during proposal maintenance in batches
for each proposal that is chosen and receives funding.

## Properties

### payer

> **payer**: `string`

Defined in: wasm/lib/proto/proposal\_pay.ts:17

#### Param

**payer**

treasury account, source of payment

***

### payment

> **payment**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/proposal\_pay.ts:19

#### Param

**payment**

(HBD) paid amount

***

### proposal\_id

> **proposal\_id**: `number`

Defined in: wasm/lib/proto/proposal\_pay.ts:13

#### Param

**proposal\_id**

id of chosen proposal

***

### receiver

> **receiver**: `string`

Defined in: wasm/lib/proto/proposal\_pay.ts:15

#### Param

**receiver**

account designated to receive funding (receiver of payment)
