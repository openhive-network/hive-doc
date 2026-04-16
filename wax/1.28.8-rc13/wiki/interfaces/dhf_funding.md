[@hiveio/wax](../globals) / dhf\_funding

# Interface: dhf\_funding

Related to block processing.
Generated during block processing every proposal maintenance period.
Note: while the fund receives part of inflation every block, the amount is recorded aside and only when there are
proposal payouts (when new funds matter), there is generation of this vop.

## Properties

### additional\_funds

> **additional\_funds**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) portion inflation accumulated since previous maintenance period

#### Defined in

wasm/lib/proto/dhf\_funding.ts:16

***

### treasury

> **treasury**: `string`

#### Param

treasury account (receiver of additional_funds)

#### Defined in

wasm/lib/proto/dhf\_funding.ts:14
