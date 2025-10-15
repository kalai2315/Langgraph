# LangGraph + Google Gemini AI Workflow

This project demonstrates how to build a simple AI agent system using LangGraph and Google Gemini 2.5 Pro. 
The system can handle conversations, decide when to use external tools, and process the results dynamically.

<img width="256" height="288" alt="image" src="https://github.com/user-attachments/assets/54a4bc37-6d1c-4921-864c-f2c37def8220" />

## Overview

The AI agent interacts with users and generates responses using the Google Gemini model.

When the model identifies a need for additional information, it calls external tools like Tavily Search.

The system uses a structured workflow where the conversation can move between the AI agent and tools, based on conditions.

All conversation history is tracked to maintain context and improve the quality of responses.

Results can be displayed neatly in a Jupyter Notebook for easy viewing.

## Key Components

AI Model: Uses Google Gemini 2.5 Pro for generating conversational responses.

Tool Integration: Supports external tools such as Tavily Search for fetching web-based information.

State Graph: Manages conversation flow using states, conditional edges, and transitions.

Conversation State: Keeps a history of messages, tool calls, and responses.

Dynamic Flow: The system automatically decides when to invoke a tool and then continues the conversation after receiving the tool’s output.

<img width="664" height="528" alt="image" src="https://github.com/user-attachments/assets/4a63d00a-018b-4bcc-ba56-54d81736861d" />

## Setup Requirements

API keys for Google Gemini and Tavily Search.

Environment variables to securely store API keys.

Jupyter Notebook for visualizing responses.

## How It Works

The conversation begins with the AI agent.

The AI evaluates whether it needs additional information from a tool.

If required, it calls the appropriate tool (e.g., web search) and retrieves the results.

The AI resumes the conversation using the tool output.

This cycle continues until the conversation reaches an endpoint.

## Benefits

Enables dynamic and context-aware conversations.

Integrates AI and external tools seamlessly.

Provides a visual and interactive experience in notebooks.

Can be extended to include multiple tools or different AI models.
