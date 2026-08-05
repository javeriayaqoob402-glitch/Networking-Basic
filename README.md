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
