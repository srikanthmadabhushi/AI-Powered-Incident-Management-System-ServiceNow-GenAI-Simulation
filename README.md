# 🚀 AI-Powered Incident Management System (ServiceNow + GenAI Simulation)

---

## 📌 Overview

This project demonstrates an **AI-driven Incident Management System** built on the ServiceNow platform. It simulates **Generative AI (Now Assist-like capabilities)** to automate incident classification, resolution suggestions, and ticket creation through a conversational interface.

The solution combines **AI logic, automation, and user interaction** to improve IT service workflows and reduce manual effort.

---

## 🎯 Key Features

### 🤖 AI Decision Engine
- Dynamic **incident classification (NLP-based simulation)**
- AI-generated **resolution suggestions**
- **Confidence scoring** mechanism
- Intelligent **Auto Resolve vs Escalate decision**

---

### ⚙️ Automation Engine
- Automatic **incident creation via AI Assistant**
- AI-triggered **auto-resolution**
- Handles **mandatory ServiceNow data policies**
- Business Rule-based **real-time field population**

---

### 💬 AI Assistant (Conversational Simulation)
- Chat-style interaction using UI Action + GlideAjax
- Accepts natural language input  
  *Example: “My internet is slow”*
- Returns:
  - Category
  - Suggested resolution
  - Confidence %
  - Decision

---

### 📝 Now Assist Simulation
- **Generate AI Summary** button
- Populates structured insights into **Work Notes**
- Mimics ServiceNow **Now Assist experience**

---

## 🏗️ Architecture

User Input (UI Action / AI Assistant)
↓
GlideAjax (Client → Server)
↓
AIHelperAjax (Script Include)
↓
AI_SignalProcessor (AI Engine)
↓
Decision + Recommendation
↓
Incident Creation (GlideRecord)
↓
Business Rules Execution
↓
Auto Resolution / Field Population

---

## 🔧 Technologies Used

- ServiceNow Platform
- GlideAjax (Client-Server Communication)
- Script Includes (Server-side logic)
- Business Rules (Automation)
- UI Actions (User Interaction)
- GlideRecord (Database operations)

---

## 🧠 AI Logic Highlights

### 🔍 Category Detection (NLP Simulation)

| Input Keywords | Category |
|--------------|--------|
| internet, wifi, slow | Network |
| app, crash, error | Software |
| others | General |

---

### ⚡ Decision Logic

| Confidence | Action |
|----------|--------|
| > 80% | Auto Resolve |
| ≤ 80% | Escalate |

---

## 🔄 Workflow

1. User clicks **Ask AI Assistant**
2. Enters issue description
3. AI detects category dynamically
4. AI generates resolution & confidence
5. System:
   - Creates Incident
   - Populates AI fields
   - Auto resolves (if applicable)

---

## 🧪 Sample Output

AI Suggestion:
Category: Network
Resolution: Restart router and check network logs
Confidence: 85%
Decision: Auto Resolve

Incident Created: INC0010025

---

## 📊 Business Value

- Reduces **manual incident triage effort**
- Improves **first-time resolution rate**
- Enables **AI-driven IT operations**
- Enhances **user experience through automation**

---

## 🚧 Challenges & Solutions

| Challenge | Solution |
|--------|--------|
| Virtual Agent not available in PDI | Built AI chat simulation using GlideAjax |
| Mandatory resolution fields | Populated via Business Rule |
| Business Rule conflicts | Separated Before & After rules |

---

## 🔮 Future Enhancements

- Integration with **Now Assist / LLM APIs**
- Advanced **NLP using external AI services**
- **AI Insights Dashboard**
- IntegrationHub for **external automation**
- Full **Virtual Agent implementation**

---

## 📁 Project Components

### Script Includes
- `AI_SignalProcessor` → AI engine logic
- `AIHelperAjax` → Client-server interaction

### Business Rules
- AI Execution (Before Insert/Update)
- AI State Handler (After Insert)

### UI Actions
- Ask AI Assistant
- Generate AI Summary

---

## 💼 Resume Highlights

- Built an **AI-powered incident automation system** using ServiceNow
- Implemented **dynamic classification and decision logic**
- Designed **end-to-end workflow using GlideAjax & Business Rules**
- Simulated **Now Assist and Virtual Agent capabilities**

---

## 🔗 Portfolio

👉 https://srikanthmadabhushi.github.io/projects.html

---

## 👤 Author

**Srikanth Madabhushi**  
MS in Artificial Intelligence  
ServiceNow | GenAI | Automation  

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub!
