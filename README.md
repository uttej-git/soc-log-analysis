# SOC Log Analysis – Failed SSH Login Detection

## 📌 Overview
This project demonstrates a **SOC (Security Operations Center) style log analysis** workflow using Linux authentication logs.  
The objective is to identify failed SSH login attempts and detect potential brute-force attacks by analyzing `auth.log`.

---

## 🎯 Objectives
- Analyze Linux authentication logs (`auth.log`)
- Detect failed SSH login attempts
- Identify suspicious IP addresses
- Simulate attack scenarios for SOC analysis practice
- Document findings in a structured manner

---

## 🛠 Tools & Technologies
- Ubuntu Linux (WSL)
- Bash shell scripting
- grep, awk, sort, uniq
- Git & GitHub

---


## 📂 Project Structure

```text
soc-log-analysis/
├── logs/
│   └── auth.log
├── analysis/
│   ├── failed_logins.txt
│   └── suspicious_ips.txt
└── report.txt



---

## 🔍 Methodology
1. Collected authentication logs from `/var/log/auth.log`
2. Filtered failed SSH login attempts
3. Removed noise caused by sudo command logs
4. Extracted attacker IP addresses using pattern matching
5. Counted repeated login attempts per IP
6. Documented findings in a SOC-style report

---

## 📊 Sample Output
2 192.168.56.101

- Indicates **2 failed SSH login attempts** from the same IP address

---

## 📝 Findings
- Repeated failed SSH login attempts were detected
- Activity indicates possible brute-force login behavior
- Attacker IP addresses were successfully identified

---

## ⚠️ Note
This project uses **simulated failed SSH login attempts** due to the absence of real attack data on a fresh Linux installation.  
The focus of the project is on **log analysis methodology**, not live exploitation.

---

## 🚀 Learning Outcomes
- Practical experience with Linux security logs
- Understanding SOC analyst workflows
- Improved Bash log-parsing skills
- Hands-on GitHub project documentation

---

## 👤 Author
**Uttej Kumar Sadanala**  
Cybersecurity Enthusiast | SOC Analyst Aspirant

