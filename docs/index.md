# Xenovia 2.0 (Anomalocaris Edition) 🚀🦐

[![Xenovia Tests](https://github.com/doctorbetaq/xenovia_agent/actions/workflows/test.yml/badge.svg)](https://github.com/doctorbetaq/xenovia_agent/actions/workflows/test.yml)

> An Advanced Agentic AI Assistant with Managed Autonomous Code Execution, Proactive Notifications, and Self-Learning Capabilities

<img src="https://github.com/doctorbetaq/xenovia/blob/main/xenovia_logo_hires%202.jpeg?raw=true" alt="Xenovia Logo" width="600" />

Xenovia is a cutting-edge AI assistant designed for complex reasoning and execution. It features the **Anomalocaris** managed code execution system, which enables autonomous Python execution in sandboxed environments with persistent monitoring and proactive reporting.

## 🌟 What's New in 2.0

### 🦐 Anomalocaris - Managed Execution Ecosystem
<img src="https://raw.githubusercontent.com/doctorbetaq/xenovia/main/aloma.png" alt="Anomalocaris" width="300" />

- **Managed Lifecycle**: Centralized control of all Shrimp instances via `ShrimpManager`.
- **Temp Mode (`TEMP_MODE`)**: Execute one-off code tasks that automatically report results and files before entering a memory-saving stopped state.
- **Anomalocaris Mode**: Persistent background workers that run periodic scripts (e.g., monitoring, scraping) with real-time log polling.
- **Proactive Notifications**: Xenovia now proactively sends **Discord Direct Messages** when your background tasks complete or produce results.
- **Frozen Legacy Core**: Simplified architecture where all execution is managed, ensuring stability and resource control.

### 🎓 Autonomous Skill Learning
- **Zero-Touch Registration**: Successful executions are automatically analyzed and converted into reusable MCP tools.
- **Context-Aware Learning**: Captures not just code, but requirements, descriptions, and file dependencies.
- **Registry UI**: Manage your agent's expanding capabilities through the web-based Registry.

### 🌐 Native Web Capabilities & Bilingual UI
- **Bilingual Web Interface**: Full dynamic switching between English and Traditional Chinese across all hubs and modals.
- **Native Playwright Browsing**: Deep integration with containerized Playwright for complex JavaScript-rendered website scraping and interaction (with domain whitelisting).
- **Dedicated Agent Identity**: Xenovia can now wield its own Google Account, falling back to the user's account only via explicit natural language requests (e.g., "send an email for me").

### 🛡️ Safety & Reliability
- **Centralized Prompts**: All LLM directives and reasoning rules are unified in a central registry (`prompts.py`).
- **Docker-Locked Sandbox**: 100% isolated environments with resource constraints and explicit DNS configurations for safe network access.
- **Human-in-the-Loop**: Mandatory confirmation for sensitive system operations outside the sandbox.
