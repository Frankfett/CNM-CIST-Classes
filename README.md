# CNM Cybersecurity Lab Activity Suite

A comprehensive, hands-on lab environment for Central New Mexico Community College's cybersecurity curriculum. This project provides interactive, professionally-designed lab activities spanning offensive security, defensive forensics, and incident response.

**Instructor:** Frank | CISSP, SecAI Certified  
**Institution:** Central New Mexico Community College  
**Program:** Cybersecurity  

---

## 📋 Overview

This lab suite consists of 10 progressive activities designed to build practical red team and blue team competency. Activities range from **Beginner** (network reconnaissance) to **Advanced** (memory forensics, malware analysis), with each building foundational knowledge for the next.

### Design Philosophy

- **Hands-on first:** Every activity includes practical exercises with real tools
- **Progressive difficulty:** Activities scaffold in complexity and depth
- **Professional standards:** Content aligns with industry certifications (Security+, CISSP, CEH, OSCP)
- **Forensically sound:** Defensive activities follow NIST and SWGDE guidelines
- **Ethical framework:** Legal warnings and authorization requirements in every activity

---

## 🎯 Activity Breakdown

### **Offensive Security Track (Activities 01–05)**

| # | Activity | Level | Duration | Focus |
|---|----------|-------|----------|-------|
| **01** | Network Reconnaissance | Beginner | 2-3 hrs | Passive/active recon, DNS enumeration, ICMP discovery |
| **02** | Port Scanning Fundamentals | Beginner | 2-3 hrs | Nmap, scan types, service detection, OS fingerprinting |
| **03** | Vulnerability Assessment | Intermediate | 3-4 hrs | Nessus, OpenVAS, CVSS scoring, remediation tracking |
| **04** | Metasploit Exploitation | Intermediate | 4-5 hrs | Module types, payloads, Meterpreter, post-exploitation |
| **05** | Wireless Security Testing | Advanced | 4-6 hrs | 802.11, Aircrack-ng, handshake capture, WPA2 cracking |

### **Defensive Forensics & Incident Response Track (Activities 06–10)**

| # | Activity | Level | Duration | Focus |
|---|----------|-------|----------|-------|
| **06** | Forensic Evidence Collection | Intermediate | 3-4 hrs | Chain of custody, hash verification, disk imaging |
| **07** | Memory Forensics Analysis | Advanced | 5-6 hrs | Volatility, rootkit detection, network connections, malware |
| **08** | Malware Analysis Lab | Advanced | 5-7 hrs | Static/dynamic analysis, IDA Pro, Ghidra, behavioral IOCs |
| **09** | Incident Response Playbook | Intermediate | 4-5 hrs | Timeline analysis, artifact correlation, threat hunting |
| **10** | Security Hardening | Beginner | 2-3 hrs | Baselines, patch management, configuration as code |

---

## 🚀 Getting Started

### Prerequisites

- **Web Browser:** Modern browser with ES6 JavaScript support
- **Local Hosting (optional):** Python HTTP server for offline use
  ```bash
  python3 -m http.server 8000
  ```

### Quick Start

1. **Clone/Download** the repository
   ```bash
   git clone https://github.com/your-org/CNM-CIST-Classes.git
   cd CNM-CIST-Classes
   ```

2. **Open the landing page**
   ```bash
   open index.html
   # or
   firefox index.html
   ```

3. **Navigate to an activity**
   - Click on any activity card from the home page
   - Or directly open `activity01.html`, `activity02.html`, etc.

4. **Track progress**
   - Checklists auto-save to browser localStorage
   - Progress bars indicate completion percentage
   - Previous/Next navigation links between activities

### Lab Requirements by Activity

**Offensive Track:**
- Activities 01–02: Linux terminal, Nmap, basic networking tools
- Activity 03: Nessus or OpenVAS (free versions available)
- Activity 04: Metasploit framework, vulnerable VMs (HackTheBox, TryHackMe)
- Activity 05: Aircrack-ng suite, WiFi adapter with monitor mode, wireless lab network

**Defensive Track:**
- Activity 06: dd/ddrescue, write blockers, forensic imaging tools
- Activity 07: Volatility framework, memory dumps (DumpIt, LiME)
- Activity 08: IDA Pro/Ghidra, debuggers (WinDbg), malware samples (curated)
- Activity 09: Log aggregation tools, timeline utilities (Plaso)
- Activity 10: Configuration management tools, hardening baselines

---

## 📁 Project Structure

```
CNM-CIST-Classes/
├── index.html              # Landing page with course overview & activity grid
├── activity01.html         # Network Reconnaissance
├── activity02.html         # Port Scanning Fundamentals
├── activity03.html         # Vulnerability Assessment
├── activity04.html         # Metasploit Exploitation
├── activity05.html         # Wireless Security Testing
├── activity06.html         # Forensic Evidence Collection
├── activity07.html         # Memory Forensics Analysis
├── activity08.html         # Malware Analysis Lab
├── activity09.html         # Incident Response Playbook
├── activity10.html         # Security Hardening
├── README.md               # This file
├── CONTRIBUTING.md         # Contribution guidelines
└── docs/
    ├── STANDARDS.md        # Design and content standards
    ├── SETUP.md            # Detailed environment setup
    └── CERTIFICATE_PATHS.md # Alignment with industry certs
```

---

## 🎨 Design System

All activities use a **consistent, professional design language**:

### Color Palette
- **Navy** (`#0F1419`): Primary background and text
- **Cyan** (`#00D9FF`): Accent for links, highlights, beginner/intermediate badges
- **Red** (`#DC3545`): Advanced badges, warnings, critical alerts
- **Gray Light** (`#F0F2F5`): Page background
- **Green** (`#28A745`): Success states, tips

### Components
- **Sticky header** with navigation and breadcrumb
- **Hero section** with activity badge, title, metadata (difficulty, duration, tools)
- **Content wrapper** with progressive sections
- **Info boxes** (objective, warning, tip) for key concepts
- **Code blocks** with syntax highlighting (dark navy, cyan text)
- **Checklists** with localStorage persistence
- **Tables** for artifacts, tools, and technical data
- **Tool grids** highlighting required software
- **Phase workflow cards** showing sequential processes
- **Progress bar** indicating completion (updated on scroll)
- **Navigation** (Previous/Next) between activities

### Typography
- **Font Stack:** Segoe UI, Tahoma, Geneva, Verdana, sans-serif
- **Responsive:** Scales smoothly from mobile to desktop
- **Accessibility:** Supports `prefers-reduced-motion`

---

## 💾 Data Persistence

All activities use **browser localStorage** to persist user progress:

```javascript
// Checklists auto-save
localStorage.setItem('activity01-check1', JSON.stringify(true))
```

**Note:** Clearing browser cache/storage will reset progress. Consider exporting checklist state before clearing.

---

## 🔐 Legal & Ethical Framework

### Authorization Requirement

Every activity includes a legal warning:

> **⚠️ Authorization Required:** All hacking, penetration testing, forensics, and security testing activities described herein must be performed **only on systems you own or have explicit written authorization to test.** Unauthorized testing is illegal under the Computer Fraud and Abuse Act (CFAA) and similar international laws.

### Responsible Disclosure

Students are required to:
- Obtain signed authorization before any testing
- Document all findings securely
- Follow responsible disclosure timelines
- Report vulnerabilities to system owners, not public forums

### Professional Ethics

- Maintain confidentiality of findings
- Follow chain of custody procedures in forensics exercises
- Respect privacy in all simulated scenarios
- Understand the legal implications of each technique

---

## 📊 Curriculum Alignment

### Certification Mapping

**CompTIA Security+**
- Activities 01–04, 06, 09, 10

**CompTIA CEH (Certified Ethical Hacker)**
- All 10 activities cover CEH domains

**CompTIA CISSP**
- Activities 06–10 focus on defensive and governance aspects

**GIAC GCIH (Incident Handler)**
- Activities 06–09 provide incident response foundation

**Offensive Security OSCP**
- Activities 01–05 build skills for OSCP lab environment

### NIST Frameworks

- **NIST CSF:** All activities map to identify, protect, detect, respond, recover
- **NIST AI RMF:** AI Red Teaming content in separate branch (planned)
- **NIST SP 800-53:** Security controls in Activity 10

### MITRE Frameworks

- **MITRE ATT&CK:** Activities 01–05, 09 reference ATT&CK tactics/techniques
- **MITRE ATLAS:** AI threat modeling (planned extension)

---

## 🛠️ Customization & Extension

### Adding New Activities

1. **Copy a template:** Use `activity0X.html` as a base
2. **Update metadata:**
   - Title, badge (difficulty level)
   - Duration, tools required
   - Learning objectives
3. **Add content sections:**
   - Introduction
   - Key concepts and tables
   - Tool overview and code examples
   - 3–5 hands-on exercises
   - Submission checklist
4. **Update navigation:** Link from previous activity
5. **Update progress bar:** Calculate completion percentage

### Modifying Branding

Update the logo and colors in:
- **index.html:** Header logo, course cards
- **activity0X.html:** All activity pages (CSS variables)

```css
:root {
    --navy: #0F1419;        /* Update primary color */
    --cyan: #00D9FF;        /* Update accent color */
    --red: #DC3545;         /* Update advanced badge */
}
```

### Localizing for Other Institutions

1. Update logo and branding colors
2. Modify instructor name and credentials
3. Add institution-specific contact/support info
4. Customize code examples and tool references
5. Add links to your institution's lab environment

---

## 📝 Content Standards

For consistency and quality, all new content should follow:

- **Markdown formatting** for code examples
- **Consistent terminology** (see STANDARDS.md)
- **Real tools only** (no fictional software)
- **Legal disclaimers** on all offensive exercises
- **Accessibility:** WCAG 2.1 AA minimum
- **Mobile-responsive** design
- **Dark mode support** where applicable

See `docs/STANDARDS.md` for detailed guidelines.

---

## 🔄 Repo Naming Consideration

### Current: `CNM-CIST-Classes`

**Pros:**
- Clear institutional reference (CNM)
- Department clear (CIST = Computer Information Systems Technology)
- Scope obvious (Classes/courses)
- Professional and searchable

**Alternatives to consider:**

| Name | Pros | Cons |
|------|------|------|
| `CNM-Cybersecurity-Labs` | More specific focus | Longer |
| `cybersecurity-curriculum` | Generic, portable | Loses institutional identity |
| `red-team-bootcamp` | Modern, catchy | Doesn't reflect blue team content |
| `mastermind-rogue-labs` | Brand-aligned (your archetype) | Unclear institutional connection |
| `offensive-defensive-labs` | Describes both tracks | Generic |

**Recommendation:** **Keep `CNM-CIST-Classes`** — it's:
- ✅ Clear and searchable
- ✅ Institution-branded (important for CNM portfolios)
- ✅ Professional and official-sounding
- ✅ Future-proof if you add non-lab content later

If you want to emphasize the advanced/red team focus, consider a **repo description** instead:

```
Central New Mexico Community College cybersecurity curriculum: 
10 progressive labs spanning offensive security, forensics, and incident response.
```

---

## 🚀 Deployment Options

### Local Testing

```bash
# Python 3
python3 -m http.server 8000

# Node.js (http-server)
npx http-server -p 8000

# Ruby
ruby -run -ehttpd . -p8000
```

### GitHub Pages (Free)

1. Push to GitHub
2. Enable Pages in settings
3. Activity pages live at `https://username.github.io/CNM-CIST-Classes/`

### Institutional LMS

- **Canvas/Blackboard:** Embed as external tool or link
- **Moodle:** Upload as SCORM package (with modifications)
- **Custom Portal:** Embed in iFrame with proper CORS headers

### Offline Distribution

- Package as HTML export
- Distribute via USB or institution portal
- Works entirely offline (no external dependencies)

---

## 📚 Additional Resources

### For Instructors

- **Setup Guide:** `docs/SETUP.md` — Lab environment configuration
- **Certificate Paths:** `docs/CERTIFICATE_PATHS.md` — Cert alignment
- **Standards:** `docs/STANDARDS.md` — Content and design guidelines

### For Students

- **Activity 01–10:** Self-contained, start with Activity 01
- **Prerequisite Knowledge:** CompTIA Security+ or equivalent recommended
- **Lab VMs:** Links in each activity to HackTheBox, TryHackMe, DVWA

### External References

- **Volatility Framework:** https://github.com/volatilityfoundation/volatility
- **Metasploit:** https://www.metasploit.com/
- **NIST SP 800-72:** Digital Evidence Guidelines
- **MITRE ATT&CK:** https://attack.mitre.org/
- **OWASP Top 10:** https://owasp.org/

---

## 🤝 Contributing

Contributions are welcome! Please see `CONTRIBUTING.md` for:

- Code style and standards
- How to submit new activities
- Reporting issues and bugs
- Pull request process

---

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**.

- ✅ **Allowed:** Educational use, modification for classroom, attribution
- ❌ **Not allowed:** Commercial distribution, claiming as your own

See `LICENSE.md` for full terms.

---

## 📞 Support & Feedback

- **Issues/Bugs:** GitHub Issues
- **Feature Requests:** GitHub Discussions
- **Contact:** Frank | CISSP, SecAI Certified
- **Institution:** Central New Mexico Community College

---

## 🗂️ Version History

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2024-07 | Activities 01–07 complete, 08–10 in progress |
| v0.9 | 2024-06 | Activities 01–05 (offensive track) complete |
| v0.1 | 2024-05 | Project structure and design system established |

---

**Last Updated:** July 2024  
**Status:** Active Development (Activities 08–10 in progress)  
**Contributors:** Frank (Instructor, CNM Cybersecurity Program)

---

## 🎯 Future Roadmap

- [ ] Activities 08–10 completion
- [ ] AI Red Teaming branch (prompt injection, LLM attacks)
- [ ] Video walkthroughs for each activity
- [ ] Automated lab environment setup (Terraform/Docker)
- [ ] LMS integration (Canvas/Blackboard SCORM)
- [ ] Interactive code sandbox (CodePen-style)
- [ ] Discussion forum/collaborative features
- [ ] Mobile app companion

---

**Built with ❤️ by Frank | CISSP, SecAI Certified**  
*Empowering cybersecurity professionals, one lab at a time.*
