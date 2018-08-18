# 0x02 (Core Objects)
Arrays are used when there is an unkown number of elements in a payload.
## 0x01 (Bound Witness)
A bound witness in the XYO Network.

**Structure**

Name | Size | Type
--- | --- | ---
Size | 4 Bytes | Unsigned Int
Keys | Variable |  Array(0x06) `Keyset`
Payloads Hash | Variable |  Array(0x06) `Hash`
Payloads | Variable |  Array(0x10) `Payload`
Signatures | Variable |  Array(0x06) `Signatures`

## 0x02 (Keyset)
A group of keys in the XYO Network.

**Structure**

Name | Size | Type
--- | --- | ---
Keys | Variable |  Array(0x07) `Encoded Public Key Object`

## 0x03 (Payload)
Heuristics in the XYO Network.

**Structure**

Name | Size | Type
--- | --- | ---
Heuristics | Variable |  Array(0x10) 
