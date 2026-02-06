[@hiveio/wax](../globals) / TFormatFunction

# Type Alias: TFormatFunction()\<T\>

> **TFormatFunction**\<`T`\>: (`args`) => `string` \| `any`

Formatter function that receives input value for the matched property and returns the formatted output
Remember that this function takes two arguments. The first one is for data parsing, e.g. for transactions
parsing using [["createTransactionFromJson"]](../interfaces/ITransaction.md). That data should maintain immutable.

The second argument is the target working argument which should be returned from the formatter function
if your options specify to ignore given formatting.

## Type Parameters

• **T** = `object`

## Parameters

### args

[`IFormatFunctionArguments`](../interfaces/IFormatFunctionArguments)\<`T`\>

formatter function arguments

## Returns

`string` \| `any`

desired formatted output data

## Example

```typescript
;@WaxFormattable({ matchProperty: "operations" })
public transactionFormatter(source: DeepReadonly<ApiTransaction>, target: object): string | object {
  if(!this.options.transaction.displayAsId)
    return target;

  const { id } = this.wax.Transaction.fromApi(source);

  return id;
}
```

## Defined in

[wasm/lib/detailed/formatters/types.ts:114](https://gitlab.syncad.com/hive/wax/-/blob/fd756288e9a34740db6a53e19d17ae5e94b49e4a/ts/wasm/lib/detailed/formatters/types.ts#L114)
