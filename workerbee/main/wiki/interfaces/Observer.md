[@hiveio/workerbee](../globals) / Observer

# Interface: Observer\<T\>

Defined in: [src/types/subscribable.ts:4](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/types/subscribable.ts#L4)

An object interface that defines a set of callback functions a user can use to get notified

## Type Parameters

### T

`T`

## Properties

### complete

> **complete**: () => `void`

Defined in: [src/types/subscribable.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/types/subscribable.ts#L26)

A callback function that gets called by the producer if and when it has no more
values to provide (by calling `next` callback function). This means that no error
has happened. This callback can't be called more than one time, it can't be called
if the `error` callback function have been called previously, nor it can't be called
if the consumer has unsubscribed.

#### Returns

`void`

***

### error

> **error**: (`err`) => `void`

Defined in: [src/types/subscribable.ts:18](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/types/subscribable.ts#L18)

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

***

### next

> **next**: (`value`) => `void`

Defined in: [src/types/subscribable.ts:10](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/types/subscribable.ts#L10)

A callback function that gets called by the producer during the subscription when
the producer "has" the `value`. It won't be called if `error` or `complete` callback
functions have been called, nor after the consumer has unsubscribed.

#### Parameters

##### value

`T`

#### Returns

`void`
