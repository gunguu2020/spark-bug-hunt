# 🕵️‍♂️ Spark Bug Hunt

Welcome to **Spark Bug Hunt**! This is my very first project created entirely with the help of an AI Agent. Even with no prior coding experience, I was able to set up a sophisticated, self-evolving AI system on Windows.

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

---
*Created with ❤️ by George & Gemini CLI*
