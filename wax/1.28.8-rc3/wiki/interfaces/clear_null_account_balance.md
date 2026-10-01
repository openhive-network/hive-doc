[@hiveio/wax](../globals) / clear\_null\_account\_balance

# Interface: clear\_null\_account\_balance

Related to block processing.
Generated during block processing potentially every block, but only if nonzero assets were burned. Triggered by removal of all
assets from 'null' account balances.

## Properties

### total\_cleared

> **total\_cleared**: [`asset`](./asset)[]

#### Param

(HIVE, VESTS or HBD) nonzero assets burned on 'null' account

#### Defined in

wasm/lib/proto/clear\_null\_account\_balance.ts:13
