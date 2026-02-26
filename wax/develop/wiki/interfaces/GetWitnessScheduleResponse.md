[@hiveio/wax](../globals) / GetWitnessScheduleResponse

# Interface: GetWitnessScheduleResponse

## Properties

### account\_subsidy\_rd

> **account\_subsidy\_rd**: `object`

#### budget\_per\_time\_unit

> **budget\_per\_time\_unit**: `number`

#### decay\_params

> **decay\_params**: `object`

##### decay\_params.decay\_per\_time\_unit

> **decay\_per\_time\_unit**: `number`

##### decay\_params.decay\_per\_time\_unit\_denom\_shift

> **decay\_per\_time\_unit\_denom\_shift**: `number`

#### max\_pool\_size

> **max\_pool\_size**: `number`

#### min\_decay

> **min\_decay**: `number`

#### pool\_eq

> **pool\_eq**: `number`

#### resource\_unit

> **resource\_unit**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L27)

***

### account\_subsidy\_witness\_rd

> **account\_subsidy\_witness\_rd**: `object`

#### budget\_per\_time\_unit

> **budget\_per\_time\_unit**: `number`

#### decay\_params

> **decay\_params**: `object`

##### decay\_params.decay\_per\_time\_unit

> **decay\_per\_time\_unit**: `number`

##### decay\_params.decay\_per\_time\_unit\_denom\_shift

> **decay\_per\_time\_unit\_denom\_shift**: `number`

#### max\_pool\_size

> **max\_pool\_size**: `number`

#### min\_decay

> **min\_decay**: `number`

#### pool\_eq

> **pool\_eq**: `number`

#### resource\_unit

> **resource\_unit**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L38)

***

### current\_shuffled\_witnesses

> **current\_shuffled\_witnesses**: `string`[]

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L9)

***

### current\_virtual\_time

> **current\_virtual\_time**: `string`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:7](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L7)

***

### elected\_weight

> **elected\_weight**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:11](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L11)

***

### hardfork\_required\_witnesses

> **hardfork\_required\_witnesses**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:26](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L26)

***

### id

> **id**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:6](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L6)

***

### majority\_version

> **majority\_version**: `string`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L22)

***

### max\_miner\_witnesses

> **max\_miner\_witnesses**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:24](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L24)

***

### max\_runner\_witnesses

> **max\_runner\_witnesses**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L25)

***

### max\_voted\_witnesses

> **max\_voted\_witnesses**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:23](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L23)

***

### median\_props

> **median\_props**: `object`

#### account\_creation\_fee

> **account\_creation\_fee**: [`NaiAsset`](./NaiAsset)

#### account\_subsidy\_budget

> **account\_subsidy\_budget**: `number`

#### account\_subsidy\_decay

> **account\_subsidy\_decay**: `number`

#### hbd\_interest\_rate

> **hbd\_interest\_rate**: `number`

#### maximum\_block\_size

> **maximum\_block\_size**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:15](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L15)

***

### min\_witness\_account\_subsidy\_decay

> **min\_witness\_account\_subsidy\_decay**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:49](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L49)

***

### miner\_weight

> **miner\_weight**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L13)

***

### next\_shuffle\_block\_num

> **next\_shuffle\_block\_num**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:8](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L8)

***

### num\_scheduled\_witnesses

> **num\_scheduled\_witnesses**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:10](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L10)

***

### timeshare\_weight

> **timeshare\_weight**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L12)

***

### witness\_pay\_normalization\_factor

> **witness\_pay\_normalization\_factor**: `number`

#### Defined in

[wasm/lib/detailed/api/database\_api/get\_witness\_schedule.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/6d2b363a268310a39308191bcec492025211959a/ts/wasm/lib/detailed/api/database_api/get_witness_schedule.ts#L14)
