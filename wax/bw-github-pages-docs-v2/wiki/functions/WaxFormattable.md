[@hiveio/wax](../globals) / WaxFormattable

# Function: WaxFormattable()

> **WaxFormattable**(`options`?): [`TWaxFormatterDecorator`](../type-aliases/TWaxFormatterDecorator)

When used on method, marks that this method is intended to be used for wax formatting with given property matching.
When no options provided, method name is used for property matching

## Parameters

### options?

property to match or decorator options

`string` | [`IWaxFormatterDecoratorOptions`](../interfaces/IWaxFormatterDecoratorOptions)\<`any`\>

## Returns

[`TWaxFormatterDecorator`](../type-aliases/TWaxFormatterDecorator)

## Example

```typescript
;@WaxFormattable()
public prop(value: Date): string {
  return value.toString();
}
```

## Defined in

[wasm/lib/detailed/decorators/formatters.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/2f0aa97c17fb0fa1f30220cb74fec9c62bf0cce9/ts/wasm/lib/detailed/decorators/formatters.ts#L54)
