[@hiveio/wax](../globals) / proposal\_pay

# Interface: proposal\_pay

Related to create_proposal_operation.
Generated during block processing during proposal maintenance in batches
for each proposal that is chosen and receives funding.

## Properties

### payer

> **payer**: `string`

#### Param

treasury account, source of payment

#### Defined in

wasm/lib/proto/proposal\_pay.ts:17

***

### payment

> **payment**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) paid amount

#### Defined in

wasm/lib/proto/proposal\_pay.ts:19

***

### proposal\_id

> **proposal\_id**: `number`

#### Param

id of chosen proposal

#### Defined in

wasm/lib/proto/proposal\_pay.ts:13

***

### receiver

> **receiver**: `string`

#### Param

account designated to receive funding (receiver of payment)

#### Defined in

wasm/lib/proto/proposal\_pay.ts:15
