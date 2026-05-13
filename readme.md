<div align="center">

<!-- title -->

<!--lint ignore no-dead-urls-->

# Awesome Elixir LLM/GenAI  [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![lint](https://github.com/druyang/awesome-elixir-llm-ai/actions/workflows/lint.yaml/badge.svg)](https://github.com/druyang/awesome-elixir-llm-ai/actions/workflows/lint.yaml)

<!-- subtitle -->

A (awesome) list of resources for building LLM/GenAI applications in Elixir. This list is focused on large language models (LLMs) and deep learning AI applications.

<!-- image -->

<a href="" target="_blank" rel="noopener noreferrer">
  <img src="" />
</a>

<!-- description -->

[Elixir](https://elixir-lang.org/) is a functional, concurrent, general-purpose programming language that runs on BEAM, the Erlang virtual machine. 
With scalability and (near) realtime capabilities, Elixir has the potential to be useful for building LLM/AI applications. Many of these tool and resources are experimental and under active development.

I'm a big fan of Elixir (as a MLE/Data Scientist). This is a list of resources that I've found useful as I combine my learning of Elixir and my LLM/AI background.

</div>

<!-- TOC -->

## Contents

- [LLM Clients and APIs](#llm-clients-and-apis)
- [Agent Frameworks](#agent-frameworks)
- [Model Serving and Inference](#model-serving-and-inference)
- [Vector Databases and RAG](#vector-databases-and-rag)
- [MCP and Integrations](#mcp-and-integrations)
- [AI Coding Assistants and Skills](#ai-coding-assistants-and-skills)
- [Evaluation and Utilities](#evaluation-and-utilities)
- [Audio and Speech](#audio-and-speech)
- [Resources](#resources)
  - [Notebooks](#notebooks)
  - [Videos](#videos)
  - [Example Applications](#example-applications)

## LLM Clients and APIs

Libraries for calling LLM provider APIs and generating structured outputs.

- [Anthropix](https://github.com/lebrunel/anthropix) - Unofficial Anthropic Claude API client with tool use, prompt caching, message batching, and streaming.
- [ExLLM](https://github.com/azmaveth/ex_llm) - All-in-one LLM library for Elixir with unified provider interface and structured outputs (14 providers with access to 300+ models).
- [Gemini_ex](https://github.com/nshkrdotcom/gemini_ex) - A Gemini and VertexAI Elixir client.
- [InstructorLite](https://github.com/martosaur/instructor_lite) - Structured outputs for LLMs in Elixir.
- [instructor_ex](https://github.com/thmsmlr/instructor_ex) - Structured, Ecto outputs with OpenAI (and OSS LLMs).
- [LLMComposer](https://github.com/doofinder/llm_composer) - A streamlined way to build OpenAI and Ollama applications with auto-execution of functions.
- [Ollama](https://github.com/lebrunel/ollama-ex) - A nifty little library for working with Ollama in Elixir.
- [Omni](https://github.com/aaronrussell/omni) - Universal Elixir client for LLM APIs with streaming text generation, tool use, and structured output across providers.
- [OpenaiEx](https://github.com/cyberchitta/openai_ex) - A community-maintained OpenAI API client.
- [ReqLLM](https://github.com/agentjido/req_llm) - A Req plugin for calling 18+ LLM providers with a unified streaming and non-streaming interface, inspired by Vercel's AI SDK.

## Agent Frameworks

Libraries for building LLM agents, chains, and multi-agent systems.

- [Alloy](https://github.com/alloy-ex/alloy) - Minimal, OTP-native agent harness focused on the completion-tool-call loop, with multi-provider support and supervised GenServer agents.
- [AshAi](https://github.com/ash-project/ash_ai) - A library for building OpenAI style LLM driven applications with Ash.
- [ClaudeCode SDK](https://github.com/guess/claude_code) - The idiomatic Elixir SDK for building AI agents on top of the Claude Code CLI, with OTP sessions, streaming, and in-process tools.
- [Elixir Langchain](https://github.com/brainlid/langchain) - Integrate AI services and self-hosted models into an Elixir application, a port of the popular Langchain Python library.
- [Jido](https://github.com/agentjido/jido) - A framework for building distributed agent systems in Elixir.
- [Legion](https://github.com/dimamik/legion) - Elixir framework for building AI agents that write and execute sandboxed Elixir code instead of making function calls.
- [OpenAI Agents Elixir](https://github.com/rwdaigle/openai-agents-elixir) - Idiomatic Elixir framework for building agentic workflows on OpenAI's Responses API, modeled after OpenAI's Python Agents library.
- [Sagents](https://github.com/sagents-ai/sagents) - Build interactive AI agents with OTP supervision, middleware, human-in-the-loop approvals, sub-agent delegation, and a LiveView debugger (built on Elixir LangChain).
- [Whisperer](https://github.com/Monitor-Lizzard/whisperer) - Unopinionated, OTP-based framework for sequencing and orchestrating multi-agent AI workflows in Elixir.

## Model Serving and Inference

Tools for running and hosting AI models locally or on cloud infrastructure.

- [Bumblebee](https://github.com/elixir-nx/bumblebee) - A library for serving and distributing models in Elixir, a counterpart to Hugging Face's Transformers.
- [Bumblebee Model Harness](https://github.com/fly-apps/bumblebee-model-harness) - Host AI models on (fly.io) GPUs.
- [ortex](https://github.com/elixir-nx/ortex) - A wrapper around the ONNX Runtime.

## Vector Databases and RAG

Vector stores, retrieval, and Retrieval Augmented Generation utilities.

- [pgvector-elixir](https://github.com/pgvector/pgvector-elixir) - Add vector embeddings to postgres via Ecto.
- [Qdrant](https://github.com/marinac-dev/qdrant) - An Elixir client for the Qdrant vector similarity search engine.
- [rag](https://github.com/bitcrowd/rag) - Retrieval Augmented Generation in Elixir.
- [sqlite_vec](https://github.com/joelpaulkoch/sqlite_vec) - Add vector embeddings to sqlite via Ecto.
- [TextChunker](https://github.com/revelrylabs/text_chunker_ex) - A semantic text chunker with langchain-style chunking.
- [Vettore](https://github.com/elchemista/vettore) - High-performance in-memory vector database built with Rustler, supporting cosine, euclidean, dot product, and HNSW similarity search with MMR reranking.

## MCP and Integrations

Model Context Protocol servers and IDE/tool integrations.

- [Anubis MCP](https://github.com/zoedsoupe/anubis-mcp) - Actively maintained Elixir MCP SDK (continuation of hermes-mcp) for building MCP clients and servers with HTTP and SSE transports.
- [Hermes MCP](https://github.com/cloudwalk/hermes-mcp) - High-performance Elixir SDK for the Model Context Protocol, with full client and server implementations.
- [MCP Hex Server](https://hex-mcp.9elements.com/) - A MCP server for Elixir Hex packages.
- [Phantom MCP](https://github.com/dbernheisel/phantom_mcp) - An MCP server framework for Elixir Plug with Phoenix integration and stdio support for clients like Claude Desktop.
- [Tidewave Phoenix](https://github.com/tidewave-ai/tidewave_phoenix) - Tidewave for Phoenix, introspection/integration of a phoenix web app for AI coding tools over MCP.

## AI Coding Assistants and Skills

Plugins, skills, and agent configurations for AI coding tools targeting Elixir/Phoenix development.

- [claude-elixir-phoenix](https://github.com/oliver-kriska/claude-elixir-phoenix) - Claude Code plugin for Elixir/Phoenix that orchestrates specialist agents for planning, implementation, and review, with auto-loading skills for LiveView, Ecto, OTP, and Tidewave MCP integration.

## Evaluation and Utilities

Development tools, LLM evaluation, and other utilities.

- [Livebook](https://github.com/livebook-dev/livebook) - A web application for writing interactive and collaborative code notebooks, an Elixir alternative to Jupyter Notebook.
- [PythonX](https://github.com/cocoa-xu/pythonx) - Run Python code from Elixir. Possible to run Hugging Face models ([example](https://samrat.me/running-ml-models-in-elixir-using-pythonx/)).
- [Tribunal](https://github.com/georgeguimaraes/tribunal) - LLM evaluation and testing framework with deterministic and LLM-as-judge assertions for hallucinations, toxicity, and PII.

## Audio and Speech

- [Cool Whisper Server](https://github.com/dailydaniel/cool-whisper-server) - OpenAI compatible Elixir-based HTTP server for running inference on audio files.

## Resources

### Notebooks

- [Talking to OpenAI real-time with boombox](https://github.com/membraneframework/boombox/blob/master/examples/data/talk_to_llm.html)

### Videos

- (Feb 2024) - [Smarter Apps with Ash and GenAI](https://www.youtube.com/watch?v=10VBTcN8gAo)
- (2025) - [Whisperer: An Elixir-Based Multi-Agent Workflow Framework](https://www.elixirconf.eu/talks/whisperer-an-elixir-based-multi-agent-workflow-framework/) - ElixirConf EU 2025 talk on building OTP-native multi-agent workflows.
- (2025) - [Full-Stack AI with Elixir: Simplicity and Scale to Millions of Customers](https://elixirconf.com/talks/full-stack-ai-with-elixir-simplicity-and-scale-to-millions-of-customers/) - ElixirConf US 2025 talk from CloudWalk on running multi-agent LLM chat and GPU image moderation in production.

### Example Applications

- [Gettext LLM](https://github.com/paulsabou/gettext_llm) - Translate all Gettext PO folders/files in your project using any LLM endpoint supported by langchain.
- [Why Elixir/OTP doesn't need an Agent framework (InstructorLite Example)](https://goto-code.com/blog/elixir-otp-for-llms/) - Uses InstructorLite to show why Elixir does not need a wrapping agent framework (opinion).

## Contributing

[Contributions of any kind welcome](contributing.md)! As tools for Elixir develop, I'll be updating this list and welcome any contributions.

[Thanks goes to these contributors](https://github.com/druyang/awesome-elixir-llm-ai/graphs/contributors)!
