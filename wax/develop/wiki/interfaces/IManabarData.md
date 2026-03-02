[@hiveio/wax](../globals) / IManabarData

# Interface: IManabarData

## Properties

### current

> **current**: `bigint`

Current manabar value

#### Defined in

[wasm/lib/detailed/interfaces.ts:81](https://gitlab.syncad.com/hive/wax/-/blob/bcf25065a2448e046a140eba3f1afc6bc46c42c4/ts/wasm/lib/detailed/interfaces.ts#L81)

***

### max

> **max**: `bigint`

Maximum manabar value

#### Defined in

[wasm/lib/detailed/interfaces.ts:88](https://gitlab.syncad.com/hive/wax/-/blob/bcf25065a2448e046a140eba3f1afc6bc46c42c4/ts/wasm/lib/detailed/interfaces.ts#L88)

***

### percent

> **percent**: `number`

Percent of manabar load with two digits of precision, safely calculated based on the [current](./IManabarData#current) and [max](./IManabarData#max) values

#### Defined in

[wasm/lib/detailed/interfaces.ts:95](https://gitlab.syncad.com/hive/wax/-/blob/bcf25065a2448e046a140eba3f1afc6bc46c42c4/ts/wasm/lib/detailed/interfaces.ts#L95)
