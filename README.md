
<div align="center">
  <img src="https://github.com/ranganaths/.github/raw/main/assets/title.png" alt="Rapier – minimalist LLM framework" width="600"/>
</div>

<!-- For translation, replace English with [English](https://github.com/ranganaths/Rapier/blob/main/README.md), and remove the link for the target language. -->


![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
[![Docs](https://img.shields.io/badge/docs-latest-blue)](https://ranganaths.github.io/Rapier/)
 
Rapier is a (https://github.com/ranganaths/Rapier/blob/main/rapier/__init__.py) minimalist LLM framework

- **Lightweight**: Zero bloat, zero dependencies, zero vendor lock-in.
  
- **Expressive**: Everything you love—([Multi-](https://ranganaths.github.io/rapier/design_pattern/multi_agent.html))[Agents](https://ranganaths.github.io/rapier/design_pattern/agent.html), [Workflow](https://ranganaths.github.io/rapier/design_pattern/workflow.html), [RAG](https://ranganaths.github.io/rapier/design_pattern/rag.html), and more.

- **[Agentic Coding](https://zacharyhuang.substack.com/p/agentic-coding-the-most-fun-way-to)**: Let AI Agents (e.g., Cursor AI) build Agents—10x productivity boost!

Get started with Pocket Flow:
- To install, ```pip install rapier```or just copy the [source code](https://github.com/ranganaths/rapier/blob/main/rapier/__init__.py) (only 100 lines).
- To learn more, check out the [documentation](https://ranganaths.github.io/rapier/). To learn the motivation, read the [story](https://zacharyhuang.substack.com/p/i-built-an-llm-framework-in-just).
- Have questions? Check out this [AI Assistant](https://chatgpt.com/g/g-677464af36588191b9eba4901946557b-pocket-flow-assistant), or [create an issue!](https://github.com/ranganaths/rapier/issues/new)
- 🎉 Join our [Discord](https://discord.gg/hUHHE9Sa6T) to connect with other developers building with Pocket Flow!
- 🎉 Pocket Flow is initially Python, but we now have [Typescript](https://github.com/ranganaths/rapier-Typescript), [Java](https://github.com/ranganaths/rapier-Java), [C++](https://github.com/ranganaths/rapier-CPP) and [Go](https://github.com/ranganaths/rapier-Go) versions!

## Why Pocket Flow?

Current LLM frameworks are bloated... You only need 100 lines for LLM Framework!

<div align="center">
  <img src="https://github.com/ranganaths/.github/raw/main/assets/meme.jpg" width="400"/>


  |                | **Abstraction**          | **App-Specific Wrappers**                                      | **Vendor-Specific Wrappers**                                    | **Lines**       | **Size**    |
|----------------|:-----------------------------: |:-----------------------------------------------------------:|:------------------------------------------------------------:|:---------------:|:----------------------------:|
| LangChain  | Agent, Chain               | Many <br><sup><sub>(e.g., QA, Summarization)</sub></sup>              | Many <br><sup><sub>(e.g., OpenAI, Pinecone, etc.)</sub></sup>                   | 405K          | +166MB                     |
| CrewAI     | Agent, Chain            | Many <br><sup><sub>(e.g., FileReadTool, SerperDevTool)</sub></sup>         | Many <br><sup><sub>(e.g., OpenAI, Anthropic, Pinecone, etc.)</sub></sup>        | 18K           | +173MB                     |
| SmolAgent   | Agent                      | Some <br><sup><sub>(e.g., CodeAgent, VisitWebTool)</sub></sup>         | Some <br><sup><sub>(e.g., DuckDuckGo, Hugging Face, etc.)</sub></sup>           | 8K            | +198MB                     |
| LangGraph   | Agent, Graph           | Some <br><sup><sub>(e.g., Semantic Search)</sub></sup>                     | Some <br><sup><sub>(e.g., PostgresStore, SqliteSaver, etc.) </sub></sup>        | 37K           | +51MB                      |
| AutoGen    | Agent                | Some <br><sup><sub>(e.g., Tool Agent, Chat Agent)</sub></sup>              | Many <sup><sub>[Optional]<br> (e.g., OpenAI, Pinecone, etc.)</sub></sup>        | 7K <br><sup><sub>(core-only)</sub></sup>    | +26MB <br><sup><sub>(core-only)</sub></sup>          |
| **rapier** | **Graph**                    | **None**                                                 | **None**                                                  | **100**       | **+56KB**                  |

</div>

## How does Pocket Flow work?

The [100 lines](https://github.com/ranganaths/rapier/blob/main/rapier/__init__.py) capture the core abstraction of LLM frameworks: Graph!
<br>
<div align="center">
  <img src="https://github.com/ranganaths/.github/raw/main/assets/abstraction.png" width="900"/>
</div>
<br>

From there, it's easy to implement popular design patterns like ([Multi-](https://ranganaths.github.io/rapier/design_pattern/multi_agent.html))[Agents](https://ranganaths.github.io/rapier/design_pattern/agent.html), [Workflow](https://ranganaths.github.io/rapier/design_pattern/workflow.html), [RAG](https://ranganaths.github.io/rapier/design_pattern/rag.html), etc.
<br>
<div align="center">
  <img src="https://github.com/ranganaths/.github/raw/main/assets/design.png" width="900"/>
</div>
<br>
✨ Below are basic tutorials:

<div align="center">
  
|  Name  | Difficulty    |  Description  |  
| :-------------:  | :-------------: | :--------------------- |  
| [Chat](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-chat) | ☆☆☆ <br> *Dummy*   | A basic chat bot with conversation history |
| [Structured Output](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-structured-output) | ☆☆☆ <br> *Dummy* | Extracting structured data from resumes by prompting |
| [Workflow](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-workflow) | ☆☆☆ <br> *Dummy*   | A writing workflow that outlines, writes content, and applies styling |
| [Agent](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-agent) | ☆☆☆ <br> *Dummy*   | A research agent that can search the web and answer questions |
| [RAG](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-rag) | ☆☆☆ <br> *Dummy*   | A simple Retrieval-augmented Generation process |
| [Batch](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-batch) | ☆☆☆ <br> *Dummy* | A batch processor that translates markdown content into multiple languages |
| [Streaming](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-llm-streaming) | ☆☆☆ <br> *Dummy*   | A real-time LLM streaming demo with user interrupt capability |
| [Chat Guardrail](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-chat-guardrail) | ☆☆☆ <br> *Dummy*  | A travel advisor chatbot that only processes travel-related queries |
| [Map-Reduce](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-map-reduce) | ★☆☆ <br> *Beginner* | A resume qualification processor using map-reduce pattern for batch evaluation |
| [Multi-Agent](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-multi-agent) | ★☆☆ <br> *Beginner* | A Taboo word game for asynchronous communication between two agents |
| [Supervisor](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-supervisor) | ★☆☆ <br> *Beginner* | Research agent is getting unreliable... Let's build a supervision process|
| [Parallel](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-parallel-batch) | ★☆☆ <br> *Beginner*   | A parallel execution demo that shows 3x speedup |
| [Parallel Flow](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-parallel-batch-flow) | ★☆☆ <br> *Beginner*   | A parallel image processing demo showing 8x speedup with multiple filters |
| [Majority Vote](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-majority-vote) | ★☆☆ <br> *Beginner* | Improve reasoning accuracy by aggregating multiple solution attempts |
| [Thinking](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-thinking) | ★☆☆ <br> *Beginner*   | Solve complex reasoning problems through Chain-of-Thought |
| [Memory](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-chat-memory) | ★☆☆ <br> *Beginner* | A chat bot with short-term and long-term memory |
| [Text2SQL](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-text2sql) | ★☆☆ <br> *Beginner* | Convert natural language to SQL queries with an auto-debug loop |
| [MCP](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-mcp) | ★☆☆ <br> *Beginner* |  Agent using Model Context Protocol for numerical operations |
| [A2A](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-a2a) | ★☆☆ <br> *Beginner* | Agent wrapped with Agent-to-Agent protocol for inter-agent communication |
| [Web HITL](https://github.com/ranganaths/rapier/tree/main/cookbook/rapier-web-hitl) | ★☆☆ <br> *Beginner* | A minimal web service for a human review loop with SSE updates |

</div>

👀 Want to see other tutorials for dummies? [Create an issue!](https://github.com/ranganaths/rapier/issues/new)

## How to Use Pocket Flow?

🚀 Through **Agentic Coding**—the fastest LLM App development paradigm-where *humans design* and *agents code*!

<br>
<div align="center">
  <a href="https://zacharyhuang.substack.com/p/agentic-coding-the-most-fun-way-to" target="_blank">
    <img src="https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F423a39af-49e8-483b-bc5a-88cc764350c6_1050x588.png" width="700" alt="IMAGE ALT TEXT" style="cursor: pointer;">
  </a>
</div>
<br>

✨ Below are examples of more complex LLM Apps:

<div align="center">
  
|  App Name     |  Difficulty    | Topics  | Human Design | Agent Code |
| :-------------:  | :-------------: | :---------------------: |  :---: |  :---: |
| [Danganronpa Simulator](https://github.com/ranganaths/rapier-Tutorial-Danganronpa-Simulator) <br> <sup><sub>Forget the Turing test. Danganronpa, the ultimate AI experiment!</sup></sub> | ★★★ <br> *Advanced*   | [Workflow](https://ranganaths.github.io/rapier/design_pattern/workflow.html) <br> [Agent](https://ranganaths.github.io/rapier/design_pattern/agent.html) | [Design Doc](https://github.com/ranganaths/rapier-Tutorial-Danganronpa-Simulator/blob/main/docs/design.md) | [Flow Code](https://github.com/ranganaths/rapier-Tutorial-Danganronpa-Simulator/blob/main/flow.py)
| [Codebase Knowledge Builder](https://github.com/ranganaths/Tutorial-Codebase-Knowledge) <br> <sup><sub>Life's too short to stare at others' code in confusion</sup></sub> |  ★★☆ <br> *Medium* | [Workflow](https://ranganaths.github.io/rapier/design_pattern/workflow.html) | [Design Doc](https://github.com/ranganaths/Tutorial-Codebase-Knowledge/blob/main/docs/design.md) | [Flow Code](https://github.com/ranganaths/Tutorial-Codebase-Knowledge/blob/main/flow.py)
| [Build Cursor with Cursor](https://github.com/ranganaths/Tutorial-Cursor) <br> <sup><sub>We'll reach the singularity soon ...</sup></sub> | ★★★ <br> *Advanced*   | [Agent](https://ranganaths.github.io/rapier/design_pattern/agent.html) | [Design Doc](https://github.com/ranganaths/Tutorial-Cursor/blob/main/docs/design.md) | [Flow Code](https://github.com/ranganaths/Tutorial-Cursor/blob/main/flow.py)
| [Ask AI Paul Graham](https://github.com/ranganaths/Tutorial-YC-Partner) <br> <sup><sub>Ask AI Paul Graham, in case you don't get in</sup></sub> | ★★☆ <br> *Medium*  | [RAG](https://ranganaths.github.io/rapier/design_pattern/rag.html) <br> [Map Reduce](https://ranganaths.github.io/rapier/design_pattern/mapreduce.html) <br> [TTS](https://ranganaths.github.io/rapier/utility_function/text_to_speech.html) | [Design Doc](https://github.com/ranganaths/Tutorial-AI-Paul-Graham/blob/main/docs/design.md) | [Flow Code](https://github.com/ranganaths/Tutorial-AI-Paul-Graham/blob/main/flow.py)
| [Youtube Summarizer](https://github.com/ranganaths/Tutorial-Youtube-Made-Simple)  <br> <sup><sub> Explain YouTube Videos to you like you're 5 </sup></sub> | ★☆☆ <br> *Beginner*   | [Map Reduce](https://ranganaths.github.io/rapier/design_pattern/mapreduce.html) |  [Design Doc](https://github.com/ranganaths/Tutorial-Youtube-Made-Simple/blob/main/docs/design.md) | [Flow Code](https://github.com/ranganaths/Tutorial-Youtube-Made-Simple/blob/main/flow.py)
| [Cold Opener Generator](https://github.com/ranganaths/Tutorial-Cold-Email-Personalization)  <br> <sup><sub> Instant icebreakers that turn cold leads hot </sup></sub> | ★☆☆ <br> *Beginner*   | [Map Reduce](https://ranganaths.github.io/rapier/design_pattern/mapreduce.html) <br> [Web Search](https://ranganaths.github.io/rapier/utility_function/websearch.html) |  [Design Doc](https://github.com/ranganaths/Tutorial-Cold-Email-Personalization/blob/master/docs/design.md) | [Flow Code](https://github.com/ranganaths/Tutorial-Cold-Email-Personalization/blob/master/flow.py)


</div>


