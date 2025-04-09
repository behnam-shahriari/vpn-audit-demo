# VPN Audit Simulation – Demo Report  
**Author:** Behnam Shahriari  
**Date:** April 9, 2025  

---

## 🔍 Objective  
To simulate a VPN audit and check for IP and DNS leaks using common tools and techniques.

---

## 🛠️ Tools Used  
- Windscribe VPN (Free version)  
- ipleak.net  
- dnsleaktest.com  
- Wireshark (for DNS packet capture)

---

## 🔬 Tests Performed  

### ✅ With VPN ON  
- **IPLeak.net:** IP masked (Romania) — real IP hidden  
- **DNSLeakTest:** DNS resolved via VPN provider (NetActuate) — no leak detected  

### ❌ With VPN OFF  
- **IPLeak.net:** Real IP visible (Türkiye)  
- **DNSLeakTest:** DNS requests sent to Google DNS servers — unprotected  

### 🧪 Wireshark Capture  
Captured DNS queries like `google.com`, `ipleak.net`, and `dnsleaktest.com`  
→ Verified DNS traffic visibility with and without VPN

---

## ✅ Conclusion  
- VPN effectively hid both IP and DNS when active  
- Without VPN, data was exposed — proving the importance of DNS protection  
- Wireshark confirmed visibility of DNS traffic

---

## 📌 Next Steps for Real Projects  
For an actual VPN app audit, I would:
- Test for WebRTC and IPv6 leaks  
- Analyze kill switch reliability  
- Check encryption protocols  
- Recommend DNS over HTTPS or DNS tunneling if needed

---

**Demo Files Attached:**  
- Screenshots folder (4 tests + Wireshark)  
- Wireshark capture file: `vpn-traffic.pcapng`
