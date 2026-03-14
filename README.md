🤖 Cloud-Native AI Automation Engine (n8n)

This repository contains the architecture and logic for a self-hosted, enterprise-grade automation system. The project demonstrates the full data lifecycle: from ingestion and infrastructure management to AI-driven analysis.

🏗️ Architecture & InfrastructureEnvironment:

Self-hosted on a Linux-based Virtual Private Server (VPS) via DigitalOcean.Containerization: Fully containerized using Docker for scalable deployment and environment isolation.Security: Managed via SSL/TLS encryption, environment variables, and encrypted credential storage.Core Stack: n8n, JavaScript, Google Gemini Pro API, Telegram Bot API, YouTube Data API.

🚀 Key Workflows

AI Recruitment Agent (Job Search & LLM Analysis)Ingestion: Fetches real-time data from Job Search REST APIs.Logic: Filters listings based on specific keywords and data normalization via custom JavaScript nodes.AI Orchestration: Passes job descriptions and my resume through Google Gemini Pro to analyze compatibility.Output: Automatically generates tailored motivation letters based on the prompt-engineered analysis.
YouTube Content PipelineAutomation: Full-lifecycle management of video uploads via the YouTube Data API.Trigger: Event-driven execution initiated through a Telegram Bot interface.Status Tracking: Real-time monitoring of subscriber counts and video metrics.
Data Transformation & MaintenanceJSON Parsing: Utilizes complex JavaScript logic to handle heterogeneous data sources.Asynchronous Handling: Implemented Wait and Conditional (If) nodes to manage LLM latency and ensure data quality.
🛠️ How to Use

Install n8n (ideally via Docker).Import the My_workflow.json file.Configure your environment variables for GEMINI_API_KEY, TELEGRAM_BOT_TOKEN, and YOUTUBE_OAUTH.
