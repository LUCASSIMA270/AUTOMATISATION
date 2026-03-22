# AUTOMATISATION

N8N Automations Collection

This repository contains a set of advanced n8n workflows designed for automated strategic intelligence, economic monitoring, and daily knowledge sharing. These workflows leverage multiple APIs (Mistral AI, Groq, Pexels, Google News RSS, Yahoo Finance) to collect, analyze, and distribute high-value content via email.
🚀 Workflows Overview
1. 🏛️ Culture G (Daily Historical Anecdote)

An immersive daily "MEMO" application that sends a unique historical anecdote every morning.

    Mechanism: Triggered daily at 10:00 AM.

    Intelligence: Uses Mistral AI (mistral-small-latest) to generate a journalistic and immersive historical story in JSON format.

    Visuals: Automatically fetches three relevant images from the Pexels API based on keywords extracted from the story.

    Delivery: Sends a beautifully formatted HTML email (using Georgia serif font for a "paper" feel) to multiple recipients via Gmail.

2. 🛢️ IRAN WAR (Global Macro Research)

A high-level strategic newsletter focused on the Iranian conflict and its global economic repercussions, designed with a "Goldman Sachs Analyst" persona.

    Mechanism: Triggered every weekday at 6:00 AM.

    Data Sourcing: Aggregates RSS feeds from Reuters, BBC, Al Jazeera, OilPrice.com, Defense News, and Middle East Eye.

    Financial Integration: Fetches real-time market data for WTI Crude and Brent Crude via Yahoo Finance.

    Analysis: Uses Mistral Large to generate an 8-section strategic report, including executive synthesis, operational situation, energy market analysis (Strait of Hormuz risks), and prospective 30-60-90 day scenarios.

    Output: A professional institutional-grade HTML email with dynamic market tiles and risk alerts.

3. 📈 ACTUALITES (Multipolar Economic Intelligence)

A deep-dive monitoring tool tracking the "Global Chessboard" across three main blocks: France, USA, and Asia.

    Mechanism: Scheduled daily at 10:00 AM.

    Coverage: * Asia: Economy, innovation, and semiconductors.

        USA: Macro-finance (Fed, Wall Street) and AI (Nvidia, OpenAI).

        France: Industrial reindustrialization and French Tech.

    Intelligence: Uses Llama 3.3 70B (via Groq) with a "Sovereign Consultant" persona to detect "weak signals".

    Prospective Analysis: Instead of simple summaries, it produces critical analysis on strategic dependencies and power struggles.

    Delivery: Sends a structured HTML report with specific color coding (#1a237e for titles) and professional formatting.

🛠️ Setup & Requirements
Prerequisites

    An active n8n instance.

    API Keys for the following services:

        Mistral AI (for Culture G and Iran War).

        Groq (for Economic News).

        Pexels (for image sourcing).

        Google/Gmail OAuth2 (for email distribution).

Installation

    Download the JSON files from this repository.

    In n8n, click on Import from File for each workflow.

    Configure the Credentials for each node (Gmail, HTTP Header Auth for Mistral/Groq/Pexels).

    Activate the workflows.

📝 Author

Workflows developed by Lucas Simatovic (Master 2 Economic & Strategic Intelligence).