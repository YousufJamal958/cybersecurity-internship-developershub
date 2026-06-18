# 🔐 Cybersecurity Internship — Developershub
### Vulnerability Assessment & Security Hardening of a Node.js Web Application

![Security](https://img.shields.io/badge/Security-Assessment-red)
![Node.js](https://img.shields.io/badge/Node.js-Web%20App-green)
![OWASP](https://img.shields.io/badge/OWASP-NodeGoat-blue)
![Status](https://img.shields.io/badge/Status-In%20Progress-orange)

---

## 👤 Intern Details

| Field | Details |
|-------|---------|
| **Name** | Yousuf Jamal |
| **Internship** | Developershub Cybersecurity Internship |
| **Deadline** | June 26, 2026 |
| **Target App** | OWASP NodeGoat v1.3 |

---

## 📋 Project Overview

This repository contains all work completed during the Developershub Cybersecurity Internship. The goal is to analyze a vulnerable Node.js web application (OWASP NodeGoat), identify security vulnerabilities, implement fixes, and document all findings.

The project is divided into 3 weeks:

| Week | Task | Status |
|------|------|--------|
| Week 1 | Security Assessment & Vulnerability Testing | ✅ Complete |
| Week 2 | Implementing Security Fixes | 🔄 In Progress |
| Week 3 | Advanced Security & Final Report | ⏳ Upcoming |

---

## 🎯 Week 1 — Security Assessment

### What Was Done
- Set up OWASP NodeGoat (a deliberately vulnerable Node.js app) on localhost
- Performed manual vulnerability testing (XSS and SQL Injection)
- Ran an automated vulnerability scan using OWASP ZAP
- Documented all findings in a formal report

### Tools Used
| Tool | Purpose |
|------|---------|
| OWASP ZAP | Automated vulnerability scanner |
| Browser Developer Tools | Manual inspection and XSS testing |
| MongoDB 5.0 | Database for the application |
| Node.js v24 | Runtime environment |

### Key Findings Summary

| Risk Level | Count |
|------------|-------|
| 🔴 High | 4 |
| 🟠 Medium | 8 |
| 🟡 Low | 10 |
| **Total** | **22** |

### Vulnerabilities Found
- ✅ **Cross-Site Scripting (XSS)** — Confirmed via manual test (script executed in browser)
- ✅ **Cross-Site Scripting Persistent** — Found by OWASP ZAP
- ✅ **Cross-Site Scripting Reflected (x11)** — Found by OWASP ZAP
- ✅ **SQL Injection** — Found by OWASP ZAP
- ✅ **Off-site Redirect** — Found by OWASP ZAP
- ✅ **Missing Security Headers** (CSP, Anti-clickjacking, X-Content-Type)
- ✅ **Vulnerable JavaScript Libraries (x2)**
- ✅ **Cookie without SameSite Attribute**
- ✅ **Application Error Disclosure**
- ✅ **Directory Browsing Enabled**

### 📄 Report
The full vulnerability assessment report is included in this repository:
👉 `Week1_Cybersecurity_Assessment_Report.docx`

---

## 🔧 Week 2 — Security Fixes (In Progress)

Planned fixes include:

- **Input Sanitization** — Using the `validator` library
- **Password Hashing** — Using `bcrypt`
- **Token Authentication** — Using `jsonwebtoken`
- **Security Headers** — Using `helmet`
- **Logging** — Using `winston`

---

## 🚀 How to Run the Application

### Prerequisites
- Node.js installed
- MongoDB 5.0 installed and running

### Steps

**1. Start MongoDB:**
```bash
net start MongoDB
```

**2. Install dependencies:**
```bash
npm install
```

**3. Start the application:**
```bash
npm start
```

**4. Open in browser:**
```
http://localhost:4000
```

---

## 📁 Repository Structure

```
├── app/                  # Main application code
│   ├── routes/           # Express route handlers
│   ├── views/            # HTML templates
│   └── assets/           # Static files (CSS, JS)
├── artifacts/            # Database reset scripts
├── config/               # App configuration files
├── test/                 # Test files
├── server.js             # Main server entry point
├── package.json          # Dependencies
├── Week1_Cybersecurity_Assessment_Report.docx
└── README.md
```

---

## 📚 What I Learned

- How to set up and analyze a vulnerable web application
- How Cross-Site Scripting (XSS) attacks work in practice
- How to use OWASP ZAP for automated security scanning
- How to document vulnerabilities in a professional report
- The importance of input sanitization and security headers

---

## 🔗 References

- [OWASP NodeGoat](https://github.com/OWASP/NodeGoat)
- [OWASP ZAP](https://www.zaproxy.org/)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [Node.js Security Best Practices](https://nodejs.org/en/docs/guides/security/)

---

*Developershub Cybersecurity Internship — June 2026*
