# Enhancing-Linux-Endpoint-Security-with-WAZUH-Unauthorized-Process-Detection


Author: [Adams Samson](https://www.linkedin.com/in/adams-samson)  
Project Repository: GitHub | 2025

## 🛡️ Problem Statement

10ALYTICS-DC, a growing provider of data center and cloud services, has identified vulnerabilities within its Linux environment. Legitimate tools like Netcat (used for debugging) are being exploited for malicious activities such as unauthorized access and data exfiltration. This project aims to improve real-time threat detection and response using Wazuh by ensuring only authorized processes are executed and suspicious activities are effectively blocked.

## 🎯 Objectives

- Implement Wazuh command monitoring to track active processes in real time  
- Detect and log unauthorized `nc` (Netcat) execution used for tunneling or backdoor access  
- Generate alerts in Wazuh for suspicious activity, with real-time visibility via the dashboard

## 🧰 Tools & Technologies

- **Wazuh** – SIEM tool for security monitoring & alerting  
- **Ubuntu** – Target endpoint system  
- **Kali Linux** – Attacker system for simulating unauthorized access  

## ⚙️ Deployment & Configuration

### Wazuh Agent on Ubuntu (Target)

- Deployed Wazuh agent to monitor system activity  
- Configured communication with Wazuh Manager to forward logs  
- Enabled command monitoring to detect unauthorized processes

### Kali Linux (Attacker Simulation)

- Executed unauthorized connections using Netcat  
- Simulated privilege escalation techniques  
- Verified that malicious activity was detected and logged by Wazuh

## 📈 Results – 10ALYTICS Data Centre

- **Process Execution Tracking**: Active processes successfully monitored in real time  
- **Detection of Netcat Usage**: Netcat execution was logged and flagged as a security concern  
- **Security Alerts**: Unauthorized activity triggered real-time alerts in Wazuh Dashboard  

## ✅ Recommendations

1. **Harden Endpoint Protection**: Implement process whitelisting and deploy antivirus solutions  
2. **Enable Continuous Logging**: Preserve audit logs for forensic investigations  
3. **Automate Incident Response**: Configure Wazuh remediation rules for auto-containment  
4. **Integrate Slack Webhook for Real-Time Monitoring**: Use Slack webhooks to push Wazuh alerts directly to the security team, enabling faster incident response and collaboration  

## 🔚 Conclusion

This project successfully demonstrates the role of Wazuh in reinforcing Linux endpoint security through real-time unauthorized process detection. By leveraging SIEM capabilities such as command monitoring and alerting, 10ALYTICS can proactively identify and contain threats, strengthen infrastructure resilience, and maintain operational integrity.

---

> 👨🏽‍💻 Connect with me: [Adams Samson on LinkedIn](https://www.linkedin.com/in/adams-samson)
