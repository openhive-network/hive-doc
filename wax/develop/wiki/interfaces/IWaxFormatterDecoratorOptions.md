[@hiveio/wax](../globals) / IWaxFormatterDecoratorOptions

# Interface: IWaxFormatterDecoratorOptions\<T\>

## Type Parameters

• **T** = `any`

## Properties

### matchInstanceOf()?

> `optional` **matchInstanceOf**: (...`args`) => `T`

Matches instance of a given class

#### Parameters

##### args

...`any`[]

#### Returns

`T`

#### Defined in

[wasm/lib/detailed/decorators/formatters.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/c69b0cd6f3a40872b17b06ad7d40b4f704a75376/ts/wasm/lib/detailed/decorators/formatters.ts#L34)

***

### matchProperty?

> `optional` **matchProperty**: `string`

Property to match. If not specified defaults to the formatter method name

#### Defined in

[wasm/lib/detailed/decorators/formatters.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/c69b0cd6f3a40872b17b06ad7d40b4f704a75376/ts/wasm/lib/detailed/decorators/formatters.ts#L9)

***

### matchValue?

> `optional` **matchValue**: `any`

Optional value to match on the property.
Note: uses strict equality for value checking (`===`)

#### Defined in

[wasm/lib/detailed/decorators/formatters.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/c69b0cd6f3a40872b17b06ad7d40b4f704a75376/ts/wasm/lib/detailed/decorators/formatters.ts#L17)

***

### requireDefined?

> `optional` **requireDefined**: `boolean`

Optional value to require property value to be defined (!== undefined)

Note: Does not work with [matchInstanceOf](./IWaxFormatterDecoratorOptions#matchinstanceof)

#### Default

```ts
false
```

#### Defined in

[wasm/lib/detailed/decorators/formatters.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/c69b0cd6f3a40872b17b06ad7d40b4f704a75376/ts/wasm/lib/detailed/decorators/formatters.ts#L27)
