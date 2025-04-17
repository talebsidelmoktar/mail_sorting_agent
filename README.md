# 🦇 Alfred the Email Butler Agent

An intelligent agent built with `LangGraph` and `OpenAI GPT-4o`, acting as **Alfred the Butler** to filter and handle Bruce Wayne’s (aka Batman’s) email inbox.

Alfred reads incoming emails, classifies them as spam or not, drafts polite responses for Mr. Wayne, and notifies him when appropriate — all in a stately and efficient manner.

---

## 🧠 Features

- 📥 Reads and logs details of incoming emails
- 🧹 Classifies emails as **SPAM** or **HAM**
- ✍️ Drafts professional replies for Mr. Wayne’s review
- 📤 Notifies Bruce Wayne with the message and draft
- ❌ Moves spam to a "spam folder"
- 🧱 Modular and extensible LangGraph workflow

---

## 🛠️ Tech Stack

| Component        | Role                                  |
|------------------|----------------------------------------|
| `LangGraph`      | Agentic graph engine                   |
| `OpenAI GPT-4o`  | LLM for classification and drafting    |
| `LangChain`      | Prompt & message orchestration         |
| `Python`         | Core logic implementation              |

---

## 🧩 Workflow Diagram

```text
START
  ↓
read_email
  ↓
classify_email
  ↓─────────────┐
 SPAM          HAM
  ↓              ↓
handle_spam   drafting_response
                ↓
           notify_mr_wayne
                ↓
               END
