[@hiveio/wax](../globals) / consolidate\_treasury\_balance

# Interface: consolidate\_treasury\_balance

Related to block processing.
Generated during block processing potentially every block, but only if there is nonzero transfer. Transfer occurs
if there are assets on OBSOLETE_TREASURY_ACCOUNT ('steem.dao'). They are consolidated from all balances (per asset
type) and moved to NEW_HIVE_TREASURY_ACCOUNT ('hive.fund').

## Properties

### total\_moved

> **total\_moved**: [`asset`](./asset)[]

#### Param

(HIVE, VESTS or HBD) funds moved from old to new treasury

#### Defined in

wasm/lib/proto/consolidate\_treasury\_balance.ts:14
