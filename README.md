# AI Agent Assignment

This repository contains the workflow schema and execution proof for my Agentic AI assignment built using n8n and Google Gemini.

## Project Description
I built an agentic workflow in n8n that acts as an autonomous assistant. Instead of just answering questions statically, it uses a ReAct decision loop to choose and trigger external tools based on what the user asks.

Key parts used:
- User Input: Chat trigger interface
- Model: Google Gemini (Gemini 2.5 Flash)
- Memory: Window buffer memory to track conversation context
- Tools:
  - Get Weather (fetches live weather data)
  - Get News (retrieves real-time headlines)

## Workflow Architecture (Schema)
The complete node connections and workflow layout are shown below:

![Architecture Schema](architecture.jfif)

## Execution Proof (Outputs)
Here are the test runs showing the agent calling the tools and returning live answers:

![Output 1](Output%201.jpeg)

![Output 2](Output%202.jpeg)

## Code / Schema File
The entire pipeline configuration is exported and stored in the file:
AI agent.json

To test or inspect it:
1. Open n8n.
2. Select Import from File and pick AI agent.json.
3. Connect your Gemini API key to the model node and run the chat trigger.
