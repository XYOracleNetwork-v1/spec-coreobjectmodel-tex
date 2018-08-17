# 0x01 (Arrays)
Arrays are used when there is an unkown number of elements in a payload.
## 0x01 (Strong Array with Short Size and Short Number)
A strong array with size is used when there is an array with the same type, but the type has variable size (e.g. origin chain).

**Header**

Name | Size | Type
--- | --- | ---
Size | 2 Bytes | Unsigned Short
Major | 1 Byte | Byte
Minor | 1 Byte | Byte
Number of Elements | 2 Bytes | Unsigned Short

**Array Element**

Name | Size | Type
--- | --- | ---
Payload | Variable | Specified in Header wth the Major and Minor

## 0x02 (Strong Array without Size)
A strong array without size is used when there is an array with the same type, and the type has the same size (e.g. RSSI array).

**Header**

Name | Size | Type
--- | --- | ---
Major | 1 Byte | Byte
Minor | 1 Byte | Byte
Number of Elements | 2 Bytes | Unsigned Short

**Array Element**

Name | Size | Type
--- | --- | ---
Payload | Variable | Specified in Header wth the Major and Minor

## 0x03 (Weak Array with Short Size and Short Number)
A weak array is used when there is an array with different types (e.g. hueristics).

**Header**

Name | Size | Type
--- | --- | ---
Size | 2 Bytes | Unsigned Short
Number of Elements | 2 Bytes | Unsigned Short

**Array Element**

Name | Size | Type
--- | --- | ---
Major | 1 Byte | Byte
Minor | 1 Byte | Byte
Payload | Variable | Specified in the Major and Minor

## 0x04 (Strong Array with Byte Size and Byte Number)
A strong array with size is used when there is an array with the same type, but the type has variable size (e.g. origin chain).

**Header**

Name | Size | Type
--- | --- | ---
Size | 1 Byte | Unsigned Byte
Major | 1 Byte | Byte
Minor | 1 Byte | Byte
Number of Elements | 1 Byte | Unsigned Byte

**Array Element**

Name | Size | Type
--- | --- | ---
Payload | Variable | Specified in Header wth the Major and Minor

##  0x05
(Weak Array with Byte Size and Byte Number)
A weak array is used when there is an array with different types (e.g. hueristics).

**Header**

Name | Size | Type
--- | --- | ---
Size | 1 Byte | Unsigned Byte
Number of Elements | 1 Byte | Unsigned Byte

**Array Element**

Name | Size | Type
--- | --- | ---
Major | 1 Byte | Byte
Minor | 1 Byte | Byte
Payload | Variable | Specified in the Major and Minor

## 0x06 (Strong Array with Short Size and Byte Number)
A strong array with size is used when there is an array with the same type, but the type has variable size (e.g. origin chain).

**Header**

Name | Size | Type
--- | --- | ---
Size | 2 Bytes | Unsigned Short
Major | 1 Byte | Byte
Minor | 1 Byte | Byte
Number of Elements | 1 Byte | Unsigned Byte

**Array Element**

Name | Size | Type
--- | --- | ---
Payload | Variable | Specified in Header wth the Major and Minor

## 0x07 (Weak Array with Short Size and Byte Number)
A weak array is used when there is an array with different types (e.g. hueristics).

**Header**

Name | Size | Type
--- | --- | ---
Size | 2 Bytes | Unsigned Short
Number of Elements | 1 Byte | Byte

**Array Element**

Name | Size | Type
--- | --- | ---
Major | 1 Byte | Byte
Minor | 1 Byte | Byte
Payload | Variable | Specified in the Major and Minor

## 0x08 (Strong Array with Int Size and Short Number)
A strong array with size is used when there is an array with the same type, but the type has variable size (e.g. origin chain).

**Header**

Name | Size | Type
--- | --- | ---
Size | 4 Bytes | Unsigned Int
Major | 1 Byte | Byte
Minor | 1 Byte | Byte
Number of Elements | 2 Bytes | Unsigned Short

**Array Element**

Name | Size | Type
--- | --- | ---
Payload | Variable | Specified in Header wth the Major and Minor

## 0x09 (Weak Array with Int Size and Short Number)
A weak array is used when there is an array with different types (e.g. hueristics).

**Header**

Name | Size | Type
--- | --- | ---
Size | 4 Bytes | Unsigned Int
Number of Elements | 2 Bytes | Unsigned Short

**Array Element**

Name | Size | Type
--- | --- | ---
Major | 1 Byte | Byte
Minor | 1 Byte | Byte
Payload | Variable | Specified in the Major and Minor
