# MCP-Based No-Code AI Automation System

## 📌 Project Overview
This project demonstrates a practical implementation of **Modern Context Protocol (MCP)** to enable
Large Language Models (LLMs) to perform real-world actions without writing any backend code.

Using **Cursor IDE as the MCP Host** and **Composio as the MCP Server**, the system allows AI to
interact with applications like **LinkedIn** and **Gmail** using simple natural language prompts.

---

## 🧠 Problem Statement
Traditional LLM workflows using function calling:
- Require manual function definitions
- Cannot directly execute actions
- Are difficult to scale across multiple services
- Increase maintenance and security risks

This project addresses these limitations using **MCP**.

---

## 💡 Proposed Solution
The solution uses **Modern Context Protocol (MCP)** to expose tools and actions to the LLM in a
standardized way.

### Key Components:
- **MCP Host:** Cursor IDE
- **MCP Server:** Composio
- **Tools Integrated:** Gmail, LinkedIn
- **Execution Style:** No-code, prompt-based actions

---

## 🏗️ MCP Architecture
The MCP architecture consists of:
- MCP Host (Cursor IDE)
- MCP Server (Composio)
- External tools connected via APIs (Gmail, LinkedIn)

The host and server communicate using the MCP protocol, enabling seamless execution of actions.

📁 Architecture diagrams are available in the `architecture/` folder.

---

## 🔄 MCP Communication Workflow
1. User enters a natural language prompt
2. MCP Host requests available tools from MCP Server
3. MCP Server returns tool list
4. LLM selects the appropriate tool
5. MCP Server executes the tool
6. Result is returned and formatted for the user

Detailed workflow diagrams are available in `workflow/`.

---

## 🧪 Implementation Summary
- Connected Gmail and LinkedIn to Composio using OAuth
- Selected required actions in Composio dashboard
- Generated MCP server link
- Connected MCP Server to Cursor IDE
- Verified tool availability inside Cursor
- Executed actions using natural language prompts

No custom code or API logic was written during implementation.

---

## 🧾 Sample Prompt
```text
Create a LinkedIn post with the following text:
"Exploring Modern Context Protocol for no-code AI automation!"

