# IPv4 — Basic Notes

## 1. IPv4 hota kya hai?

IPv4 ka full form **Internet Protocol Version 4** hai.

IPv4 ek addressing system hai jo network par devices ko identify karne ke liye use hota hai.

Example:

    192.168.1.10

IPv4 address mein **4 octets** hote hain aur har octet ki value **0 se 255** tak hoti hai.

Example:

    192 . 168 . 1 . 10
     ↑     ↑    ↑    ↑
   Octet Octet Octet Octet

IPv4 total **32 bits** ka hota hai:

    4 octets × 8 bits = 32 bits

---

## 2. IPv4 ko Binary mein kaise convert karte hain?

Har decimal octet ko separately **8-bit binary** mein convert karte hain.

Binary place values:

    128  64  32  16  8  4  2  1

### Example: 192 ko binary mein convert karna

192 = 128 + 64

Isliye:

    128 64 32 16 8 4 2 1
     1  1  0  0 0 0 0 0

So:

    192 = 11000000

### Example: 168 ko binary mein convert karna

168 = 128 + 32 + 8

    128 64 32 16 8 4 2 1
     1  0  1  0 1 0 0 0

So:

    168 = 10101000

### Example: 1

    1 = 00000001

### Example: 10

10 = 8 + 2

    128 64 32 16 8 4 2 1
     0  0  0  0 1 0 1 0

So:

    10 = 00001010

---

## 3. Complete IPv4 example

IPv4:

    192.168.1.10

Convert each octet:

    192 = 11000000
    168 = 10101000
      1 = 00000001
     10 = 00001010

Therefore:

    192.168.1.10

becomes:

    11000000.10101000.00000001.00001010

Ye complete IPv4 ka **32-bit binary representation** hai.

---

## 4. Binary se Decimal kaise nikalte hain?

Binary ko decimal mein convert karne ke liye **8-bit place values** use karo:

    128  64  32  16  8  4  2  1

Binary number mein jahan **1** ho, us place value ko add karo.

### Example: 11000000

    128 64 32 16 8 4 2 1
     1  1  0  0 0 0 0 0

Add:

    128 + 64 = 192

So:

    11000000 = 192

### Example: 10101000

    128 64 32 16 8 4 2 1
     1  0  1  0 1 0 0 0

Add:

    128 + 32 + 8 = 168

So:

    10101000 = 168

### Complete IPv4 example

Binary:

    11000000.10101000.00000001.00001010

Har octet separately convert karo:

    11000000 = 192
    10101000 = 168
    00000001 = 1
    00001010 = 10

Result:

    192.168.1.10

**Easy rule:** Binary mein jahan `1` ho, uski value add karo; jahan `0` ho, ignore karo.

## 5. Important rule

IPv4 ke har octet ke liye ye values yaad rakho:

    128 64 32 16 8 4 2 1

Agar decimal number ko binary mein convert karna ho, in values mein se woh values choose karo jin ka sum tumhara decimal number banata ho.

Example:

    150 = 128 + 16 + 4 + 2

Therefore:

    150 = 10010110

---

## 6. Practice

Khud convert karo:

1. 192 → ?
2. 168 → ?
3. 10 → ?
4. 255 → ?
5. 172 → ?
6. 16 → ?
7. 64 → ?
8. 127 → ?

Phir complete addresses:

    192.168.1.1
    10.0.0.5
    172.16.10.20

ko binary mein convert karne ki practice karo.

## Quick Summary

**IPv4 = 32 bits = 4 octets × 8 bits**

Example:

    192.168.1.10

Binary:

    11000000.10101000.00000001.00001010

**Conversion values:**

    128 64 32 16 8 4 2 1

**Rule:** Har octet ko separately 8-bit binary mein convert karo.
