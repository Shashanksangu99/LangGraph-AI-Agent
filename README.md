# Stateful Multi-Agent System with LangGraph and Groq's Gemma-7B-IT
## Project Overview
This project demonstrates a multi-agent system built using LangGraph, an extension of LangChain that enables structured, graph-based coordination between multiple AI agents. The system is powered by the Gemma-7B-IT model from Groq, known for its high-speed and low-latency inference.

The agents are designed to collaboratively solve complex tasks by passing messages and building memory over multiple interactions, mimicking human-like problem-solving workflows.

## Motivation
In traditional AI workflows, a single monolithic agent attempts to handle all tasks, often leading to inefficiencies and limitations. By designing specialized agents that focus on specific subtasks and communicate with each other, the system becomes more scalable, modular, and intelligent.

This project was built to explore:

- How multiple lightweight agents can work together in a graph-based environment.

- How using faster models like Groq’s Gemma-7B-IT can dramatically reduce inference time while maintaining quality.

- How agent memory and interaction history can improve contextual understanding over time.

## Agents Designed
Question Rewriter Agent

- Reformulates or clarifies incoming user questions to make them more precise and complete.

- Helps ensure downstream agents receive high-quality, unambiguous input.

Answer Generator Agent

- Takes the refined questions and generates detailed, accurate answers.

- Leverages the optimized performance of Gemma-7B-IT for fast responses.

Final Answer Combiner

- Optionally merges outputs from different agents to produce a cohesive final response.

- Each agent has a specific, narrow role, making the system easier to debug, extend, and improve over time.

## Value Proposition
- Speed and Efficiency: Using Groq’s Gemma-7B-IT allows the system to respond faster than traditional large language models hosted elsewhere.

- Modularity: The agent architecture is modular, meaning new specialized agents can easily be added to the workflow.

- Scalability: Graph-based structures allow for complex workflows that go beyond simple chains, enabling parallel reasoning paths.

- Real-world Applications: Such multi-agent systems can be adapted for customer support, research assistants, automated QA systems, educational tutors, and more.

## Technologies Used
- LangGraph (multi-agent graph framework)

- LangChain (core agent and LLM orchestration)

- Groq API (access to the Gemma-7B-IT model)

- Python (for coding the logic and workflows)

## Future Work
- Adding tool-augmented agents (e.g., web search, calculators)

- Introducing dynamic agent spawning based on task complexity

- Evaluating performance across different LLMs and providers

- Building a front-end interface for real-time interaction
