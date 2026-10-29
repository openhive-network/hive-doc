[@hiveio/wax](../globals) / IHealthCheckerEvents

# Interface: IHealthCheckerEvents

Defined in: [wasm/lib/detailed/healthchecker/healthchecker.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L32)

## Properties

### data

> **data**: (`endpoints`) => `void` \| `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/healthchecker/healthchecker.ts:36](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L36)

#### Parameters

##### endpoints

[`TScoredEndpoint`](../type-aliases/TScoredEndpoint)[]

#### Returns

`void` \| `Promise`\<`void`\>

***

### error

> **error**: (`error`) => `void` \| `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/healthchecker/healthchecker.ts:37](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L37)

#### Parameters

##### error

[`WaxHealthCheckerError`](../classes/WaxHealthCheckerError)

#### Returns

`void` \| `Promise`\<`void`\>

***

### newbest

> **newbest**: (`endpoint`) => `void` \| `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/healthchecker/healthchecker.ts:33](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L33)

#### Parameters

##### endpoint

[`TScoredEndpoint`](../type-aliases/TScoredEndpoint)

#### Returns

`void` \| `Promise`\<`void`\>

***

### newdown

> **newdown**: (`endpoint`) => `void` \| `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/healthchecker/healthchecker.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L35)

#### Parameters

##### endpoint

[`TScoredEndpoint`](../type-aliases/TScoredEndpoint)

#### Returns

`void` \| `Promise`\<`void`\>

***

### newup

> **newup**: (`endpoint`) => `void` \| `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/healthchecker/healthchecker.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L34)

#### Parameters

##### endpoint

[`TScoredEndpoint`](../type-aliases/TScoredEndpoint)

#### Returns

`void` \| `Promise`\<`void`\>

***

### validationerror

> **validationerror**: (`error`) => `void` \| `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/healthchecker/healthchecker.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/healthchecker.ts#L38)

#### Parameters

##### error

[`WaxHealthCheckerValidatorFailedError`](../classes/WaxHealthCheckerValidatorFailedError)

#### Returns

`void` \| `Promise`\<`void`\>
