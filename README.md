[logo]: https://www.xy.company/img/home/logo_xy.png

![logo]

# XYO Core Object Model (spec-coreobjectmodel-tex)

It is important to have an efficient way of encoding objects in the XYO Network given  the  limited  space  and  computational  power  on  IoT  devices.   To  solve this, we utilize a typed based encoding system where all object interpretation knowledge is held outside of the object itself.

## Types

Types act as identifiers for certain objects and interpretations for binary data. A type may infer size,  unpacking method,  and/or known information.  Types follow a major and minor structure for organization where the major is a group of objects and a minor is the field that describes the object type. 

Name | Major
--- | --- |
[Arrays](https://github.com/XYOracleNetwork/spec-coreobjectmodel-tex/blob/master/arrays.pdf) | 0x01
[Core Objects](https://github.com/XYOracleNetwork/spec-coreobjectmodel-tex/blob/master/coreObjects.pdf) | 0x02
[Hashes](https://github.com/XYOracleNetwork/spec-coreobjectmodel-tex/blob/master/hashes.pdf) | 0x03
[Public Keys](https://github.com/XYOracleNetwork/spec-coreobjectmodel-tex/blob/master/publicKeys.pdf) | 0x04
[Signatures](https://github.com/XYOracleNetwork/spec-coreobjectmodel-tex/blob/master/signatures.pdf) | 0x05
**Custum** | 0xff

## Credits
Made with ❤️
by [XYO](https://xyo.network)