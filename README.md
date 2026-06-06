# Claude Agent SDK — Course Notebooks

This repository contains the solution notebooks for the Udemy course:
**"Claude Agent SDK: Build Production AI Agents in Python"**

---

## How to Use

Each notebook is self-contained. Click the **Open in Colab** button for the
lecture you are working on. No local setup required.

---

## Section 2 — Your First Agent

| Lecture | Notebook |
|---|---|
| 2.1 — Setting Up Colab & Your API Key | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-2-your-first-agent/2.1-setting-up-colab-and-api-key.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 2.2 — Writing Your First query() Call | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-2-your-first-agent/2.2-writing-your-first-query-call.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 2.3 — Reading Agent Messages & the Result Stream | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-2-your-first-agent/2.3-reading-agent-messages-and-result-stream.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 2.4 — Hands-On: Build a File Explorer Agent | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-2-your-first-agent/2.4-file-explorer-agent.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |

---

## Section 3 — Built-In Tools Deep Dive

| Lecture | Notebook |
|---|---|
| 3.1 — File Tools: Read, Write, Edit | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-3-built-in-tools-deep-dive/3.1-file-tools-read-write-edit.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 3.2 — Shell Tools: Bash & Monitor | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-3-built-in-tools-deep-dive/3.2-shell-tools-bash-and-monitor.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 3.3 — Search Tools: Glob & Grep | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-3-built-in-tools-deep-dive/3.3-search-tools-glob-and-grep.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 3.4 — Web Tools: WebSearch & WebFetch | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-3-built-in-tools-deep-dive/3.4-web-tools-websearch-and-webfetch.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 3.5 — User Interaction: AskUserQuestion | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-3-built-in-tools-deep-dive/3.5-user-interaction-askuserquestion.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 3.6 — Hands-On: Build a Codebase TODO Summarizer Agent | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-3-built-in-tools-deep-dive/3.6-todo-summarizer-agent.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |

---

## Section 4 — Permissions & Safety

| Lecture | Notebook |
|---|---|
| 4.1 — Understanding allowed_tools and Permission Modes | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-4-permissions-and-safety/4.1-allowed-tools-and-permission-modes.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 4.2 — Read-Only Agents vs Auto-Edit Agents | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-4-permissions-and-safety/4.2-readonly-vs-autoedit-agents.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 4.3 — Blocking Dangerous Operations | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-4-permissions-and-safety/4.3-blocking-dangerous-operations.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 4.4 — Hands-On: Build a Safe Code Review Agent | <a href="https://colab.research.google.com/github/gopidon/claude-agent-sdk-course-code/blob/main/section-4-permissions-and-safety/4.4-safe-code-review-agent.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |

---

## Requirements

- A Google account — for Google Colab
- An Anthropic API key — get yours at https://platform.claude.com/
- No local setup required — everything runs in the cloud

---

## API Key Setup

Each notebook reads your API key from Colab Secrets:

1. Open the notebook in Colab
2. Click the 🔑 key icon in the left sidebar
3. Add a secret named `ANTHROPIC_API_KEY`
4. Paste your Anthropic API key as the value
5. Run the notebook from the top

---

## Model

All notebooks use `claude-haiku-4-5` by default — the fastest and most
cost-effective Claude model. You can change this by updating the
`MODEL_NAME` variable at the top of any notebook.

For the latest available models visit:
https://platform.claude.com/docs/en/about-claude/models/overview

---

## Course Link

Enroll in the course on Udemy: [Claude Agent SDK: Build Production AI Agents in Python](link)

---

## License

The notebooks in this repository are for educational purposes and intended
for use by enrolled students of the course.
