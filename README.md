# GramaGyan — Multilingual AI-Powered Government Services Assistant

## Overview

GramaGyan is a full-stack conversational assistant I developed to help people find information about Indian government schemes, welfare programs, eligibility criteria, application procedures, and public services.

It retrieves relevant information from configured government portals and web results, then uses GPT-4o-mini to generate context-grounded responses with source references.

## Features

- Supports English, Hindi, Telugu, and Roman Hindi.
- Handles mixed-language and transliterated queries.
- Prioritizes government websites and extracts relevant page content.
- Provides answers with source references.
- Supports browser-based speech input and spoken responses.
- Uses in-memory caching, source prioritization, and configurable timeouts.

## How it works

1. Users submit a typed or spoken question through the React interface.
2. The FastAPI backend identifies language and mixed-language patterns.
3. It retrieves relevant content from configured government sources and web results.
4. GPT-4o-mini generates an answer using the retrieved context.
5. The interface displays the response and available sources; users can listen to the answer.

## Technology

- **Frontend:** React.js, JavaScript, HTML, CSS
- **Backend:** Python, FastAPI, REST APIs
- **LLM:** OpenAI API, GPT-4o-mini
- **Retrieval:** Web search, Requests, BeautifulSoup
- **Speech:** Browser speech recognition and text-to-speech

## Answer quality

Responses are generated from retrieved webpage content and include source references where available. Check the linked source pages for authoritative information. No formal accuracy or performance benchmark results are reported here.

## Security

Keep API keys and other credentials out of the repository. Use environment variables for local configuration.
