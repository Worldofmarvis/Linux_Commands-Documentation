# 🐧 Linux Commands for CTF & Penetration Testing

A curated, example-driven documentation of essential Linux commands I've mastered during my cybersecurity journey. Each guide includes practical CTF scenarios, not just man-page repeats.

## 📖 Table of Contents
- [Why This Repo?](#why-this-repo)
- [How to Use](#how-to-use)
- [Contributing / Feedback](#contributing--feedback)

## 🎯 Why This Repo?
While studying for CTFs (Capture The Flag) and Linux privilege escalation, I realized most command references lack *real attack/defense context*. This repo fills that gap with:
- 🔍 Real CTF use-cases (e.g., using `strings` on a suspicious binary)
- 🛠️ One-liners & flags you'll actually need under time pressure
- ⚠️ Common pitfalls (e.g., SSH key permissions)

## 📂 Commands Covered
| Command | Focus Area | CTF Example |
|---------|-----------|--------------|
| [SSH](The%20Secure%20Shell%20(SSH).md) | Remote access, tunneling | Forward a local port through a compromised jump host |
| [wget](The%20Wget.md) | File transfer, mirroring | Download a reverse shell payload with `--no-check-certificate` |
| [strings](The%20strings.md) | Binary analysis, forensics | Extract hidden flags from an ELF binary |

> *More coming soon...*

## 🚀 How to Use
Clone and browse:
```bash
git clone https://github.com/Worldofmarvis/CTF-Documentation.git
cd CTF-Documentation
