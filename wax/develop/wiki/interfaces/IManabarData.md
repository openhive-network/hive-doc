[@hiveio/wax](../globals) / IManabarData

# Interface: IManabarData

Defined in: [wasm/lib/detailed/interfaces.ts:75](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L75)

## Properties

### current

> **current**: `bigint`

Defined in: [wasm/lib/detailed/interfaces.ts:81](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L81)

Current manabar value

***

### max

> **max**: `bigint`

Defined in: [wasm/lib/detailed/interfaces.ts:88](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L88)

Maximum manabar value

***

### percent

> **percent**: `number`

Defined in: [wasm/lib/detailed/interfaces.ts:95](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L95)

Percent of manabar load with two digits of precision, safely calculated based on the [current](./#current) and [max](./#max) values
