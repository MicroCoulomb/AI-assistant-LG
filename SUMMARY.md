# SUMMARY

## Project Showcase

LangGraph-based personal AI assistant that combines tool-augmented task execution with an evaluator loop, letting users define success criteria and have the system iterate until the response is acceptable or clarification is needed.

- Built as a graph-driven agent workflow with separate worker, tool, and evaluator stages, enabling multi-step reasoning, tool use, and self-correction in a controlled loop.
- Supports practical task execution through browser automation, sandboxed file management, Python REPL execution, web search, and Wikipedia retrieval, making it useful for research, lightweight automation, and assisted problem solving.
- Adds an automated quality check layer by scoring each response against user-provided success criteria, which is a strong pattern for reliable agent behavior and evaluative AI systems.
- Includes conversation persistence and session reset handling with in-memory checkpointing and resource cleanup, keeping the interactive experience stable during repeated use.
- Exposes the system through a simple Gradio chat interface, making the agent workflow accessible as a usable application rather than just a backend prototype.

**Tech Stack**

- LangGraph
- LangChain
- OpenAI GPT-4o-mini
- Gradio
- Playwright
- Python
- Pydantic
- Google Serper API
- Wikipedia API
- dotenv

## Project Card

Tool-augmented LangGraph AI assistant with evaluator-based response checking against user-defined success criteria.

- Uses a multi-node agent workflow for tool calling and iterative answer refinement.
- Handles browser automation, file operations, search, and Python execution in one assistant loop.
- Wraps the backend in a lightweight Gradio interface for interactive use.

**Main Tech Stack**

- LangGraph
- LangChain
- OpenAI GPT-4o-mini
- Gradio
- Playwright
