# Personal AI Assistant

## Summary

This project is a personal AI assistant chatbot built using LangGraph for the underlying logic and Gradio for the user interface. It provides an interactive chat experience where users can input requests and success criteria, allowing the assistant to process and respond accordingly. The assistant leverages a graph-based workflow with evaluation loops to ensure responses meet user-defined success criteria.

## Features

- Interactive chatbot interface with message history.
- Ability to specify success criteria for each interaction.
- Reset functionality to start a new session.
- Asynchronous processing for efficient handling of requests.
- Resource cleanup on session reset.
- Graph-based workflow with LangGraph for state management.
- Evaluation mechanism to assess response quality against success criteria.
- Memory checkpointing for conversation persistence.

## Capabilities

The assistant is equipped with a range of tools and capabilities to handle diverse tasks:

- **Web Browsing and Navigation**: Uses Playwright to browse the internet, navigate web pages, and retrieve content.
- **File Management**: Can read, write, and manage files within the sandbox directory.
- **Online Search**: Performs web searches using Google Serper API.
- **Wikipedia Queries**: Accesses and queries information from Wikipedia.
- **Python Code Execution**: Runs Python code snippets via a REPL tool for dynamic computations.
- **Push Notifications**: Sends notifications to the user via Discord webhook.
- **Currency Handling**: Ensures all currency responses are in Philippine Peso (PHP).
- **Date and Time Awareness**: Incorporates current date and time in responses.

The assistant operates in a loop, using tools as needed, and evaluates its own responses to determine if success criteria are met or if further user input is required.

## Project Structure

```
AI-assistant-LG/
├── app.py                 # Main application file with Gradio UI
├── assistant.py           # Core assistant logic using LangGraph
├── assistant_tools.py     # Utility tools for the assistant
├── __pycache__/           # Compiled Python files
│   ├── assistant_tools.cpython-312.pyc
│   ├── assistant.cpython-312.pyc
│   ├── sidekick_tools.cpython-312.pyc
│   └── sidekick.cpython-312.pyc
├── sandbox/
│   ├── cebpac.md          # Documentation or notes
│   └── PAL.md             # Documentation or notes
└── README.md              # This file
```

## Getting Started

To run the application, ensure you have the required dependencies installed (e.g., via pip for Python packages). Then, execute the following command:

```bash
python app.py
```

The application will launch in your default web browser.
