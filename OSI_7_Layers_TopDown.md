# OSI Model — 7 Layers کی وضاحت (Application سے شروع)

OSI (Open Systems Interconnection) model ایک conceptual framework ہے جو بتاتا ہے کہ data ایک computer سے دوسرے computer تک network کے ذریعے کیسے سفر کرتا ہے۔ یہاں ہم اوپر سے نیچے (Application → Physical) ترتیب سے دیکھیں گے — یعنی جس طرح data user کی apps سے شروع ہو کر cable تک جاتا ہے۔

**یاد رکھنے کا طریقہ:** "All People Seem To Need Data Processing" (اوپر سے نیچے: Application → Physical)

---

## Layer 7 — Application Layer
**کام:** یہ وہ layer ہے جس سے user براہ راست contact میں آتا ہے — یعنی وہ apps اور protocols جو ہم روزانہ استعمال کرتے ہیں۔

**Examples:** Browser (HTTP/HTTPS)، Email (SMTP)، File transfer (FTP)۔

---

## Layer 6 — Presentation Layer
**کام:** Data کو ایسی شکل میں convert کرنا جسے Application Layer سمجھ سکے — جیسے encryption/decryption، compression، اور format conversion (جیسے JPEG, ASCII)۔

**Examples:** SSL/TLS encryption، data compression۔

---

## Layer 5 — Session Layer
**کام:** دو devices کے درمیان "session" یعنی connection کو start، maintain، اور end کرنا۔

**Examples:** Login sessions، video call کا connection برقرار رکھنا۔

---

## Layer 4 — Transport Layer
**کام:** Data کو segments میں تقسیم کرنا، یہ ensure کرنا کہ data مکمل اور صحیح ترتیب میں پہنچے۔ اگر کچھ lost ہو جائے تو دوبارہ بھیجنا۔

**Examples:** TCP (reliable، دوبارہ check کرتا ہے)، UDP (fast لیکن بغیر confirmation کے)۔

---

## Layer 3 — Network Layer
**کام:** Data کو ایک network سے دوسرے network تک بھیجنا — یعنی صحیح route ڈھونڈنا۔ یہاں IP address استعمال ہوتا ہے۔

**Examples:** Router، IP address، Ping، Traceroute۔

---

## Layer 2 — Data Link Layer
**کام:** Bits کو "frames" میں convert کرنا اور یہ ensure کرنا کہ data اسی local network کے اندر صحیح device تک پہنچے (MAC address کے ذریعے)۔ Error check بھی کرتی ہے۔

**Examples:** Switch، MAC address، Wi-Fi (802.11)۔

---

## Layer 1 — Physical Layer
**کام:** Raw data (bits: 0 اور 1) کو electrical signal، light، یا radio waves کی صورت میں ایک device سے دوسرے device تک transmit کرنا۔

**Examples:** Cables (Ethernet cable)، Hub، wireless signals، connectors۔

---

## خلاصہ Table (Application سے Physical تک)

| Layer # | نام | بنیادی کام | Example |
|---|---|---|---|
| 7 | Application | User کے ساتھ contact | Browser, Email |
| 6 | Presentation | Data format/encryption | SSL, JPEG |
| 5 | Session | Connection start/end | Login session |
| 4 | Transport | Data کی مکمل delivery | TCP, UDP |
| 3 | Network | صحیح route ڈھونڈنا | IP address, Router |
| 2 | Data Link | Local network میں delivery | MAC address, Switch |
| 1 | Physical | Raw signal transmission | Cable, Hub |

---

*یہ model networking سیکھنے کی بنیاد ہے — Packet Tracer میں practice کرتے وقت آپ Layer 3 (router, IP addressing)، Layer 2 (switch) اور Layer 1 (cables) کو عملی طور پر استعمال کریں گی۔*
