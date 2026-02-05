[@hiveio/wax](../globals) / shutdown\_witness

# Interface: shutdown\_witness

Related to block processing.
Generated during block processing when witness is removed from active witnesses after it was detected he have missed
all blocks scheduled for him for last day. No longer active after HF20.

## See

producer_missed_operation

## Properties

### owner

> **owner**: `string`

#### Param

witness that was shut down

#### Defined in

wasm/lib/proto/shutdown\_witness.ts:13
