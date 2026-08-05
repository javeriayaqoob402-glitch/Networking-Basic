# SSH, Ports, aur Key-Lock Access (Complete Documentation)

## 1. Ports Kya Hain?

Computer mein **Port** ek darwazay (door) ki tarah hota hai jo kisi
specific service ya app ke liye khula hota hai.

**IP Address:** Aapka ghar ka pata (Address) hai.

**Port:** Aapke ghar ka specific darwaza hai (Jaise main door, back
door, window).

**Example:** Web browsing ke liye Port **80/443** khula hota hai, aur
remote management ke liye **Port 22**.

------------------------------------------------------------------------

## 2. SSH Kya Hai?

**SSH (Secure Shell)** ek safe pathway (surakshit rasta) hai jo **Port
22** ke zariye do computers ko aapas mein jorta hai. Is ke zariye aap
kisi doosre computer ko remotely (door baith kar) control kar sakte
hain. Aap ka bheja gaya saara data encrypt (code) ho kar jata hai taake
beech mein koi use chura na sake.

------------------------------------------------------------------------

## 3. SSH Key & Lock Concept (Bina Password Access)

Jab aap baar baar kisi doosre laptop se pictures ya files lena chahte
hain, toh har baar password daalna pareshani banta hai. Is ko khatam
karne ke liye hum **Public Key (Taala/Lock)** aur **Private Key
(Chabi/Key)** ka concept use karte hain.

### Key & Lock Kaise Kaam Karta Hai?

1.  **Public Key (Taala/Lock):** Ye aap apne dost/target ke laptop mein
    daal dete hain. Is ko koi bhi dekh le toh fark nahi parta.

2.  **Private Key (Chabi):** Ye sirf aapke apne laptop mein rehti hai.
    Is ko kisi ke saath share nahi kiya jata.

Jab aapka laptop samne wale laptop se connect hone lagta hai, toh aapki
**Chabi (Private Key)** us ke laptop par lage **Taale (Public Key)** se
match hoti hai. Matching hone par darwaza bina password ke turant khul
jata hai.

------------------------------------------------------------------------

## 4. Practical Implementation (Step-by-Step)

### Step 1: Apne Laptop Par Key Pair (Chabi aur Taala) Banayein

``` bash
ssh-keygen
```
