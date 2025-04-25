# Agent Tala - Gold Market Analysis Agent

## Overview

Agent Tala is an AI-powered agent designed to provide expert analysis of the gold market. It leverages historical price data, macroeconomic news, geopolitical events, and supply/demand factors to offer comprehensive insights and investment recommendations (Buy, Hold/Monitor, Maintain).

The agent is built using Google's Agent Development Kit (ADK) and utilizes Google's Gemini models for its analytical capabilities.

## Features

*   **Historical Trend Analysis:** Identifies patterns, support/resistance levels, and trends from past price data.
*   **Fundamental Analysis:** Evaluates the impact of economic indicators (interest rates, inflation, GDP), geopolitical events, and central bank policies on gold prices.
*   **Integrated Analysis:** Combines historical and fundamental analysis for a holistic market view.
*   **Risk/Opportunity Assessment:** Highlights potential risks and investment opportunities.
*   **Clear Recommendations:** Provides explicit suggestions: `Buy`, `Do Not Buy / Monitor Closely`, or `Maintain`.
*   **Data-Driven Reasoning:** Justifies recommendations by referencing input data and news.
*   **Web Search Integration:** Uses Google Search (via `google_search` tool) to potentially gather up-to-date information if needed during analysis (though the primary analysis relies on provided input data).

## Setup

1.  **Environment Variables:** Configure the necessary environment variables in the [`agent_tala/.env`](agent_tala/.env) file. Key variables include:
    *   `GOOGLE_API_KEY`: Your Google API key for accessing Gemini models.

2.  **Dependencies:** Ensure you have the required Python libraries installed, including `google-adk`, `google-generativeai`, etc. (A `requirements.txt` file would typically list these).

## How to Run

You can run the agent using the ADK CLI. Based on the comments in [`agent_tala/agent.py`](agent_tala/agent.py), the command might be similar to:

```sh
adk web --port xxx
```