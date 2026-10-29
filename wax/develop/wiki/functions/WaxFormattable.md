[@hiveio/wax](../globals) / WaxFormattable

# Function: WaxFormattable()

> **WaxFormattable**(`options?`): [`TWaxFormatterDecorator`](../type-aliases/TWaxFormatterDecorator)

Defined in: [wasm/lib/detailed/decorators/formatters.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/decorators/formatters.ts#L54)

When used on method, marks that this method is intended to be used for wax formatting with given property matching.
When no options provided, method name is used for property matching

## Parameters

### options?

`string` \| [`IWaxFormatterDecoratorOptions`](../interfaces/IWaxFormatterDecoratorOptions)\<`any`\>

property to match or decorator options

## Returns

[`TWaxFormatterDecorator`](../type-aliases/TWaxFormatterDecorator)

## Example

**Simple wax decorator usage**

```typescript
;@WaxFormattable()
public prop(value: Date): string {
  return value.toString();
}
```
