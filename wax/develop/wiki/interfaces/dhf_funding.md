[@hiveio/wax](../globals) / dhf\_funding

# Interface: dhf\_funding

Defined in: wasm/lib/proto/dhf\_funding.ts:12

Related to block processing.
Generated during block processing every proposal maintenance period.
Note: while the fund receives part of inflation every block, the amount is recorded aside and only when there are
proposal payouts (when new funds matter), there is generation of this vop.

## Properties

### additional\_funds

> **additional\_funds**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/dhf\_funding.ts:16

#### Param

**additional\_funds**

(HBD) portion inflation accumulated since previous maintenance period

***

### treasury

> **treasury**: `string`

Defined in: wasm/lib/proto/dhf\_funding.ts:14

#### Param

**treasury**

treasury account (receiver of additional_funds)
