[@hiveio/wax](../globals) / ASignatureProvider

# Abstract Class: ASignatureProvider

Defined in: [wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:7](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L7)

Helper class encapsulating transaction signing flow. Derived class must implement signature generation logic.

## Extended by

- [`AEncryptionProvider`](./AEncryptionProvider)

## Implements

- [`IOnlineSignatureProvider`](../interfaces/IOnlineSignatureProvider)

## Constructors

### Constructor

> **new ASignatureProvider**(): `ASignatureProvider`

#### Returns

`ASignatureProvider`

## Methods

### generateSignatures()

> `abstract` `protected` **generateSignatures**(`transaction`): `Promise`\<`string`[]\>

Defined in: [wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L17)

#### Parameters

##### transaction

[`ISignatureTransaction`](../interfaces/ISignatureTransaction)

#### Returns

`Promise`\<`string`[]\>

***

### signTransaction()

> **signTransaction**(`transaction`): `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:8](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L8)

Signs a transaction by signing a digest of the transaction

#### Parameters

##### transaction

[`ISignatureTransaction`](../interfaces/ISignatureTransaction)

transaction to be signed

#### Returns

`Promise`\<`void`\>

resolves when the wallet finished signing (signature(s) appended internally)

#### Implementation of

[`IOnlineSignatureProvider`](../interfaces/IOnlineSignatureProvider).[`signTransaction`](../interfaces/IOnlineSignatureProvider#signtransaction)
