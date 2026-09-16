[@hiveio/wax](../globals) / feed\_publish

# Interface: feed\_publish

This is an operation for witnesses.
The witnesses publish the exchange rate between Hive and HBD.
Only the exchange rate published by the top 20 witnesses is used to define the exchange rate.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/07_feed_publish.md?ref_type=heads

## Properties

### exchange\_rate

> **exchange\_rate**: `undefined` \| [`price`](./price)

#### Param

How many HBD the 1 Hive should cost
                               Example: "base":"0.345 HBD","quote":"1.000 HIVE"

#### Defined in

wasm/lib/proto/feed\_publish.ts:20

***

### publisher

> **publisher**: `string`

#### Param

The witness.

#### Defined in

wasm/lib/proto/feed\_publish.ts:15
