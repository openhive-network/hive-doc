[@hiveio/workerbee](../globals) / TBlogContentProvided

# Type Alias: TBlogContentProvided\<TAccounts\>

> **TBlogContentProvided**\<`TAccounts`\> = \{ \[K in TAccounts\[number\]\]: IOperationTransactionPair\<comment\>\[\] \| WorkerBeeIterable\<IOperationTransactionPair\<comment\>\> \}

Defined in: [src/chain-observers/providers/blog-content-provider.ts:10](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/blog-content-provider.ts#L10)

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[]
