# ⚡ AI Code Auditor — PromptWars Virtual

AI Code Auditor is an intelligent developer assistant engineered to automate code reviews, detect structural bugs, and suggest optimization strategies. Built for the **[Mini Challenge] I am a Prompt Warrior** on Hack2Skill, this tool leverages **Google Antigravity** to act as an automated peer-reviewer for software engineers.

---

## 🚀 Submission Links
- **GitHub Repository:** https://github.com/Prerakgarg2007/ai-code-auditor
- **Live Application Link:** Running Locally

---

## 📌 Problem Statement
Manual code reviews are time-consuming and often miss subtle performance bottlenecks or security vulnerabilities. **AI Code Auditor** solves this by allowing developers to instantly scan their scripts. By using structured AI prompts, it delivers constructive feedback, complexity analysis, and refactored code blocks in seconds.

---

## 🧠 Prompt Engineering Strategy
As a "Prompt Warrior," the focus was on designing strict structural boundaries and system rules to ensure the LLM reviews code objectively without breaking syntax.

### 1. System Prompt Design
To prevent the model from generating conversational fluff, we anchored it with this system instruction:
```text
You are an elite Senior Software Engineer and Security Auditor. 
Analyze the provided code snippet for:
1. Syntax errors or logical bugs.
2. Performance bottlenecks (Time/Space complexity).
3. Security vulnerabilities.

Output your response strictly in the following format:
### 🐞 Bugs Detected
[List bugs or state "None"]
### ⚡ Performance Optimizations
[List improvements]
### 🛠️ Refactored Code
[Provide clean, optimized markdown code block]
