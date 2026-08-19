# IPv6 Basics

## What is IPv6?

IPv6 stands for **Internet Protocol Version 6**. It is used to identify devices on networks.

- IPv6 = **128 bits**
- IPv4 = **32 bits**
- IPv6 uses **8 groups**
- Each group contains **4 hexadecimal digits**

Example:

`2001:0db8:85a3:0000:0000:8a2e:0370:7334`

8 groups × 16 bits = **128 bits**

## IPv6 and Hexadecimal

IPv6 uses hexadecimal:

`0 1 2 3 4 5 6 7 8 9 A B C D E F`

Every hexadecimal digit represents **4 binary bits**.

| Hex | Binary |
|---|---|
| 0 | 0000 |
| 1 | 0001 |
| 2 | 0010 |
| 3 | 0011 |
| 4 | 0100 |
| 5 | 0101 |
| 6 | 0110 |
| 7 | 0111 |
| 8 | 1000 |
| 9 | 1001 |
| A | 1010 |
| B | 1011 |
| C | 1100 |
| D | 1101 |
| E | 1110 |
| F | 1111 |

## IPv6 to Binary

Convert **each hexadecimal digit** into 4 binary bits.

Example:

`2001`

- `2` = `0010`
- `0` = `0000`
- `0` = `0000`
- `1` = `0001`

Therefore:

`2001 = 0010000000000001`

One IPv6 group contains **16 bits**.

## Complete Example

IPv6:

`2001:0db8:85a3:0000:0000:8a2e:0370:7334`

Binary:

`0010000000000001:0000110110111000:1000010110100011:0000000000000000:0000000000000000:1000101000101110:0000001101110000:0111001100110100`

Total = **128 bits**

## IPv4 vs IPv6

| Feature | IPv4 | IPv6 |
|---|---|---|
| Address size | 32 bits | 128 bits |
| Format | Decimal | Hexadecimal |
| Groups | 4 octets | 8 groups |
| Example | 192.168.1.10 | 2001:db8::1 |

## Easy Rule

**IPv4:** Decimal → Binary  
Example: `192 = 11000000`

**IPv6:** Hexadecimal → Binary  
Example: `A = 1010`

### Practice

Convert these to binary:

1. `A`
2. `F`
3. `B`
4. `2`
5. `C`
6. `9`

Convert these IPv6 groups:

1. `2001`
2. `0db8`
3. `abcd`
4. `1234`
5. `ffff`

## Summary

**IPv6 = 128 bits**

**8 groups × 16 bits = 128 bits**

**1 hexadecimal digit = 4 binary bits**

For IPv6 binary conversion, convert every hexadecimal digit into its 4-bit binary equivalent.
