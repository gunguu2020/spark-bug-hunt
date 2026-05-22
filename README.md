# 🕵️‍♂️ Spark Bug Hunt
Welcome to **Spark Bug Hunt** — a structured quality assurance initiative focused on stress-testing Spark Intelligence,a self-evolving AI runtime. This repository documents my systematic exploration of the Spark CLI, tracking bugs, edge cases, and behavioral anomalies discovered during real-world usage on a Windows environment.

## 🚀 What is Spark Intelligence?
Spark Intelligence (by @Spark_coded) is a "living intelligence" layer for AI agents. Unlike traditional chatbots, Spark:
- **Learns as you work:** It captures memory from coding sessions.
- **Self-Evolves:** It uses a "recursive loop" to improve its own insights.
- **Compounds Knowledge:** It builds a local "Mind" that helps future AI agents understand the project better.

## 🛠 Tools I Used
To get this running, I collaborated with the **Gemini CLI** and utilized the following modern tech stack:
- **Gemini CLI:** The AI agent that guided me through the entire installation.
- **Node.js:** The JavaScript runtime that powers the CLI tools.
- **Git:** Used for version control and cloning the Spark codebase.
- **Python 3.14:** The engine that runs the Spark Intelligence services.

## 📥 Installation Steps
I followed these steps to get everything running on my Windows machine:

1. **Environment Setup:** Installed Node.js and the Gemini CLI.
2. **Prerequisite Check:** Used the Gemini CLI to identify that I needed Git and Python.
3. **One-Command Setup:** Ran the following PowerShell command to bootstrap the system:
```powershell
   irm https://raw.githubusercontent.com/vibeforge1111/vibeship-spark-intelligence/main/install.ps1 | iex
```
4. **Verification:** Confirmed the system was healthy using `spark doctor`.

## 🔍 The Bug Hunt
The "Bug Hunt" is my initiative to explore the Spark Intelligence ecosystem. As a first-time user, I am documenting my journey, testing the limits of the AI's memory, and identifying any issues or "bugs" that arise during normal use.

## 📝 Bug Log
I use this section to track any unexpected behaviors or improvements I find.

| ID | Date | Description | Status |
|----|------|-------------|--------|
| 001 | 2026-05-22 | Initial setup successful; no bugs found yet. | ✅ Resolved |
| 002 | 2026-05-22 | `spark learn` command crashes with `AttributeError: 'NoneType' object has no attribute 'insight'`. Run `spark learn meta "This is a test"` to reproduce. Breaks manual learning feature. | 🔴 High Priority |
| 003 | 2026-05-22 | Config type validation failure. `spark config set advisor.max_items 'any-text'` accepts a string instead of a number. Will cause crashes when the setting is used. | 🟡 Medium Priority |
| 004 | 2026-05-22 | Missing "Chips" directory. Running `spark chips list` returns `Chips directory not found`. Folder is not created during standard installation, blocking new users from accessing domain chips. | 🟡 Medium Priority |
| 005 | 2026-05-22 | Configuration Desync (Silent Failure). `spark config set` confirms "Saved successfully" but `spark advisory doctor` ignores the change and uses old values. User believes system is configured but AI silently ignores them. Reproduce: Set `advisory.preferred_provider` to any value, then run `spark advisory doctor`. | 🔴 High Priority |
| 006 | 2026-05-22 | Inconsistent Project Status. After running `spark project answer` on a decision question, global "Questions answered" counter increments but "Decisions" count stays at zero. System memory is inconsistent between counters. Reproduce: Answer a [decision] question and check `spark project status`. | 🟡 Medium Priority |

---
*Created with ❤️ by George & Gemini CLI*
