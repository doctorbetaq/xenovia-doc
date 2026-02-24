# 🖥️ Usage Guide

Xenovia can be accessed and controlled through multiple interfaces: the Web Dashboard, Discord, and LINE.

## 🦐 Execution Modes

Xenovia's Anomalocaris code engine operates in one of three modes depending on the task:

| Mode | Behavior | Best For |
| :--- | :--- | :--- |
| `ONCE` | Standard one-off execution. | Simple calculations, file conversions. |
| `TEMP_MODE` | Execute, Report Result + Files, then STOP. | Data analysis, complex research. |
| `ANOMALOCARIS` | Runs a persistent background `periodic_task.py` script. | Monitoring, hourly scraping, auto-tasks. |

*(Note: Mode selection is automated by the reasoning engine, but you can manually spawn Anomalocaris workers via the Web UI Hub.)*

## 🤖 Discord Commands

Control your Managed Shrimp instances directly from Discord:

- `/shrimp list`: List all currently managed execution instances and their operational status.
- `/shrimp start <id>`: Start a stopped instance.
- `/shrimp stop <id>`: Gracefully halt a running instance.
- `/shrimp files <id>`: View the workspace contents of an instance.
- `/shrimp containers`: *(Admin)* See raw Docker container status on the host system.
- `/shrimp prune`: *(Admin)* Safely remove unmanaged "zombie" containers to reclaim system resources.

## 📊 Model Cost & Speed Comparison

You can switch the active reasoning model through the Web UI's Hub settings.

| Model | Provider | Speed | Best For |
| :--- | :--- | :--- | :--- |
| `gemini-2.0-flash-lite` | Google | ⚡⚡⚡ | Fast, cheap background tasks |
| `gemini-2.0-flash` | Google | ⚡⚡ | **Default Choice** - Balanced |
| `claude-3-5-sonnet` | Anthropic | ⚡ | Complex coding & extensive tool use |

## 🌐 Playwright Browsing

When Xenovia needs to interact securely with complex, modern web apps:
- It utilizes a containerized `browserless/chrome` instance.
- Ensure the domain you are trying to automate is registered in the **Domain Whitelist** via the Web UI to prevent accidental or malicious navigation.
