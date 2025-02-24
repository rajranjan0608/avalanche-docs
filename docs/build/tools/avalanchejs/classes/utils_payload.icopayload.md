[avalanche](../README.md) › [Utils-Payload](../modules/utils_payload.md) › [ICOPayload](utils_payload.icopayload.md)

# Class: ICOPayload

Class for payloads representing ICO images.

## Hierarchy

  ↳ [BINPayload](utils_payload.binpayload.md)

  ↳ **ICOPayload**

## Index

### Constructors

* [constructor](utils_payload.icopayload.md#constructor)

### Properties

* [payload](utils_payload.icopayload.md#protected-payload)
* [typeid](utils_payload.icopayload.md#protected-typeid)

### Methods

* [fromBuffer](utils_payload.icopayload.md#frombuffer)
* [getContent](utils_payload.icopayload.md#getcontent)
* [getPayload](utils_payload.icopayload.md#getpayload)
* [returnType](utils_payload.icopayload.md#returntype)
* [toBuffer](utils_payload.icopayload.md#tobuffer)
* [typeID](utils_payload.icopayload.md#typeid)
* [typeName](utils_payload.icopayload.md#typename)

## Constructors

###  constructor

\+ **new ICOPayload**(`payload`: any): *[ICOPayload](utils_payload.icopayload.md)*

*Inherited from [BINPayload](utils_payload.binpayload.md).[constructor](utils_payload.binpayload.md#constructor)*

*Overrides [PayloadBase](utils_payload.payloadbase.md).[constructor](utils_payload.payloadbase.md#constructor)*

*Defined in [src/utils/payload.ts:278](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L278)*

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`payload` | any | undefined | Buffer only  |

**Returns:** *[ICOPayload](utils_payload.icopayload.md)*

## Properties

### `Protected` payload

• **payload**: *Buffer* = Buffer.alloc(0)

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[payload](utils_payload.payloadbase.md#protected-payload)*

*Defined in [src/utils/payload.ts:198](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L198)*

___

### `Protected` typeid

• **typeid**: *number* = 21

*Overrides [BINPayload](utils_payload.binpayload.md).[typeid](utils_payload.binpayload.md#protected-typeid)*

*Defined in [src/utils/payload.ts:600](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L600)*

## Methods

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[fromBuffer](utils_payload.payloadbase.md#frombuffer)*

*Defined in [src/utils/payload.ts:236](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L236)*

Decodes the payload as a [Buffer](https://github.com/feross/buffer) including 4 bytes for the length and TypeID.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getContent

▸ **getContent**(): *Buffer*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[getContent](utils_payload.payloadbase.md#getcontent)*

*Defined in [src/utils/payload.ts:218](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L218)*

Returns the payload content (minus typeID).

**Returns:** *Buffer*

___

###  getPayload

▸ **getPayload**(): *Buffer*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[getPayload](utils_payload.payloadbase.md#getpayload)*

*Defined in [src/utils/payload.ts:226](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L226)*

Returns the payload (with typeID).

**Returns:** *Buffer*

___

###  returnType

▸ **returnType**(): *Buffer*

*Inherited from [BINPayload](utils_payload.binpayload.md).[returnType](utils_payload.binpayload.md#returntype)*

*Overrides [PayloadBase](utils_payload.payloadbase.md).[returnType](utils_payload.payloadbase.md#abstract-returntype)*

*Defined in [src/utils/payload.ts:276](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L276)*

Returns a [Buffer](https://github.com/feross/buffer) for the payload.

**Returns:** *Buffer*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[toBuffer](utils_payload.payloadbase.md#tobuffer)*

*Defined in [src/utils/payload.ts:251](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L251)*

Encodes the payload as a [Buffer](https://github.com/feross/buffer) including 4 bytes for the length and TypeID.

**Returns:** *Buffer*

___

###  typeID

▸ **typeID**(): *number*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[typeID](utils_payload.payloadbase.md#typeid)*

*Defined in [src/utils/payload.ts:204](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L204)*

Returns the TypeID for the payload.

**Returns:** *number*

___

###  typeName

▸ **typeName**(): *string*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[typeName](utils_payload.payloadbase.md#typename)*

*Defined in [src/utils/payload.ts:211](https://github.com/ava-labs/avalanchejs/blob/598fbcc/src/utils/payload.ts#L211)*

Returns the string name for the payload's type.

**Returns:** *string*
