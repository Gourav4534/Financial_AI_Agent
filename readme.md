# Multi-Agent AI Playground

This repository contains a Python project that demonstrates the creation and use of multiple AI agents, designed for web search and financial analysis. These agents leverage advanced language models and tools to provide insightful and organized outputs, such as web search results and financial data summaries.

---

## Features

- **Web Search Agent**: Retrieves and summarizes web information using DuckDuckGo, ensuring sources are always included.
- **Finance AI Agent**: Provides financial insights, including stock prices, analyst recommendations, fundamentals, and company news, using YFinance.
- **Multi-Agent Team**: Combines both agents to work collaboratively, delivering enhanced outputs for complex queries.
- **Interactive Playground**: Features a user-friendly FastAPI-based playground for testing and interacting with agents in real-time.

---

## Setup

### Prerequisites

Ensure you have the following installed:
- Python 3.12

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add your `PHI_API_KEY`:
     ```
     PHI_API_KEY=<your-api-key>
     ```

---

## Usage

1. Start the Playground app:
   ```bash
   python Playground.py
   ```

   The app will run locally and reload automatically on code changes.

2. Use the interactive agents:
   - **Web Search Agent**: Searches the web and includes sources in the response.
   - **Finance AI Agent**: Summarizes stock information and news using tables.

3. Run a multi-agent query example:
   ```python
   multi_ai_agent.print_response("Summarize analyst recommendation and share the latest news for NVDA", stream=True)
   ```

---

## Project Structure

- `Playground.py`: Main application script for the interactive playground.
- `financial_agent.py`: Script defining the financial agent's logic.
- `.gitignore`: Specifies files to ignore in version control.
- `requirements.txt`: Lists all Python dependencies.

---

## Requirements

The project requires the following Python libraries:
- `phidata`
- `python-dotenv`
- `yfinance`
- `packaging`
- `duckduckgo-search`
- `fastapi`
- `uvicorn`
- `groq`

---



