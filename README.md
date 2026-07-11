# Zero to Hero: The Free Cybersecurity Roadmap

> Skills over certificates. Understanding over memorization. Building over consuming.

This repository is a self-paced, project-based path from **absolute zero** to **entry/intermediate security professional**, built entirely from free, official, and open-source resources. It is designed to be forked, followed, and turned into a public portfolio.

---

## How This Repo Works

- Every **phase** lives in `phases/` as its own Markdown file (e.g. `phase-00-mindset-learning-system.md`).
- Every phase is self-contained: objectives, theory, labs, projects, checkpoints, and a capstone.
- You do not move to the next phase until you pass that phase's checkpoints.
- Everything you produce — notes, screenshots, write-ups, scripts, rules — goes into **your own fork**, not this repo. This repo is the map. Your fork is the journey.
- Phases are released and refined incrementally — this is phase 1 of the *repo itself* being built. Check back for phases 1–49 as they're added.

### The 30/70 Rule
30% theory (just enough to know *why*), 70% hands-on (labs, breaking things, rebuilding them).

### The Feynman Requirement
Every topic ends with you writing your own explanation, at multiple levels (5-year-old → SOC analyst → CISO), in your own GitHub. If you can't explain it simply, you don't understand it yet.

---

## Suggested Fork Structure

When you fork this roadmap to track your own progress, mirror this structure in your fork:

```
your-cybersec-journey/
├── README.md                      # your intro, goals, contact/portfolio links
├── progress-tracker.md            # phase-by-phase completion tracker
├── learning-journal/
│   ├── weekly-reflections/
│   └── monthly-reviews/
├── labs/
│   └── phase-00/ phase-01/ ...    # raw lab work, configs, pcaps, logs
├── projects/
│   └── (one folder per capstone/mini-capstone)
├── writeups/
│   └── ctf/ incidents/ research/
├── notes/
│   ├── cheatsheets/
│   ├── diagrams/
│   └── mind-maps/
├── scripts-and-tools/
├── detection-rules/
│   ├── sigma/
│   └── yara/
├── playbooks/
├── resources/
│   ├── books/
│   └── papers/
└── portfolio/
    ├── resume/
    └── interview-notes/
```

---

## Progress Tracking System

Each phase tracks, at minimum:
- Completion %
- Skills earned
- Hours invested
- Labs / Projects completed
- GitHub commits made for that phase
- A one-paragraph weekly reflection

See `templates/progress-tracker.md` for a ready-to-copy table.

---

## The Full Roadmap (49 Phases)

| # | Phase | Focus |
|---|-------|-------|
| 0 | Mindset & Learning System | How to learn this, and not quit |
| 1 | Computer Fundamentals | Hardware, binary, how a computer actually works |
| 2 | Operating Systems | Processes, memory, filesystems, boot process |
| 3 | Networking | OSI/TCP-IP, routing, DNS, packet analysis |
| 4 | Linux | CLI mastery, permissions, services, scripting |
| 5 | Windows | Registry, services, AD basics, PowerShell |
| 6 | Git & GitHub | Version control, portfolio workflow |
| 7 | Python | Scripting for security automation |
| 8 | Web Technologies | HTTP, HTML/JS, how the web actually works |
| 9 | Databases | SQL, NoSQL, and how they get breached |
| 10 | Virtualization | VirtualBox/VMware, building your home lab |
| 11 | Cloud Fundamentals | AWS/Azure/GCP free-tier basics |
| 12 | Security Fundamentals | CIA triad, risk, controls, frameworks |
| 13 | SOC Foundations | Alerts, triage, ticketing, shift life |
| 14 | Threat Intelligence | IOCs, TTPs, MITRE ATT&CK in practice |
| 15 | Incident Response | IR lifecycle, playbooks, tabletop exercises |
| 16 | Digital Forensics | Disk, memory, and file-system forensics |
| 17 | Malware Analysis | Static/dynamic analysis basics |
| 18 | Detection Engineering | Writing and testing detections |
| 19 | SIEM | Wazuh/Elastic/Security Onion in a home lab |
| 20 | Threat Hunting | Hypothesis-driven hunting |
| 21 | Active Directory Security | Attacking and defending AD |
| 22 | Windows Internals | Processes, tokens, the kernel |
| 23 | Linux Security | Hardening, auditd, SELinux/AppArmor |
| 24 | Web Security | OWASP Top 10, PortSwigger labs |
| 25 | API Security | REST/GraphQL abuse and defense |
| 26 | Network Security | Firewalls, IDS/IPS, segmentation |
| 27 | Cryptography | Applied crypto, common failures |
| 28 | Reverse Engineering | Assembly, disassemblers, debuggers |
| 29 | Red Team Basics | Recon, initial access, C2 concepts |
| 30 | Blue Team Operations | Detection, containment, eradication |
| 31 | Purple Team | Adversary emulation + detection validation |
| 32 | Cloud Security | IAM misconfig, cloud attack paths |
| 33 | Container Security | Docker hardening and escapes |
| 34 | Kubernetes Security | RBAC, network policy, cluster attacks |
| 35 | Identity Security | SSO, MFA, identity attack paths |
| 36 | Email Security | SPF/DKIM/DMARC, phishing analysis |
| 37 | Endpoint Security | EDR concepts, Sysmon, telemetry |
| 38 | Detection Engineering (Advanced) | Sigma at scale, detection-as-code |
| 39 | Automation | SOAR concepts, scripting response |
| 40 | Security Engineering | Secure architecture, threat modeling |
| 41 | DFIR (Advanced) | Full-scope investigations |
| 42 | Bug Hunting | Bug bounty methodology (free scopes) |
| 43 | Vulnerability Research | Finding and documenting vulns |
| 44 | Secure Coding | Writing code that doesn't get you breached |
| 45 | DevSecOps | Security in CI/CD |
| 46 | Threat Emulation | Building adversary simulation exercises |
| 47 | Enterprise Security | Governance, policy, compliance |
| 48 | Advanced Specializations | Pick your track and go deep |
| 49 | Final Master Capstone | Full enterprise attack + defend simulation |

---

## Philosophy Reminder

This roadmap will never ask you to pay for anything. If a phase ever suggests a resource that requires a credit card or hidden paywall, that's a bug — open an issue.
**Status:** Phase 0 complete and below. Phases 1–49 are released incrementally.

[Phase 0 Mindset Learning System →](../phase-00-mindset-learning-system.md)
