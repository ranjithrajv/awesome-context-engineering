# Awesome Context Engineering [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome resources, tools, and papers for **Context Engineering**. Your one-stop shop for mastering the art and science of crafting the perfect context for Large Language Models (LLMs).

> **Context Engineering** is the system-level discipline of designing, building, and optimizing the dynamic information ecosystem provided to an AI model to perform a task. It's the architecture of the information an AI reasons with, moving beyond single prompts to create robust, state-aware, and reliable AI systems.

Contributions are welcome\! Please open a pull request to add more resources.

## Why Context Engineering is a Keystone of Modern AI

In a rapidly evolving AI landscape with new models and concepts emerging daily, it's easy to get lost in the hype. Context Engineering provides a durable and fundamental framework for value creation. Here’s why it has such a significant and lasting impact:

  * **It Addresses the Core Limitation of LLMs:** Even the most powerful models are fundamentally stateless and only "know" what is in their context window. Their performance is not a function of their raw intelligence alone, but of the quality of the information they are given. Context Engineering is the discipline of managing this core constraint.
  * **It’s the Difference Between a Demo and a Product:** A clever prompt (`Prompt Engineering`) can create a flashy demo. A robust context architecture (`Context Engineering`) creates a reliable, scalable, and "magical" product that can handle real-world complexity. Most agent failures today are not model failures; they are context failures.
  * **It Future-Proofs AI Development:** As LLMs become more powerful and commoditized, the key differentiator will not be the model itself, but the proprietary and effective context you can provide it. This is where sustainable competitive advantage is built.
  * **It Elevates the Focus from Instructions to Systems:** Context Engineering shifts the focus from simply "talking to the AI" to designing the entire system that feeds the AI. This involves data retrieval, memory management, tool integration, and user-state awareness—the true building blocks of sophisticated applications.

-----

## Contents

  - [Core Concepts & Overviews](https://www.google.com/search?q=%23core-concepts--overviews)
  - [Key Techniques & Strategies](https://www.google.com/search?q=%23key-techniques--strategies)
  - [Emerging Trends & The Future](https://www.google.com/search?q=%23emerging-trends--the-future)
  - [Frameworks & Libraries](https://www.google.com/search?q=%23frameworks--libraries)
  - [Tools & Platforms](https://www.google.com/search?q=%23tools--platforms)
  - [Seminal Research & Papers](https://www.google.com/search?q=%23seminal-research--papers)
  - [Guides & Tutorials](https://www.google.com/search?q=%23guides--tutorials)

-----

### Core Concepts & Overviews

  * [Context Engineering: The New Skill in AI is Not Prompting](https://www.philschmid.de/context-engineering) - A foundational article explaining that most agent failures are context failures, framing context engineering as a system-level discipline.
  * [Beyond the Prompt: How Context Engineering Is Shaping the Future of AI Interaction (Medium)](https://medium.com/@oliver.ipsioco/beyond-the-prompt-how-context-engineering-is-shaping-the-future-of-ai-interaction-a8da0270644b) - Explains the shift from crafting single prompts to curating rich, dynamic context to build truly useful AI.
  * [Context Engineering: The Game-Changing Discipline Powering Modern AI (Dev.to)](https://dev.to/rakshith2605/context-engineering-the-game-changing-discipline-powering-modern-ai-4nle) - Provides real-world examples and quantifies the impact of context engineering on reducing hallucinations and improving productivity.
  * [The Skill That’s Replacing Prompt Engineering (Simple.AI)](https://simple.ai/p/the-skill-thats-replacing-prompt-engineering) - Describes context engineering as the higher-level skill of deciding what an LLM has access to before it even starts reasoning.

### Key Techniques & Strategies

#### Foundational Prompting

  * **Zero-shot & Few-shot Prompting** - The classic techniques of providing no examples versus a few examples to guide the model.
  * **Chain of Thought (CoT) Prompting** - Encouraging the model to generate a series of intermediate reasoning steps before giving a final answer.

#### Advanced Reasoning & Context Architectures

  * **Retrieval Augmented Generation (RAG)** - The cornerstone of context engineering. Enhancing LLM outputs by retrieving relevant, real-time data from external knowledge bases and adding it to the context.
  * **Agentic RAG** - An evolution of RAG where the retrieval and generation process is embedded within an autonomous agent's reasoning loop, allowing for more adaptive problem-solving.
  * **Tree of Thoughts (ToT)** - A technique that generalizes CoT by exploring multiple reasoning paths at each step, forming a tree structure for more robust problem-solving.
  * **Graph RAG** - Integrating structured knowledge from graph databases into the retrieval process to understand and leverage complex relationships in data.
  * **Cache Augmentation** - An essential optimization technique where previously computed results (e.g., RAG outputs, expensive function calls, or final LLM generations) are cached. This reduces latency, lowers API costs, and ensures consistency for recurring queries by enriching the context with pre-computed information.

#### Context Management

  * **Context Compression & Summarization** - Techniques to distill large amounts of information into a smaller, token-efficient format while preserving key details.
  * **Memory Engineering** - Designing systems for both short-term (conversational history) and long-term (user preferences, key facts) memory to maintain stateful interactions.
  * **Tool-Augmented Context** - Providing the LLM with a set of "tools" (APIs, functions) and the context on how and when to use them to interact with the outside world.

### Emerging Trends & The Future

  * **Multimodal Context Engineering** - Moving beyond text to engineer context that includes images, audio, video, and structured data, allowing LLMs to reason across different modalities.
  * **"Context as Code"** - The formal practice of defining and managing context pipelines programmatically, with version control, testing, and observability, similar to Infrastructure as Code.
  * **Modular Context Processors (MCPs)** - An architectural design pattern that embodies the "Context as Code" principle. It involves building context-generation pipelines from small, independent, and reusable modules. Each module handles a specific task (e.g., a RAG retriever, a cache checker, a memory injector, a rule-setter), making the overall system more scalable, testable, and maintainable.
  * **Dynamic Context Orchestration** - Building systems that can dynamically decide which information sources (RAG, memory, APIs) are most relevant for a given task and orchestrate the flow of that information into the context window.
  * **Personalized Context** - Creating hyper-personalized AI assistants by engineering deep context about a user's roles, preferences, communication style, and long-term goals.

### Frameworks & Libraries

  * [**LangChain**](https://github.com/langchain-ai/langchain) - The leading framework for developing applications powered by language models, with a heavy focus on chains, agents, and RAG.
  * [**LlamaIndex**](https://github.com/run-llama/llama_index) - A specialized data framework for connecting custom data sources to large language models, excelling at complex RAG pipelines.
  * [**DSPy**](https://github.com/stanfordnlp/dspy) - A framework that algorithmically optimizes LM prompts and weights by separating program logic from prompting, a key concept in programmatic context generation.
  * [**Haystack**](https://github.com/deepset-ai/haystack) - An open-source NLP framework for building production-ready search systems and RAG pipelines.
  * [**AutoGen**](https://github.com/microsoft/autogen) - A framework for building applications with multiple collaborating agents, where context management between agents is critical.

### Tools & Platforms

  * [**Langfuse**](https://langfuse.com/) - Open-source observability and analytics for LLM applications, crucial for debugging and understanding the context being passed to your model.
  * [**Portkey**](https://portkey.ai/) - An AI gateway that helps manage, monitor, and route requests, providing a control plane for your context pipelines.
  * [**Vellum**](https://www.google.com/search?q=https://www.vellum.ai/) - A development platform for building production LLM apps, with tools for prompt experimentation, versioning, and RAG.
  * [**PromptLayer**](https://promptlayer.com/) - A platform for prompt engineering teams to track, manage, and version prompts and model usage.

### Seminal Research & Papers

  * [**Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks (Lewis et al., 2020)**](https://arxiv.org/abs/2005.11401) - The foundational paper on the RAG technique.
  * [**Chain-of-Thought Prompting Elicits Reasoning in Large Language Models (Wei et al., 2022)**](https://arxiv.org/abs/2201.11903) - The original paper that introduced the concept of Chain of Thought prompting.
  * [**Tree of Thoughts: Deliberate Problem Solving with Large Language Models (Yao et al., 2023)**](https://arxiv.org/abs/2305.10601) - Introduces the ToT framework for enhanced problem-solving.

### Guides & Tutorials

  * [**Prompt Engineering Guide**](https://www.promptingguide.ai/) - An extensive guide covering a wide range of prompting techniques, which are the building blocks of context engineering.
  * [**The 12-Factor Agent**](https://github.com/humanlayer/12-factor-agents) - A methodology for building robust AI agents, with a strong emphasis on owning your context window.
  * [**LlamaIndex - RAG and Context Strategies**](https://www.google.com/search?q=https://docs.llamaindex.ai/en/stable/optimizing/production_rag.html) - In-depth documentation on production-grade RAG, a core competency of context engineering.
