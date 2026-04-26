# n8n-chat-agent-groq-serpapi
#  n8n AI Agent with Memory & Web Search

An intelligent conversational AI agent built using **n8n**, powered by a Groq chat model and enhanced with memory and real-time web search via SerpAPI.

---

##  Features

*  Chat-based trigger (real-time interaction)
*  AI Agent using Groq (LLaMA model)
*  Conversation memory (buffer window)
*  Web search integration (SerpAPI)
*  Modular workflow design using n8n

---

##  Workflow Architecture

```
Chat Trigger → AI Agent
                  ↑
      ┌───────────┼───────────┐
      │           │           │
  Groq Model   Memory     SerpAPI
```

---

## ⚙️ Technologies Used

* n8n (workflow automation)
* Groq API (LLM - llama-3.3-70b-versatile)
* SerpAPI (web search)
* LangChain nodes (agent, memory, tools)

---

##  Workflow Overview

### 1. Chat Trigger

* Entry point for user messages
* Initiates the workflow

### 2. AI Agent

* Central decision-making unit
* Processes input using connected tools and memory

### 3. Groq Chat Model

* Model: `llama-3.3-70b-versatile`
* Handles natural language understanding and responses

### 4. Simple Memory

* Buffer window memory
* Maintains conversation context

### 5. SerpAPI Tool

* Enables real-time web search
* Enhances responses with external data

---

## 🔧 Setup Instructions

### 1. Import Workflow

* Open n8n
* Import the provided JSON file

---

### 2. Configure Credentials

You must add your own API keys:

#### Groq API

* Create API key from Groq Console
* Add credential in n8n

#### SerpAPI

* Create account at SerpAPI
* Add API key in n8n

---

### 3. Connect Credentials

* Open each node:

  * Groq Chat Model
  * SerpAPI
* Select your configured credentials

---

### 4. Run Workflow

* Activate workflow
* Send a chat message to trigger

---

## Security Note

* API keys are NOT included in this repository
* Credentials must be configured locally in n8n
* Never expose API keys publicly

---

##  Example Use Cases

* Ask general knowledge questions
* Perform real-time web searches
* Maintain conversational context
* Build your own “Jarvis”-style assistant

---

##  Notes

* This workflow uses n8n LangChain nodes
* Requires active internet connection
* Performance depends on API limits (Groq, SerpAPI)

---

## Future Improvements

* Add email automation
* Integrate voice input/output
* Add database memory (long-term)
* Deploy on cloud for 24/7 access

---

##  Author

Built as part of learning backend + AI automation using n8n.

---

## ⭐ Support

If you found this useful:

* Star the repo
* Fork and improve
* Share with others
