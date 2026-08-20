# Kali Linux — 50 Zaroori Commands

## 📁 Navigation & File Management (1-15)

1. `pwd` — Batata hai ke abhi aap kis directory mein hain
2. `ls` — Current directory ki files/folders dikhata hai
3. `ls -a` — Hidden files bhi dikhata hai
4. `ls -l` — Files ki tafseeli list (permissions, size, date)
5. `cd foldername` — Us folder ke andar jata hai
6. `cd ..` — Ek folder peeche jata hai
7. `cd ~` — Seedha home directory mein le jata hai
8. `mkdir foldername` — Naya folder banata hai
9. `touch filename` — Nayi khaali file banata hai
10. `rm filename` — File delete karta hai
11. `rm -r foldername` — Poora folder delete karta hai
12. `cp source destination` — File copy karta hai
13. `mv source destination` — File move ya rename karta hai
14. `cat filename` — File ka content dikhata hai
15. `nano filename` — File edit karne ke liye kholta hai

---

## 🔍 Search & Find (16-22)

16. `find /path -name "filename"` — File ko naam se dhoondta hai
17. `grep "word" filename` — File ke andar lafz dhoondta hai
18. `grep -r "word" /path` — Poore folder mein lafz dhoondta hai
19. `locate filename` — File ki location system mein batata hai
20. `which commandname` — Command kahan installed hai batata hai
21. `head filename` — File ki shuru ki 10 lines dikhata hai
22. `tail filename` — File ki aakhri 10 lines dikhata hai

---

## 🔐 Permissions & Users (23-29)

23. `chmod 755 filename` — File ki permissions set karta hai
24. `chown user filename` — File ka owner badalta hai
25. `whoami` — Batata hai kaunse user ke tor par login hain
26. `sudo command` — Admin permission ke sath command chalata hai
27. `su` — Doosray user mein switch karta hai
28. `passwd` — Apna password badalta hai
29. `id` — User ki ID aur groups dikhata hai

---

## 🌐 Networking (30-40)

30. `ifconfig` — Network interfaces aur IP address dikhata hai
31. `ip a` — IP address dikhane ka naya tareeqa
32. `ping IP/domain` — Server tak connection check karta hai
33. `netstat -tulpn` — Kaunse ports open hain dikhata hai
34. `ssh user@ip` — Doosray computer se securely connect karta hai
35. `nmap IP` — Network scan karta hai
36. `curl url` — Web page ka content terminal mein laata hai
37. `wget url` — Internet se file download karta hai
38. `traceroute domain` — Data ka safar (route) dikhata hai
39. `hostname` — Computer ka naam batata hai
40. `dig domain` — Domain ki DNS information nikalta hai

---

## 💻 System Info & Processes (41-50)

41. `uname -a` — System/kernel ki information dikhata hai
42. `top` — Chal rahe processes aur CPU/RAM usage dikhata hai
43. `df -h` — Disk space ki information dikhata hai
44. `du -sh foldername` — Folder ka size batata hai
45. `free -h` — RAM ka istemal dikhata hai
46. `history` — Pichli commands ki list dikhata hai
47. `ps aux` — Sab chal rahe processes ki list
48. `kill PID` — Process ko uski ID se band karta hai
49. `apt update` — Software list update karta hai
50. `apt install packagename` — Naya software install karta hai

---

## 💡 Chhote Tips

- **Tab key** — command/filename khud complete ho jata hai
- **Up/Down arrow** — purani commands wapis la sakti hain
- **Ctrl + C** — chalti hui command rok deta hai
- **clear** ya **Ctrl + L** — terminal screen saaf karta hai
- **man commandname** — kisi command ki poori details dikhata hai

---

*Bar bar khud terminal mein try karein — sirf padhne se yaad nahi hote, practice se hote hain.*
