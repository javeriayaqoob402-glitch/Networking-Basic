# Internet, Network Aur Web Tools

---

* **Region/Country Level:** Internet ek poori region ya multiple countries ko connect karta hai.
* **City Level:** Isi tarah agar sirf ek city ke andar multiple offices ya houses connect hon, to wo bhi ek network hai lekin chhote scale par.
* **House/Office Level:** Ek ghar ya office ke andar bhi devices aapas mein ek chhota network bana sakte hain.
* **Data Sharing:** Jab devices ek network ke andar aapas mein data share karte hain, to us poore system ko network kaha jata hai — aur jab ye network country ke level tak phel jata hai, to usay internet kehte hain.

---

## Network Kya Hai

Network wo tareeqa hai jis se ek network ke andar devices ek doosre se, ya ek network se doosre network tak, connect ho sakte hain.
Matlab network sirf devices ko aapas mein jodne ka system hai — chahe wo ek ghar ke andar do computers hon, ya poori duniya ke devices.

---

## IP Address

IP (Internet Protocol) Address har device ki apni ek unique identity hoti hai network ke andar, jis se wo pehchana jata hai.
* **Example:** Home router ek IP address rakhta hai jis se wo network mein pehchana jata hai.

---

## NIC — Network Interface Card

Har device (jaise laptop) ke andar ek Network Interface Card (NIC) hota hai. Jab bhi koi device internet se connect hoti hai, to us device ka apna NIC hota hai jo connection banane mein madad karta hai.

---

## MAC Address

Jab koi device banai jati hai, to us par MAC address likh diya jata hai — ye ek permanent (fixed) address hota hai jo har device ke NIC ke sath hamesha ke liye juda hota hai.
* **Kaam Karne Ka Tarika:** Agar koi mobile device ko wifi router se connect karna chahe, to router us mobile ka MAC address dekhta hai aur badle mein us device ko ek IP address assign kar deta hai — taake wo device network mein pehchani ja sake.

---

## MAC Address vs IP Address — Difference

* **MAC Address:** Kabhi change nahi hota — ye device ke sath permanently juda hota hai (hardware level identity).
* **IP Address:** Change ho sakta hai — jab bhi device kisi naye network se connect hoti hai, to usay naya IP address mil sakta hai.
* **IP Address Kaun Deta Hai:** IP address hamesha router deta hai, jis se device internet use kar sakti hai.

---

## Network Commands

### `ip address`
Ye command device ka IP address dikhane ke liye use hoti hai.

* **Loopback (`lo`):** Loopback ek special network interface hota hai jo device ko apne aap ko hi call karne ke liye use hota hai — matlab isay "local host" bhi kaha jata hai. Ye khud device ke andar internal testing/communication ke liye use hota hai.
  * **Important Point:** Loopback ka address permanent hota hai — ye kabhi change nahi hota.
* **`wlan0`:** `wlan0` wo interface hai jo direct WiFi se connect hone par active ho jata hai. Agar device mein WiFi maujood na ho, to `wlan0` interface bhi list mein nahi aayega.
* **`eth0`:** `eth0` wo interface hai jo wire (cable) se connect hone par use hota hai — matlab jab device Ethernet cable ke zariye internet se juda hota hai.

### `hostname -i`
Ye command device ka IP address, router ka IP, aur MAC address — teeno information ek sath show karti hai.

---

## Ping Aur Traceroute

### Ping
Ping command kisi doosre device ko "Hello" kehne jaisa kaam karti hai — matlab ye check karti hai ke koi device active (alive) hai ya nahi.

* **Ping work:** Ping ek data ka packet resi device ko bhejti hai taake pata chal sake ke wo device abhi active hai ya nahi. Data packets ke zariye ek device doosre device ko data send karti hai.
* **Important Note:** Agar kisi device par firewall ya VPN use ho raha ho, ya device off ho, to us waqt ping kaam nahi karegi — response nahi milega.

**Example — Ping Ek Fixed IP Ko:**
```bash
ping 8.8.8.8
# SSH, Ports, aur Key-Lock Access (Detailed Concept)

# 🚀 Easy Networking Notes (Private IP, Public IP, NAT & Routing)

Yeh file networking ke basic concepts ko bohot aasan Roman Urdu + English mein explain karti hai taake koi bhi 5 minute mein poora flow samajh sake!

---

## 🏠 1. Private Network vs Public Network

| Concept | Explanation (Aasan Lafzon Mein) | Example Devices |
| :--- | :--- | :--- |
| **Private Network (LAN)** | Aap ke ghar / office ke **router ke andar ka ilaka**. Yeh data ghar se bahar nahi jata. | Laptop, Mobile, Smart TV, Wi-Fi Printer |
| **Public Network (WAN)** | Router ke **baher ka ilaka (Internet)** jo ISP (PTCL/Nayatel/Jazz) se jura hota hai. | Google, YouTube, Instagram Servers |

---

## 🔢 2. Private IP vs Public IP

### 🔹 Private IP Address
* **Kya hai?** Ghar ke andar har device ki local pehchan.
* **Kaise milta hai?** Router ka **DHCP** system auto-assign karta hai.
* **Example:** `192.168.1.2`, `192.168.1.5`
* **Khas baat:** Dunya ke har ghar mein same Private IP ho sakti hai (Local usage).

### 🌐 Public IP Address
* **Kya hai?** Dunya bhar ke Internet par aap ke Router ka **Unique (Global) Address**.
* **Kaise milta hai?** Aap ka **ISP (Internet Service Provider)** deta hai.
* **Example:** `39.50.200.12`
* **Khas baat:** Poori dunya mein ek waqt mein yeh IP sirf **aap ke router** ke paas hota hai. Internet se data wapas aap ke ghar aane ke liye yeh IP lazmi chahiye!

---

## 📊 3. IP Address Ranges (Pehchannay Ka Simple Rule)

Networking experts ne kuch specific numbers ko **Private** fix kar diya hai. In ke alawa baqi sab **Public** hain!

### 🟢 Private Ranges (Ghar/Office ke andar):
1. **Class A:** `10.0.0.0` se `10.255.255.255` *(Bari Companies / Enterprise)*
2. **Class B:** `172.16.0.0` se `172.31.255.255` *(Universities / Large Offices)*
3. **Class C:** `192.168.0.0` se `192.168.255.255` *(Ghar ka Wi-Fi Router)*

### 🌍 Public Ranges:
* In 3 Private ranges ke ilawa dunya ke tamam IP numbers **Public IPs** hain (e.g. Google IP: `8.8.8.8`).

---

## 🔀 4. NAT (Network Address Translation) & Port Numbers

**Sawal:** Ghar mein 5 devices hain, sab ka Public IP SAME hai. Jawab wapas kis device par jana hai, Router ko kaise pata chalta hai?

**Jawab (NAT Table Magic):**
1. Jab aap Laptop (`192.168.1.5`) se Google kholti hain, toh Router us par ek **Port Number** (e.g. `5001`) laga deta hai.
2. Router apni register (NAT Table) mein entry karta hai:  
   `Public IP : Port 5001 = Laptop (192.168.1.5)`
3. Jab Google response bhejta hai, toh Router Port 5001 dekh kar data **sidha Laptop** ko de deta hai!

---

## 🆔 5. IP Address vs MAC Address

* **IP Address (Logical Address):** Poore internet par **Destination (Manzil)** ka permanent address hota hai.
* **MAC Address (Physical Address):** Hardware ka permanent identity card number. Yeh har Router/Hop par **change** hota rehta hai (Raste ki Gaadi).

---

## 📝 Quick Summary Table

| Feature | Private IP | Public IP | MAC Address |
| :--- | :--- | :--- | :--- |
| **Kahan kaam karta hai?** | Ghar ke andar (LAN) | Dunya ke Internet par (WAN) | Device to Device (Local Link) |
| **Uniqueness?** | Local Network mein unique | Poori Dunya mein Unique | Hardware Level par Unique |
| **Assignee?** | Router (DHCP) | ISP (PTCL/Nayatel/Jazz) | Device Manufacturer |
