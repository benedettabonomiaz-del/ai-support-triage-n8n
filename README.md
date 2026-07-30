# AI-Powered Support Ticket Triage Automation

An automated customer support triage pipeline built with **n8n** and powered by **Llama 3.3**. 

Instead of treating all incoming contact forms equally, this workflow performs real-time sentiment/urgency classification to ensure critical customer issues get escalated instantly.

## Key Features
* **Automated Data Capture:** Listens for incoming contact form submissions in real-time.
* **LLM Intent Analysis:** Uses **Llama-3.3-70b** (via Groq API) to evaluate message context and categorize urgency (`URGENT` vs `NORMAL`).
* **Conditional Routing:** Utilizes n8n logic nodes to split processing paths based on AI classification.
* **Instant Escalation:** Automatically sends enriched email alerts for high-priority cases.

## Tech Stack
* **Automation Engine:** [n8n](https://n8n.io/)
* **AI Model:** Llama 3.3 70B Versatile (Groq Cloud API)
* **Integrations:** Gmail API

## How to Use
1. Clone or import the `workflow.json` into your self-hosted or cloud n8n instance.
2. Add your **Groq API Key** in the HTTP Request node header.
3. Authenticate your **Gmail** account node.
4. Activate the workflow and link your form submission trigger!
