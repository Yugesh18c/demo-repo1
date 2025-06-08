# Company News Sentiment Pipeline (LangChain + Langfuse + Azure GPT-4o)

This project builds an LLM-powered data pipeline using LangChain, Azure OpenAI, and Langfuse to analyze financial news sentiment for a given company.

---

## Features

- Input: Any company name (e.g., `"Apple Inc"`)
- Step 1: Extract its stock ticker (e.g., `"AAPL"`)
- Step 2: Fetch real-time news using Yahoo Finance
- Step 3: Analyze the sentiment using GPT-4o / GPT-4o-mini (Azure OpenAI)
- Step 4: Output a structured JSON with:
  - Sentiment (Positive/Negative/Neutral)
  - Entities: People, Places, Companies
  - Industry & Market Implications
- Step 5: Langfuse integration for full tracing, debugging, and monitoring

---

## Package Dependencies

Install the required libraries:

```bash
pip install langchain langfuse yfinance openai langchain-community YahooFinanceNewsTool
