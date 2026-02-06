[@hiveio/workerbee](../globals) / Observer

# Interface: Observer\<T\>

An object interface that defines a set of callback functions a user can use to get notified

## Type Parameters

• **T**

## Properties

### complete()

> **complete**: () => `void`

A callback function that gets called by the producer if and when it has no more
values to provide (by calling `next` callback function). This means that no error
has happened. This callback can't be called more than one time, it can't be called
if the `error` callback function have been called previously, nor it can't be called
if the consumer has unsubscribed.

#### Returns

`void`

#### Defined in

[src/types/subscribable.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/types/subscribable.ts#L26)

***

### error()

> **error**: (`err`) => `void`

A callback function that gets called by the producer if and when it encountered a
problem of any kind. The errored value will be provided through the `err` parameter.
This callback can't be called more than one time, it can't be called if the
`complete` callback function have been called previously, nor it can't be called if
the consumer has unsubscribed.

#### Parameters

##### err

`any`

#### Returns

`void`

#### Defined in

[src/types/subscribable.ts:18](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/types/subscribable.ts#L18)

***

### next()

> **next**: (`value`) => `void`

A callback function that gets called by the producer during the subscription when
the producer "has" the `value`. It won't be called if `error` or `complete` callback
functions have been called, nor after the consumer has unsubscribed.

#### Parameters

##### value

`T`

#### Returns

`void`

#### Defined in

[src/types/subscribable.ts:10](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/types/subscribable.ts#L10)
