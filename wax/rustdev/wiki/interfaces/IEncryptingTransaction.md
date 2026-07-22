[@hiveio/wax](../globals) / IEncryptingTransaction

# Interface: IEncryptingTransaction\<StopEncryptResult\>

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

• **StopEncryptResult** *extends* [`ITransactionBase`](./ITransactionBase)

## Methods

### stopEncrypt()

> **stopEncrypt**(): `StopEncryptResult`

Stops encryption chain

Note: This call is optional if you are not going to push any other decrypted operations

#### Returns

`StopEncryptResult`

current transaction instance

#### Defined in

[wasm/lib/detailed/interfaces.ts:535](https://gitlab.syncad.com/hive/wax/-/blob/4dc0107e114c9130a129f46c06f31300a30477e4/ts/wasm/lib/detailed/interfaces.ts#L535)
