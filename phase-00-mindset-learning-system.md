<div align="center">

# 🧠 Phase 0 — Mindset & Learning System

![Difficulty](https://img.shields.io/badge/difficulty-absolute%20zero-brightgreen)
![Hours](https://img.shields.io/badge/est.%20hours-10--15-blue)
![Prereqs](https://img.shields.io/badge/prerequisites-none-lightgrey)
![Cost](https://img.shields.io/badge/cost-%240.00-brightgreen)

*Before you touch a single tool, you need the operating system for your brain.*

[← Back to Roadmap](../README.md) · [Next: Phase 1 →](#-next-phase-1--computer-fundamentals)

</div>

---

> **Why this phase has almost no "hacking" in it:** this is the phase most self-taught learners skip — and the reason most of them quit around month three. Skip it and you'll feel that later.

## 📌 On This Page

- [Learning Objectives](#-learning-objectives)
- [Setup: Prerequisites, Hours, Tools, Accounts](#-setup)
- [Core Lessons](#-core-lessons) — 5 lessons
- [Real-World Case Studies](#-real-world-case-studies)
- [Free Platforms Preview](#-free-ctf--practice-platforms-preview)
- [Reference: Docs, Cheat Sheets, Books](#-documentation--references-for-this-phase)
- [Career Skills & Interview Questions](#-career-skills)
- [✅ Progress Checklist](#-progress-checklist)
- [🚦 Checkpoints](#-checkpoints)
- [🎓 Final Assessment & Portfolio](#-final-assessment)
- [📦 GitHub Deliverables](#-github-deliverables-summary)
- [💭 Reflection](#-reflection-questions-phase-wide)

---

## 🎯 Learning Objectives

By the end of this phase, you will be able to:

1. Explain why this roadmap is 30% theory / 70% practice, and apply that ratio to your own study sessions
2. Use the **Feynman Technique** to test whether you actually understand something
3. Set up a personal knowledge base you'll use for the entire roadmap
4. Create your GitHub account and first public learning repository
5. Read technical documentation (RFCs, vendor docs, MITRE ATT&CK) efficiently instead of passively
6. Design a realistic weekly study schedule and track it honestly
7. Recognize the four most common reasons self-taught learners quit, and have a countermeasure for each

---

## 🧰 Setup

<table>
<tr><td><strong>Prerequisites</strong></td><td>None — this phase assumes zero background.</td></tr>
<tr><td><strong>Estimated Hours</strong></td><td>10–15 hours over 5–7 days. Intentionally light — this builds scaffolding, not exhaustion.</td></tr>
</table>

### Required Software

| Tool | Purpose | Cost |
|------|---------|:---:|
| A modern browser (Firefox/Chrome) | Research, labs | Free |
| [Visual Studio Code](https://code.visualstudio.com/) | Notes, later code editing | Free |
| [Obsidian](https://obsidian.md/) *or* plain Markdown in VS Code | Your personal knowledge base | Free |
| [Git](https://git-scm.com/) | Version control (deep dive in Phase 6, install now) | Free |

### Required Hardware
Any laptop/desktop from the last ~8 years, 8GB+ RAM recommended. No dedicated lab hardware needed yet.

### Required Accounts *(all free)*
- ✅ [GitHub](https://github.com/) — this is your portfolio for the *entire* roadmap
- 🔵 *Optional:* TryHackMe free tier, or a security Discord community, for accountability

---

## 📚 Core Lessons

<details open>
<summary><h3>0.1 — The Security Mindset</h3></summary>

**What is it?**
The habit of asking *"how could this be abused, and how would I know if it was?"* about every system you encounter — not just when you're told to.

**Why does it exist?**
Every system is built assuming normal, well-intentioned use. Security work studies what happens outside that assumption — attackers succeed by finding the gap between what a designer imagined and what a system actually allows.

**How does it work?**
A habit of asking two paired questions, constantly:
- **Offense framing:** "If I wanted to break this, misuse it, or make it do something it wasn't meant to do, where would I start?"
- **Defense framing:** "If someone were doing that right now, what evidence would it leave, and who would notice?"

**Real-world examples**
- The Target 2013 breach began with stolen credentials from a third-party HVAC vendor — a gap between "who has network access" and "who *should*."
- Stuxnet exploited the assumption that air-gapped industrial systems were safe from network-borne malware — the gap was physical media (USB), not the network.

**Common mistakes**
- Treating security as a checklist instead of a way of thinking
- Assuming attackers only use "hacker" tools — most breaches start with phishing, reused passwords, or misconfiguration
- Believing you need to know everything before applying this mindset — start small, today

**Security implications**
No direct attack yet — this is the lens for every phase from here on. The habit of pairing offense/defense questions is what separates tool-memorizers from people who can reason about a system they've never seen.

> **🔬 Practical Lab**
> Pick three systems you interact with today (apartment key fob, email login, vending machine, QR-code menu). For each, write:
> 1. What is this system trying to prevent?
> 2. One way someone could bypass that assumption
> 3. One way the owner might detect that bypass

> **⚔️ Challenge**
> Without looking anything up, write down what you think the *weakest link* is in your own daily digital life. Be honest — this is diagnostic, not graded.

> **📖 Research Assignment**
> Read the [MITRE ATT&CK](https://attack.mitre.org/) "Getting Started" page. Understand what the matrix *is* and why it's organized as tactics (why) vs. techniques (how) — don't memorize yet.

> **📝 GitHub Assignment**
> `notes/phase-00/security-mindset.md` — your three-system exercise + weakest-link reflection.

> **💭 Reflection**
> - What surprised you about how easy it was to find a gap once you looked for one?
> - How would an attacker abuse the systems you picked? How would you detect it? Defend it?

</details>

<details>
<summary><h3>0.2 — The Learning System (How You'll Actually Retain This)</h3></summary>

**What is it?**
A repeatable process for taking in technical material, testing your own understanding, and retaining it long-term instead of forgetting it in a week.

**Why does it exist?**
Cybersecurity has a high "forgetting rate" for self-taught learners because so much is procedural (commands, flags, syntax). Passive reading/video-watching feels productive but produces almost no durable retention.

**How does it work?**
Three techniques, used together every phase:

1. **The Feynman Technique** — explain a concept from scratch, in your own words, at escalating levels:
   `5-year-old → high schooler → university student → SOC Analyst → SysAdmin → CISO`
   Getting stuck at any level pinpoints exactly where your understanding has a hole.
2. **Active Recall** — close your notes and reproduce the concept from memory, then check what you missed. Feels harder than re-reading; is dramatically more effective.
3. **Spaced Repetition** — revisit a concept after 1 day, 3 days, 7 days, ~30 days. A recurring calendar reminder or a "review" line in your weekly reflection is enough — no special software required.

**Real-world examples**
Certification bodies and university programs increasingly build spaced review directly into curricula, because "cram and forget" produces practitioners who pass an exam but can't perform the job.

**Common mistakes**
- Highlighting/re-reading and mistaking familiarity for understanding
- Watching hours of tutorials without ever closing the video and trying it
- Trying to learn everything before practicing anything — remember the 30/70 rule

> **🔬 Practical Lab**
> Take the ATT&CK concept from Lesson 0.1. Without notes, explain in writing what it is (a) to a 5-year-old and (b) to a SOC Analyst. Compare the two.

> **⚔️ Challenge**
> Pick a topic you sort-of know (Wi-Fi, email delivery, password checks). Feynman-explain it at all six levels, in one sitting, no research. Note exactly where you get stuck.

> **📖 Research Assignment**
> Look up "the forgetting curve" and "spaced repetition" — broad reading across a few sources is fine here.

> **📝 GitHub Assignment**
> `notes/phase-00/learning-system.md` — your note-taking tool, spaced-repetition plan, and Feynman write-up.

> **💭 Reflection**
> - Where did you get stuck Feynman-explaining something you thought you knew?
> - Did active recall feel harder than re-reading? Why is that a good sign?

</details>

<details>
<summary><h3>0.3 — Building Your Public Learning System (Notes + GitHub)</h3></summary>

**What is it?**
The infrastructure for documenting everything in this roadmap: a personal notes system plus a public GitHub repo that becomes your portfolio.

**Why does it exist?**
"Learning in public" forces the Feynman technique (no sloppy explanations for a public audience) and produces a visible portfolio — which matters more to employers than a course-completion list.

**How does it work?**

*Notes system* — one consistent structure from day one:
```
notes/
  phase-00/
    security-mindset.md
    learning-system.md
  cheatsheets/
  diagrams/
```
Template per note: **Topic → What/Why/How → my own example → open questions.**

*GitHub portfolio:*
1. Create a GitHub account
2. Create a new **public** repo (e.g. `my-cybersecurity-journey`)
3. Add a README describing your goal, linking this roadmap
4. Commit your Phase 0 notes

You don't need Git expertise yet (Phase 6 covers it deeply) — GitHub's web "upload files" button is a valid start, or use the command reference below if you're already comfortable with a terminal.

**Real-world examples**
Hiring managers for SOC/junior pentest roles frequently rate a documented GitHub portfolio above a certificate alone — it demonstrates communication, a core and underrated security skill.

**Common mistakes**
- Keeping the repo private "until it's good enough" — public-from-day-one is the point
- Over-engineering the notes app choice instead of starting
- Committing secrets, API keys, or personal info into a public repo

**Security implications**
Your first real "treat your own system like an attacker would" exercise: check what you're exposing before every push — including lab IPs, credentials, or client data in later phases.

> **🔬 Practical Lab**
> 1. Create your public GitHub repo
> 2. Write and commit a root `README.md` with your goals
> 3. Commit the two notes files from Lessons 0.1 and 0.2

> **⚔️ Challenge**
> Write your repo's README as if a hiring manager reads it in six months. What does it say about *how* you learn, not just what you studied?

> **📖 Research Assignment**
> Skim GitHub Docs — "About README files."

> **📝 GitHub Assignment**
> Your live repo *is* the deliverable.

> **💭 Reflection**
> - How did it feel publishing imperfect, public notes?
> - What's one thing in your repo you'd be slightly embarrassed to show a future employer — and why?

</details>

<details>
<summary><h3>0.4 — Reading Documentation Like a Professional</h3></summary>

**What is it?**
A deliberate technique for extracting what you need from dense references (RFCs, vendor docs, MITRE ATT&CK, NIST, man pages) instead of reading cover-to-cover.

**Why does it exist?**
Most phases point you at primary documentation, not blog posts *about* it. Navigating this material well is itself a core professional skill.

**How does it work?** — a three-pass approach:
1. **Skim pass** — headers/TOC only, build a map of what's where
2. **Targeted pass** — go directly to the relevant section
3. **Verification pass** — re-read slowly for precise language (RFCs define MUST/SHOULD/MAY with specific legal-like meaning)

**Real-world examples**
RFC 2119 formally defines MUST/SHOULD/MAY — missing that distinction is a common beginner mistake reading protocol RFCs in Phase 3.

**Common mistakes**
- Reading an entire RFC/NIST doc front-to-back before having a specific question
- Trusting a summarizing blog post over the primary source when they disagree
- Skipping documentation for videos, then being stuck when a question the video didn't cover comes up

**Security implications**
Misreading documentation causes real misconfigurations later — e.g. misunderstanding a firewall's default behavior or a permission model's precedence rules.

> **🔬 Practical Lab**
> Using the three-pass method, read MITRE ATT&CK's definition of Tactic vs. Technique. Answer in two sentences: what's the actual difference?

> **⚔️ Challenge**
> Find one unfamiliar man page (or browse [man7.org](https://man7.org/linux/man-pages/)), e.g. `stat`. Using skim + targeted pass only, find one surprising thing it does.

> **📖 Research Assignment**
> Read RFC 2119 (short) — you'll reference this understanding throughout networking/protocol phases.

> **📝 GitHub Assignment**
> `notes/phase-00/reading-documentation.md` — your Tactic-vs-Technique answer + man-page finding.

> **💭 Reflection**
> - What's different about reading with a specific question in mind vs. reading to "learn the topic generally"?

</details>

<details>
<summary><h3>0.5 — Designing a Study System You'll Actually Keep</h3></summary>

**What is it?**
A realistic weekly schedule and honest tracking system sized to your actual life, not an idealized one.

**Why does it exist?**
The #1 reason self-taught learners quit isn't lack of intelligence — it's an unsustainable pace leading to burnout and guilt. A sustainable pace beats an intense one you abandon in three weeks.

**How does it work?**
1. Be honest about realistically sustainable weekly hours (your *average* week, not your best one)
2. Block that time like a real appointment
3. Use the progress tracker weekly — to notice patterns, not to judge yourself
4. Plan for missed weeks in advance — a missed week isn't a failed roadmap; ignoring the tracker is the real warning sign

**Real-world examples**
Consistent, moderate practice sustained over months reliably outperforms sporadic high-intensity bursts — true for languages, instruments, and this discipline alike.

**Common mistakes**
- Scheduling 20+ hrs/week in month one out of excitement, quitting in month two
- Treating a missed day as a reason to abandon the tracker entirely
- Comparing your pace to someone else's public progress instead of your own baseline

> **🔬 Practical Lab**
> Fill out your weekly schedule block and your first `progress-tracker.md` entry — honestly, not aspirationally.

> **⚔️ Challenge**
> Write down the single most likely reason *you* might quit. Write one countermeasure now, while motivated.

> **📖 Research Assignment**
> None required — this lesson is self-knowledge, not external reading.

> **📝 GitHub Assignment**
> `notes/phase-00/study-system.md` — your filled tracker + quit-risk/countermeasure note.

> **💭 Reflection**
> - What's the realistic (not aspirational) hours/week you can sustain?
> - What will you do the first time you miss a scheduled session?

</details>

---

## 🏢 Real-World Case Studies

- **The "cert collector" trap** — accumulating certifications while unable to perform basic hands-on tasks in a technical interview screen is a well-known, avoidable failure mode. This roadmap's portfolio requirement exists specifically to prevent it.
- **Documentation as a career asset** — many well-known security researchers built their reputation (and job offers) through public write-ups and blogs, not certificates alone.

## 🎮 Free CTF / Practice Platforms (Preview)

*You won't need these deeply until later phases — free accounts now are optional.*

| Platform | Use | Link |
|---|---|---|
| OverTheWire — Bandit | Linux fundamentals (starts Phase 4) | [overthewire.org](https://overthewire.org/wargames/bandit/) |
| PicoCTF | Beginner-friendly, ongoing CTF | [picoctf.org](https://picoctf.org/) |
| TryHackMe | Free rooms available (never required) | [tryhackme.com](https://tryhackme.com/) |
| Hack The Box Academy | Free modules available | [academy.hackthebox.com](https://academy.hackthebox.com/) |

## 📖 Documentation & References for This Phase

- [MITRE ATT&CK](https://attack.mitre.org/)
- [GitHub Docs — About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [RFC 2119 — Key words for use in RFCs](https://www.rfc-editor.org/rfc/rfc2119)
- [Linux man pages online](https://man7.org/linux/man-pages/)

<details>
<summary><strong>📋 Cheat Sheets</strong></summary>

**Markdown Quick Reference**
```
# Heading 1
## Heading 2
**bold**   *italic*
- bullet list
1. numbered list
[link text](https://example.com)
`inline code`
```

**Minimal Git Command Reference** *(deep dive in Phase 6)*
```
git init                     # start a new local repo
git add .                    # stage all changes
git commit -m "message"      # commit staged changes
git remote add origin <url>  # link to your GitHub repo
git push -u origin main      # push to GitHub
```

</details>

**Free Books:** *The Linux Command Line* by William Shotts (free PDF from author's site — used starting Phase 4). MITRE ATT&CK and NIST publications function as free canonical "textbooks" throughout this roadmap.

**Open Source Tools Introduced:** Git · Obsidian · VS Code

---

## 💼 Career Skills

- Written technical communication — your notes and README *are* this skill, from day one
- Honest self-assessment and pacing — a real, assessed skill in SOC/IR roles where burnout is an operational risk

<details>
<summary><strong>🎤 Interview Questions (Yes, Even for Phase 0)</strong></summary>

- "Walk me through how you learn a new technology you've never used before."
- "Tell me about a time you had to explain something technical to a non-technical person."
- "How do you keep your skills current?"

Answering these using your *own* Phase 0 habits beats reciting a certification list.

</details>

**Common Mistakes (Phase-Wide):** picking the "perfect" notes app instead of starting · keeping notes private "until polished" · rushing this phase as filler (the habits here are load-bearing for all 49 phases)

---

## ✅ Progress Checklist

- [ ] GitHub account created
- [ ] Public learning repository created with a README
- [ ] Notes system chosen, first four notes committed (Lessons 0.1–0.4)
- [ ] Progress tracker filled out with an honest weekly schedule
- [ ] Quit-risk reflection written

---

## 🚦 Checkpoints

| Checkpoint | Pass Condition |
|---|---|
| **Knowledge Check** | Can you explain Tactic vs. Technique in ATT&CK, and MUST/SHOULD/MAY in an RFC, from memory? |
| **Practical Check** | Does your GitHub repo exist, is it public, does it have real commits? |
| **Lab Check** | Completed the three-system mindset exercise + documentation three-pass exercise? |
| **Project Check** | Could you find a note from this phase again in 30 seconds? |
| **GitHub Check** | Are all five `notes/phase-00/*.md` files committed and pushed? |
| **Documentation Check** | Do your notes follow Topic → What/Why/How → example → open questions (not copy-paste)? |
| **Feynman Check** | Explain one random concept from this phase, aloud, alone, under 90 seconds, no notes |
| **Peer Review** *(if applicable)* | Can someone else follow your README and notes without you explaining verbally? |
| **Troubleshooting** | Git push auth error? GitHub needs a Personal Access Token or SSH key, not your account password (full coverage in Phase 6) |

---

## 🎓 Final Assessment

Write `notes/phase-00/final-assessment.md`, in your own words (no copy-paste from this roadmap):

1. What is the security mindset, with your own original example?
2. What is the Feynman Technique, and why does getting "stuck" matter?
3. What is your realistic weekly study schedule, and your plan for the first missed week?

## 🏆 Portfolio Project

Your live, public GitHub repository **is** the Phase 0 portfolio project — the infrastructure every future phase's projects will live inside.

## 📦 GitHub Deliverables (Summary)

```
README.md                                  (repo root)
progress-tracker.md
notes/phase-00/security-mindset.md
notes/phase-00/learning-system.md
notes/phase-00/reading-documentation.md
notes/phase-00/study-system.md
notes/phase-00/final-assessment.md
```

## 💭 Reflection Questions (Phase-Wide)

- What surprised you about this phase, given it had almost no "technical hacking" in it?
- What's the one habit here you're most likely to drop under time pressure — and your plan for that?
- How would you explain, in one sentence, why this phase exists before Phase 1 even starts?

---

<div align="center">

### ▶ Next: Phase 1 — Computer Fundamentals

*(coming soon)*

[← Back to Roadmap](../README.md)

</div>
