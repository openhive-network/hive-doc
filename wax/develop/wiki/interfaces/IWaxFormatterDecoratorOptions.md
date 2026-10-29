[@hiveio/wax](../globals) / IWaxFormatterDecoratorOptions

# Interface: IWaxFormatterDecoratorOptions\<T\>

Defined in: [wasm/lib/detailed/decorators/formatters.ts:3](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/decorators/formatters.ts#L3)

## Type Parameters

### T

`T` = `any`

## Properties

### matchInstanceOf?

> `optional` **matchInstanceOf?**: (...`args`) => `T`

Defined in: [wasm/lib/detailed/decorators/formatters.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/decorators/formatters.ts#L34)

Matches instance of a given class

#### Parameters

##### args

...`any`[]

#### Returns

`T`

***

### matchProperty?

> `optional` **matchProperty?**: `string`

Defined in: [wasm/lib/detailed/decorators/formatters.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/decorators/formatters.ts#L9)

Property to match. If not specified defaults to the formatter method name

***

### matchValue?

> `optional` **matchValue?**: `any`

Defined in: [wasm/lib/detailed/decorators/formatters.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/decorators/formatters.ts#L17)

Optional value to match on the property.
Note: uses strict equality for value checking (`===`)

***

### requireDefined?

> `optional` **requireDefined?**: `boolean`

Defined in: [wasm/lib/detailed/decorators/formatters.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/decorators/formatters.ts#L27)

Optional value to require property value to be defined (!== undefined)

Note: Does not work with [matchInstanceOf](./#matchinstanceof)

#### Default

```ts
false
```
