# VPN Audit Simulation Demo

This project demonstrates a basic VPN security audit simulation using publicly available tools. It was created as both a demo for potential clients and a portfolio piece to showcase practical networking and diagnostic skills.

## 🔍 Objective
To evaluate whether a VPN is correctly hiding a user's IP address and preventing DNS leaks using realistic test environments.

## 🛠 Tools Used
- [Windscribe VPN](https://windscribe.com/) (Free plan)
- [ipleak.net](https://ipleak.net) – IP & DNS leak test
- [dnsleaktest.com](https://dnsleaktest.com) – DNS resolver test
- [Wireshark](https://www.wireshark.org/) – Packet analyzer

## 📄 Files Included
- `vpn-audit-report.pdf` — Full report with explanations, results, and conclusions
- `vpn-audit-report.docx` — Editable version of the report
- `vpn-traffic.pcapng` — Raw packet capture for DNS traffic
- `/screenshots/` — 5 screenshots covering:
  - IP and DNS tests with VPN ON
  - IP and DNS tests with VPN OFF
  - Wireshark DNS traffic view

## ✅ Summary of Results
- When VPN was ON:
  - IP address and DNS were properly masked (Romania location via VPN)
- When VPN was OFF:
  - Real IP and Google DNS resolvers were exposed (as expected)
- Wireshark:
  - Showed live DNS queries, verifying visibility and leak conditions

## 📌 Next Steps for a Real VPN App Audit
In a real client environment, further steps would include:
- Checking for WebRTC and IPv6 leaks
- Testing kill switch functionality
- Evaluating DNS over HTTPS or encrypted DNS
- Reviewing connection logs and VPN protocols

## 👨‍💻 Created By
Behnam Shahriari  
[Upwork Profile](https://www.upwork.com/freelancers/~01behnam-shahriari)  
[GitHub](https://github.com/behnam-shahriari)

---

*This demo is intended for educational and portfolio purposes.*
