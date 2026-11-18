[@hiveio/wax](../globals) / IEncryptingTransaction

# Interface: IEncryptingTransaction\<StopEncryptResult\>

Defined in: [wasm/lib/detailed/interfaces.ts:542](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L542)

Same as [ITransaction](./ITransaction), but marks operations as encrypted using given keys, which will be encrypted upon
ITransaction.sign.

Note: We are not able to encrypt all operations.
We are currently supporting:
- Encryption of `body` in comment operation
- Encryption of `json` in custom_json operation
- Encryption of `memo` in transfer operation
- Encryption of `memo` in transfer_to_savings operation
- Encryption of `memo` in transfer_from_savings operation
- Encryption of `memo` in recurrent_transfer operation

## Example

**Base encrypting transaction usage**

```typescript
const tx = await waxFoundation.createTransaction();

tx.startEncrypt(myPublicKey).pushOperation({
   transfer: {
     amount: chain.hive(100),
     from_account: "gtg",
     to_account: "initminer",
     memo: "This should be encrypted"
   }
}).stopEncrypt();
```

## Type Parameters

### StopEncryptResult

`StopEncryptResult` *extends* [`ITransactionBase`](./ITransactionBase)

## Methods

### stopEncrypt()

> **stopEncrypt**(): `StopEncryptResult`

Defined in: [wasm/lib/detailed/interfaces.ts:550](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L550)

Stops encryption chain

Note: This call is optional if you are not going to push any other decrypted operations

#### Returns

`StopEncryptResult`

current transaction instance
