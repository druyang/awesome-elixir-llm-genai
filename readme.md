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
With scalability and (near) realtime capabilities, Elixir has the potential to be useful for building LLM/AI applications.

I'm a big fan of Elixir (as a MLE/Data Scientist). This is a list of resources that I've found useful as I combine my learning of Elixir and my LLM/AI background.

</div>

<!-- TOC -->

## Contents

- [LLM Clients](#llm-clients)
- [LLMOps MLOps](#llmops-mlops)
- [Tooling](#tooling)
- [Example Applications](#example-applications)
- [Resources](#resources)

## LLM Clients

Libraries for wrapping LLM APIs.

- [Elixir Langchain](https://github.com/brainlid/langchain) - Integrate AI services and self-hosted models into an Elixir application, a port of the popular Langchain Python library.
- [instructor_ex](https://github.com/thmsmlr/instructor_ex) - Structured, Ecto outputs with OpenAI (and OSS LLMs).
- [OpenaiEx](https://github.com/cyberchitta/openai_ex) - A community-maintained OpenAI API client.
- [LLMComposer](https://github.com/doofinder/llm_composer) - A streamlined way to build OpenAI and Ollama applications with auto-execution of functions.

## LLMOps MLOps

- [Bumblebee](https://github.com/elixir-nx/bumblebee) - A library for serving and distributing models in Elixir, a counterpart to Hugging Face's Transformers.
- [Bumblebee Model Harness](https://github.com/fly-apps/bumblebee-model-harness) - Host AI models on (fly.io) GPUs.
- [ortex](https://github.com/elixir-nx/ortex) - A wrapper around the ONNX Runtime.

## Tooling

- [Livebook](https://github.com/livebook-dev/livebook) - A web application for writing interactive and collaborative code notebooks, an Elixir alternative to Jupyter Notebook.
- [pgvector-elixir](https://github.com/pgvector/pgvector-elixir) - Add vector embeddings to postgres via Ecto.
- [Vecto](https://github.com/agoodway/vecto) - Hybrid search with Ecto and pgvector.

## Example Applications
- [Gettext LLM](https://github.com/paulsabou/gettext_llm) - Translate all Gettext PO folders/files in your project using any LLM endpoint supported by langchain.

## Resources

### Notebooks 

- [Talking to OpenAI real-time with boombox](https://github.com/membraneframework/boombox/blob/master/boombox_examples_data/talk_to_llm.html)

## Contributing

[Contributions of any kind welcome](contributing.md)! As tools for Elixir develop, I'll be updating this list and welcome any contributions.

### Contributors

[Thanks goes to these contributors](https://github.com/druyang/awesome-elixir-llm-ai/graphs/contributors)!
