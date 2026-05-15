# 🛡️ Mission: The Invisible Logic
**Cybersecurity Foundations Intensive** | *API Security & Logic Flaw Audit*

---

### **📌 Mission Objective**
The goal of this laboratory was to perform a security audit on a containerized web storefront. I focused on identifying **Broken Object Level Authorization (BOLA)** and exploiting **Business Logic Flaws** to recover sensitive data and bypass pricing restrictions.

---

### **🛠️ Technical Stack**
| Category | Tools & Technologies |
| :--- | :--- |
| **Environment** | Docker, Ubuntu VM, Nginx |
| **Testing** | Burp Suite Community Edition, cURL |
| **Scripting** | Python 3, Bash |
| **Documentation** | Git, GitHub |

---

### **🔍 Key Security Findings**
* **BOLA (ID Swap):** Successfully exploited a vulnerability in the `/api/v1/profile/` endpoint by swapping User IDs to leak private admin credentials.
* **Logic Exploitation:** Used **Burp Suite Intruder** to brute-force a 4-digit discount code, bypassing the intended purchase logic of the storefront.
* **Remediation:** Recommended implementing **Rate Limiting** and **Strict Object-Level Authorization** checks on all API requests.

---

### **📂 Lab Inventory**
* `api_audit.log`: Detailed record of intercepted traffic and exploited endpoints.
* `deploy_web.sh`: Bash script used to provision the laboratory environment.
* `README.md`: Mission documentation and summary.
