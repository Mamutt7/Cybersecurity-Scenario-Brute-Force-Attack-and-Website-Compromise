# Cybersecurity Scenario: Brute Force Attack and Website Compromise

This project is part of the Google Cybersecurity Professional Certificate. It focuses on identifying and mitigating a brute force attack, documenting the security incident, and recommending security measures to prevent similar events. The scenario involves investigating a compromised website, analyzing network traffic, and suggesting remediations.

---

## 📋 Project Overview

### Scenario
The website **yummyrecipesforme.com** was compromised by a former employee through a brute force attack. The attacker exploited a default admin password to gain access to the web host's admin panel. They embedded malicious JavaScript into the website's source code, prompting visitors to download malware disguised as a browser update. The malware redirected users to a fake website, **greatrecipesforme.com**, where their devices were further compromised. 

As a cybersecurity analyst, my role was to:
1. Analyze the incident using `tcpdump` logs.
2. Document the attack and its impact.
3. Recommend a security measure to prevent future brute force attacks.

---

## 🔍 Key Findings

- **Attack Type:** Brute Force Attack leading to a compromised website.
- **Protocols Identified:**
  - **DNS**: Used to resolve the IP addresses of both legitimate and fake websites.
  - **HTTP**: Used for web traffic, including the malicious JavaScript and malware download.
- **Impact:** The website was compromised, customers were redirected to a fake website, and their devices were infected with malware.

---

## 🛠️ Skills Demonstrated

- **Network Protocol Analysis:**
  - Analyzed `tcpdump` logs to identify DNS and HTTP traffic patterns.
- **Incident Documentation:**
  - Documented the incident details, including the attack method, protocols used, and affected resources.
- **Recommendations for Remediation:**
  - Proposed actionable security measures to prevent similar attacks.

---

## 📖 Incident Report Summary

### Section 1: Network Protocol Involved
The attack involved the **DNS** and **HTTP** protocols:
1. **DNS** resolved the IP address of the original website (**yummyrecipesforme.com**) and the malicious website (**greatrecipesforme.com**).
2. **HTTP** facilitated web traffic, including the malicious JavaScript injection, malware download, and redirection to the fake website.

### Section 2: Incident Documentation
The incident began with a brute force attack where the attacker exploited the admin panel's default password. This allowed the attacker to modify the website's source code, embedding JavaScript that prompted users to download malware. After running the malware, users were redirected to the fake website. The issue was discovered when customers reported unusual activity, such as website redirects and slow devices. Analysis confirmed the presence of malicious JavaScript and malware.

### Section 3: Remediation Recommendation
**Recommendation:** Enforce **Two-Factor Authentication (2FA)** for admin panel logins.  
**Reason:** 2FA adds an additional layer of security, requiring both the correct password and a second verification method, such as a code sent to a trusted device. This makes it significantly harder for attackers to gain access, even if they successfully guess the password.

---

## 📂 File Contents

- **`tcpdump_log.txt`**: Contains the `tcpdump` traffic logs used to analyze the attack.

---

## 🏆 Key Takeaways

- Brute force attacks can exploit weak security configurations, such as default passwords.
- Analyzing DNS and HTTP protocols is critical for understanding website-based attacks.
- Implementing strong security measures like **Two-Factor Authentication (2FA)** can significantly reduce the risk of unauthorized access.

---

### License

This project is shared for educational purposes and is licensed under the MIT License.
