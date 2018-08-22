# 0x04, 0x05 (Public Key Cryptography)
All Public Key Cryptography types. All public keys have a major of `0x04`, and all signatures have a major of `0x05`

## 0x01 (ECDSA (secp256k1) with SHA256)
**Keypair Algorithm:** EC, Uncompressed (0x04 not prefixed because this is infered). 

**Curve:** secp256k1

**Signing Algorithm:** SHA256 with ECDSA

**Structure**

**Public Key**

Name | Size | Type
--- | --- | ---
Point X| 32 Bytes |  ByteArray
Point Y| 32 Bytes |  ByteArray

**Signature**

Name | Size | Type
--- | --- | ---
Signature Size | 1 Byte |  ByteArray
Signature | Variable |  ByteArray

## 0x02 (ECDSA (secp256k1) with SHA256)
**Keypair Algorithm:** EC, Compressed (Point Y is 03 if Y is odd, and 02 for even). 

**Curve:** secp256k1

**Signing Algorithm:** SHA256 with ECDSA

**Structure**

Name | Size | Type
--- | --- | ---
Point Y | 1 Byte |  ByteArray
Point X | 32 Bytes |  ByteArray

**Signature**

Name | Size | Type
--- | --- | ---
Signature Size | 1 Byte |  ByteArray
Signature | Variable |  ByteArray

