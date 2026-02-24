# 🚀 Quick Start

Welcome to Xenovia. Follow these steps to get your assistant up and running.

## Prerequisites
- **Python 3.10+**
- **Docker** (Crucial for code execution)
- **Google Gemini API Key** (Primary engine)
- **(Optional) Anthropic API Key** (For Claude models)

## Installation

1. **Clone & Install**:
   ```bash
   git clone https://github.com/doctorbetaq/xenovia_agent.git
   cd xenovia
   pip install -r requirements.txt
   ```

2. **Prepare Sandbox**:
   ```bash
   # Build the foundational Docker image for Shrimp Execution Units
   docker build -t xenovia-shrimp xenovia/skills/shrimp_docker/
   ```

3. **Configure**:
   ```bash
   cp .env.example .env
   # Add your GEMINI_API_KEY, Discord Token, LINE Token, and other credentials
   ```

4. **Launch**:
   ```bash
   # Starts the entire ecosystem: Web UI, Discord Bot, LINE Bot, and API
   ./xenovia.sh serve  
   ```

## Testing Your Installation

We value stability. Run the comprehensive test suite to ensure your environment is correctly configured:

```bash
# Test the Shrimp Manager and Execution Modes
python3 -m pytest tests/test_shrimp_manager.py

# Test core Skill Registration logic
python3 -m pytest tests/test_shrimp_skill.py
```
