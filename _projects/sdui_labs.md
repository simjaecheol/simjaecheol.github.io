---
layout: page
title: SDUI Labs
description: Generative Server-Driven UI (SDUI) Playground for Samsung.com e-commerce scenarios
img: /assets/img/sdui-labs.jpg
importance: 1
category: work
---

**SDUI Labs** is a monorepo laboratory environment for prototyping and validating **LLM-driven dynamic Server-Driven UI (Generative UI)** configurations tailored for Samsung.com e-commerce scenarios.

## Key Features

- **Server-Driven UI Engine:** Renders dynamic layouts from JSON schemas fetched from the backend, eliminating hardcoded client screens
- **Template-based Generative UI:** Combines LLM reasoning with pre-defined templates (Jinja2) to eliminate hallucinations and achieve production-level low latency
- **Conversational AI Mode (Multi-turn):** A full chat interface where users can interact with an AI assistant that provides both text responses and real-time UI updates (SDUI) in a side-by-side experience
- **Context-Aware Scenarios:** Tests specialized intervention scripts such as cart abandonment prevention (smart bundle offers) and natural-language comparative layouts
- **User Profiling & Personalization:** Collects user demographic data and natively injects it into the ADK Session

## Tech Stack

- **Backend:** FastAPI (Python)
- **Frontend:** React + TypeScript + Vite
- **LLM Integration:** OpenAI API with function calling
- **Templating:** Jinja2
- **Containerization:** Docker & Docker Compose

## Architecture Overview

1. **Client Request:** Send shopper's context (cart items, search history, signals) to the backend
2. **LLM Decision:** LLM determines the most suitable layout template using function calling
3. **Template Binding:** Template engine binds variables into structured SDUI JSON schema
4. **Client Render:** React client parses and renders components with real-time updates

## Project Links

- **GitHub Repository:** [simjaecheol/sdui-labs](https://github.com/simjaecheol/sdui-labs)
- **Language:** Python, TypeScript, HTML
