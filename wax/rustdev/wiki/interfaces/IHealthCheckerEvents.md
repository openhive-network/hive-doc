[@hiveio/wax](../globals) / IHealthCheckerEvents

# Interface: IHealthCheckerEvents

## Properties

### data()

> **data**: (`endpoints`) => `void` \| `Promise`\<`void`\>

#### Parameters

##### endpoints

[`TScoredEndpoint`](../type-aliases/TScoredEndpoint)[]

#### Returns

`void` \| `Promise`\<`void`\>

#### Defined in

[wasm/lib/detailed/healthchecker/healthchecker.ts:36](https://gitlab.syncad.com/hive/wax/-/blob/4dc0107e114c9130a129f46c06f31300a30477e4/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L36)

***

### error()

> **error**: (`error`) => `void` \| `Promise`\<`void`\>

#### Parameters

##### error

[`WaxHealthCheckerError`](../classes/WaxHealthCheckerError)

#### Returns

`void` \| `Promise`\<`void`\>

#### Defined in

[wasm/lib/detailed/healthchecker/healthchecker.ts:37](https://gitlab.syncad.com/hive/wax/-/blob/4dc0107e114c9130a129f46c06f31300a30477e4/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L37)

***

### newbest()

> **newbest**: (`endpoint`) => `void` \| `Promise`\<`void`\>

#### Parameters

##### endpoint

[`TScoredEndpoint`](../type-aliases/TScoredEndpoint)

#### Returns

`void` \| `Promise`\<`void`\>

#### Defined in

[wasm/lib/detailed/healthchecker/healthchecker.ts:33](https://gitlab.syncad.com/hive/wax/-/blob/4dc0107e114c9130a129f46c06f31300a30477e4/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L33)

***

### newdown()

> **newdown**: (`endpoint`) => `void` \| `Promise`\<`void`\>

#### Parameters

##### endpoint

[`TScoredEndpoint`](../type-aliases/TScoredEndpoint)

#### Returns

`void` \| `Promise`\<`void`\>

#### Defined in

[wasm/lib/detailed/healthchecker/healthchecker.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/4dc0107e114c9130a129f46c06f31300a30477e4/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L35)

***

### newup()

> **newup**: (`endpoint`) => `void` \| `Promise`\<`void`\>

#### Parameters

##### endpoint

[`TScoredEndpoint`](../type-aliases/TScoredEndpoint)

#### Returns

`void` \| `Promise`\<`void`\>

#### Defined in

[wasm/lib/detailed/healthchecker/healthchecker.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/4dc0107e114c9130a129f46c06f31300a30477e4/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L34)

***

### validationerror()

> **validationerror**: (`error`) => `void` \| `Promise`\<`void`\>

#### Parameters

##### error

[`WaxHealthCheckerValidatorFailedError`](../classes/WaxHealthCheckerValidatorFailedError)\<`string`\>

#### Returns

`void` \| `Promise`\<`void`\>

#### Defined in

[wasm/lib/detailed/healthchecker/healthchecker.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/4dc0107e114c9130a129f46c06f31300a30477e4/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L38)
