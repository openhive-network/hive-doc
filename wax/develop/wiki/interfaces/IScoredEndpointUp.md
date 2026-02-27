[@hiveio/wax](../globals) / IScoredEndpointUp

# Interface: IScoredEndpointUp

## Extends

- [`IHiveEndpointDataBase`](./IHiveEndpointDataBase)

## Properties

### endpointUrl

> **endpointUrl**: `string`

#### Inherited from

[`IHiveEndpointDataBase`](./IHiveEndpointDataBase).[`endpointUrl`](./IHiveEndpointDataBase#endpointurl)

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:65](https://gitlab.syncad.com/hive/wax/-/blob/15396aaf2f1d502cfb459bf2d76f175f28fc2dbb/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L65)

***

### latencies

> **latencies**: `number`[]

Note: Latencies are listed in a way that the last element is the newest in history

#### Defined in

[wasm/lib/detailed/healthchecker/healthchecker.ts:18](https://gitlab.syncad.com/hive/wax/-/blob/15396aaf2f1d502cfb459bf2d76f175f28fc2dbb/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L18)

***

### score

> **score**: `number`

#### Defined in

[wasm/lib/detailed/healthchecker/healthchecker.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/15396aaf2f1d502cfb459bf2d76f175f28fc2dbb/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L14)

***

### up

> **up**: `true`

#### Defined in

[wasm/lib/detailed/healthchecker/healthchecker.ts:19](https://gitlab.syncad.com/hive/wax/-/blob/15396aaf2f1d502cfb459bf2d76f175f28fc2dbb/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L19)
