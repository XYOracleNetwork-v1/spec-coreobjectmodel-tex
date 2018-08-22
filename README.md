# sdk-coreobjectmodel-md

It is important to have an efficient way of encoding objects in the XYO Network given  the  limited  space  and  computational  power  on  IoT  devices.   To  solve this, we utilize a typed based encoding system where all object interpretation knowledge is held outside of the object itself.

## Types

Types act as identifiers for certain objects and interpretations for binary data. A type may infer size,  unpacking method,  and/or known information.  Types follow a major and minor structure for organization where the major is a group of objects and a minor is the field that describes the object type. 

Name | Major
--- | --- |
[Arrays](https://github.com/XYOracleNetwork/sdk-coreobjectmodel-json/blob/master/arrays.md) | 0x01
[Core Objects](https://github.com/XYOracleNetwork/sdk-coreobjectmodel-json/blob/master/coreObjects.md) | 0x02
[Hashes](https://github.com/XYOracleNetwork/sdk-coreobjectmodel-md/blob/master/hashes.md) | 0x03
[Public Key Cryptography](https://github.com/XYOracleNetwork/sdk-coreobjectmodel-md/blob/master/publicKeyCryptography.md) | 0x04
**Custum** | 0xff
