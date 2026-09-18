
  
## Start here

- [Introduction](https://docs.typesafe.ai/introduction) — What Jev is, how System One models differ from text-generation models, and the Choice, Score, and Noul primitives.
- [Quick start](https://docs.typesafe.ai/introduction/quickstart) — The shortest path from an API key to a typed decision in Python or JavaScript.
- [How to build with TypeSafe](https://docs.typesafe.ai/concepts/how-to-build-with-system-one) — Design guidance for decomposing a workflow into narrow judgments while keeping policy and side effects in code.
- [TypeSafe Console](https://console.typesafe.ai/) — Create keys and inspect live Jev requests.

## Official resources

### Product and documentation

- [TypeSafe AI](https://typesafe.ai/) — Official product site for System One models and Jev.
- [Documentation](https://docs.typesafe.ai/) — Guides, SDK references, patterns, cookbooks, and the HTTP API.
- [HTTP API reference](https://docs.typesafe.ai/api) — Request and response contract for direct API integrations.
- [Interactive demos](https://docs.typesafe.ai/demos) — Official hands-on examples, including the smart-home assistant.
- [Workflow evals](https://evals.typesafe.ai/) — TypeSafe's published workflows, model comparisons, methodology, and example queries.

### SDKs and developer tools

- [JavaScript SDK](https://github.com/typesafe-ai/typesafe-sdk-js) — Official JavaScript and TypeScript client with inferred answer types.
- [Python SDK](https://github.com/typesafe-ai/typesafe-sdk-python) — Official synchronous and asynchronous Python client.
- [System One Adapter](https://github.com/typesafe-ai/system-one-adapter-python) — Drop-in Python adapter for running the same typed interface over OpenAI, Anthropic, and OpenAI-compatible LLM APIs.
- [TypeSafe Agent Skills](https://github.com/typesafe-ai/skills) — Official agent skill for designing TypeSafe workflows from Claude Code, Codex, and other skill-compatible agents.
- [TypeSafe GitHub organization](https://github.com/typesafe-ai) — Source repositories maintained by TypeSafe.

### Concepts, patterns, and cookbooksCompute

- [Primitives](https://docs.typesafe.ai/primitives) — Choice, Score, and Noul, including their result shapes and when to use each one.
- [Confidence](https://docs.typesafe.ai/confidence) — How confidence differs from answer probability and how to use it as an architectural control.
- [Patterns](https://docs.typesafe.ai/patterns) — Confidence-gated routing, composite scoring, speculative fan-out, and intent routing.
- [Example use cases](https://docs.typesafe.ai/concepts/use-case-map) — A map from real-world workflows to typed judgments.
- [Cookbooks](https://docs.typesafe.ai/cookbooks/parallel_questions) — Reproducible implementations for parallel questions, reranking, semantic search, guardrails, extraction, classification, and more.
- [Agent skill guide](https://docs.typesafe.ai/agent-skill) — Installation and usage instructions for the official TypeSafe skill.

### Research and writing

- [Introducing System One Models & Jev](https://typesafe.ai/blog/introducing-system-one-models-and-jev) — Launch post, product thesis, published results, and explicit limitations.
- [Manifesto](https://typesafe.ai/manifesto) — TypeSafe's case for machine-native intelligence built for software rather than conversation.
- [The Bitterest Lesson](https://typesafe.ai/blog/bitterest-lesson) — Why optimizing the wrong task can dominate gains from scale.
- [AI: too good to be true, too bad to be useful](https://typesafe.ai/blog/ai-too-good-to-be-true-too-bad-to-be-useful-typesafe-ai) — The argument for moving beyond preference-optimized chat models in automation.

### Community and updates

- [Discord](https://discord.gg/typesafe) — Official community server for builders, support, and discussion.
- [Show and Tell](https://discord.com/channels/1483217544214085663/1483217545040232493) — Builder demos and work in progress; joining the Discord server is required.
- [X](https://x.com/typesafeai) — Product and research updates.
- [LinkedIn](https://www.linkedin.com/company/typesafe-ai/) — Company announcements and hiring updates.

## Community projects

Community projects are independent unless their repository says otherwise. Read the code, licenses, data-handling notes, and evaluation caveats before using them in a consequential system.

### Client libraries and integrations

- [Advocaat](https://github.com/pithings/advocaat) — Small TypeScript client with ergonomic tagged helpers for typed chances, choices, and scores.
- [HA-Jev](https://github.com/AboveColin/HA-Jev) — Home Assistant integration that turns typed questions about entity state into sensors and automation actions, with entities reporting daily calls, tokens, and estimated cost and a token budget that halts evaluation; answers carry no explanation, so it is not suitable for safety decisions.
- [pi-typesafe](https://github.com/DevMortimer/pi-typesafe) — Pi extension and library that gives the agent and other extensions one consented, key-managed TypeSafe client with a batched `typesafe_evaluate` tool and offline-testable transport; requests are billable and opt-in per user.
- [RubyLLM TypeSafe](https://github.com/kieranklaassen/ruby_llm-typesafe) — TypeSafe provider for RubyLLM 2 with offline model metadata and typed responses.
- [s1-rs](https://github.com/AbdelStark/s1-rs) — Rust derive layer for Choice, Score, Noul, typed question sets, confidence gates, and network-free testing.
- [TypeSafe AI for Rust](https://github.com/Twister915/typesafe-ai) — Rust client with asynchronous and blocking transports, typed responses, observable retries, and inspectable errors.
- [typesafe-ai-rails](https://github.com/GenieRobot/typesafe-ai-rails) — Community Rails integration for TypeSafe's System One API, built on typesafe-sdk, with Rails configuration, persisted usage and cost telemetry, and opt-in confidence policies for Choice and Score answers.
- Rust [typesafe-rs](https://github.com/AbdelStark/typesafe-rs) — Latency-focused Rust transport SDK designed around behavioral parity with the official clients.
- Elixir [typesafe_sdk](https://github.com/nshkrdotcom/typesafe_sdk) — Elixir SDK for TypeSafe AI and Jev with typed Choice, Score, and Noul structs, configurable retries, and upstream API parity.
- Ruby [typesafe-sdk](https://github.com/joshmn/typesafe-sdk) — Community Ruby client for TypeSafe's System One API with typed Noul, Choice, and Score questions, retries, model listing, and thread-safe pooled HTTP connections; requires Ruby 3.1 or newer and has no async client.
- [TypeSafeAI.Net](https://github.com/Hawxy/TypeSafeAI.Net) — .NET client for TypeSafe's API with Noul, Choice, and Score question sets, HttpClientFactory and dependency injection support, plus Microsoft.Extensions.AI guardrail, routing, tool, and evaluator adapters.
- [Vercel AI Gateway](https://vercel.com/ai-gateway/models/jev) — Third-party hosted gateway entry for calling Jev through Vercel's AI SDK and gateway.

### Agent, developer tooling and harness

- [Bicameral](https://github.com/AbdelStark/bicameral) — Pi coding harness where an LLM writes while Jev supplies typed reflexes for policy, loop detection, and review; explicitly not a sandbox.
- [Every](https://github.com/sufianetaouil/every) — Semantic code search CLI that asks a yes/no question of every function and ranks the resulting probabilities.
- [Jev MCP](https://github.com/blakestone-x/jev-mcp) — Python MCP server exposing classify, score, check, match, and screen tools to MCP-compatible agents.

- [jev-axi](https://github.com/shiftynick/jev-axi) — Agent-ergonomic CLI following the AXI conventions that gives coding agents Jev judgments for blocking risky tool calls, screening fetched content for prompt injection, triaging build logs, flagging risky diffs, and filtering or ranking many items; its own benchmark found agents using it read fewer files but cost the same, so it is meant for judgments rather than as a substitute for reading code.
- [jev-mobile](https://github.com/Friedjof/jev-mobile) — Experimental Android agent that uses Jev for bounded, per-step choices over prevalidated UI actions, with confidence gates, pagination, escalation, and optional LLM planning; currently a proof of concept tested mainly against Android Settings.
- [jevcal](https://github.com/abhixhek/jevcal) — CLI that fits a per-question confidence threshold to a target accuracy on your own labeled data, verifies it on a held-out split, estimates how much traffic still needs a fallback model, and re-checks the locked thresholds in CI; publishes no Jev results of its own, and thresholds fitted on fewer than about 100 labeled rows should not be trusted.
- [pi-jev](https://github.com/y0usaf/pi-jev) — Pi extension with a shadow-mode tool-call gate, output judge, and a general typed `jev_ask` tool.
- [pi-warden](https://github.com/DevMortimer/pi-warden) — Pi guardrails built on pi-typesafe that return Jev's verdict to the agent as a held tool result or a short steer instead of a dialog, check writes against a project rules file, and grade their own holds against the user's next message on recorded sessions; the action guard is calibrated on one user's 17k calls, the other guards on synthetic cases only.
- [Supercov](https://github.com/supercorp-ai/supercov) — Code quality for coding agents: Jev scores each source file so the agent knows what to fix first.
- [TypeSafe MCP](https://github.com/itsmostafa/typesafe-mcp) — Go CLI and single-binary MCP server with setup for Claude Desktop, Claude Code, and Codex.
- [Jev-mcp](https://github.com/jkudish/jev-mcp) Proof of concept MCP for Typesafe's new Jev AI model
- [foreman](https://github.com/thruwire/foreman) Software Factory Foreman based on TypeSafe Jev model
- [jev-codex-router](https://github.com/0xNatoshi/jev-codex-router) Per-turn model & reasoning routing for Codex, driven by Jev (TypeSafe System One): picks the model, thinking depth and speed mode for every turn.
- [safer-with-jev](https://github.com/andrelandgraf/safer-with-jev) Neon Function proxy for the Neon AI Gateway with TypeSafe Jev routing.
- [CC](https://github.com/GhalebDweikat/CC) A calibrated context sieve for Claude Code: every tool result is judged by a System One model before it enters context.
- [blink](https://github.com/ellipsis-dev/blink) Codebase search powered by Jev from

## Code-Review
- [Jev Review](https://github.com/devagrawal09/jev-review) — Staged code-review workflow and local dashboard that follows structured signals through focused Jev calls.
- [jev-review](https://github.com/NiazMorshed2007/jev-review) Local-first MCP plugin for continuous software-quality review by AI coding agents, powered by Jev.
### Browser agents

- [Jev Browser](https://github.com/vlad-terin/jev-browser) — Agent skill and runtime that lets Jev select browser actions inside a continuous observation-action-verification loop.
- [Jev Ultrafast](https://github.com/browser-use/jev-ultrafast) — Browser Use agent with a dynamic indexed action space, batched operation and target decisions, traces, and a measured Google Flights demo.

### Games, robotics, and interactive demos

- [Crowdcheck](https://crowdcheck-ai.vercel.app/) — Live demo that tests a 144-character post on 10,000 persistent synthetic personas: code decides who sees it, and batched Jev calls return read, like/dislike, agreement, repost, follow, and block probabilities per persona group; posting requires Google sign-in, post text is sent to Jev through Vercel AI Gateway, and the simulated reactions are not a forecast of real audience behavior.
- [HEIST//ONE](https://github.com/AbdelStark/heist-one) — Observable browser stealth game where Jev supplies batched typed judgments for six guards while deterministic code owns the simulation and validates every proposal; includes a Decision Lens, scripted offline mode, evidence traces, tests, and one documented live sandbox extraction.
- [Jev Drone](https://github.com/RomanSlack/jev-drone) — MuJoCo quadrotor stack that keeps control and safety in code while using Jev for slower tactical judgments.
- [Jev Plays Pokémon](https://github.com/anxkhn/JevPlaysPokemon) — FireRed and Showdown harness where Jev battles the Elite Four by picking a move or switch from the current Pokémon, moves, stats, and opponent HP.
- [Jev Plays StarCraft](https://github.com/phyous/tsai-sc) — Structured-state harness, verified run, probability trace, and evidence bundle for the original StarCraft shareware campaign.
- [Jev Search](https://github.com/superagents-lab/jev-search) — Web search demo using Jev's typed Choice and Noul judgments to select sources, time ranges, and query candidates, then rank results retrieved through Search1API; relevance scores are model judgments, not verified accuracy.
- [TypeSafe Mario](https://github.com/fhshaik/typesafe-mario) — NES controller experiment that turns emulator telemetry into structured state and has Jev choose legal actions.
- [TypeSafe Typewriter](https://typesafe-demo.val.run/) — Live Val Town demo that updates 16 typed judgments as text changes.

### Evaluations and independent research

- [calibre](https://github.com/FirasSX914/calibre) — Independent calibration measurement of Jev on two labelled datasets, Banking77 and Web of Science, with a Jev to frontier cascade priced per row from measured tokens; the protocol was frozen before any result and the raw JSONL and figures are committed, and no routing parameter transferred between the two datasets, as the optimal threshold, the sign of the accuracy gap between the two models, and whether routing paid for itself all changed; the Web of Science labels come from publication metadata rather than per-document annotation, so part of the error measured there is label ambiguity.
- [Jev Judge vs Dimension Scores](https://agentjournal.dev/blog/llm-judge-vs-feature-extraction/) — Independent measurement on three classification tasks: one direct Jev question per row against 12–14 Jev-scored dimensions with locally fitted weights, 5,477 test rows and 34.1M input tokens for $1.43; decomposition reached 0.9076 against 0.8373 on Japanese NLI but flagged about 25× more hard benign rows as attacks, and four repair attempts failed, on dimensions the author wrote himself.
- [Jev Rerank Bench](https://github.com/anessbelbati/jev-rerank-bench) — Reranking comparison with raw provider responses, scoring code, dataset-level results, uncertainty intervals, and documented limitations.
- [Jev Spam Eval](https://github.com/bitnovus/jev-spam-eval) — Exploratory zero-shot spam study against trained TF-IDF baselines, including results and explicit post-hoc-tuning caveats.
- [TypeSafe AI Benchmark](https://github.com/iammrduncan/typesafe-ai-benchmark) — Side-by-side Jev and Qwen-on-Cerebras comparison with raw exports, cost accounting, methodology, and task-specific limitations.

### Showcases and field notes

- [Browser Use + Jev](https://x.com/gregpr07/status/2100411066966749359) — Gregor Zunic's real-time flight-search demo and short description of the dynamic DOM action space.
- [Internal classifier field note](https://x.com/identityTorn/status/2100475121324728615) — A builder's early matched-precision comparison against a private fine-tuned Qwen classifier; useful anecdotal evidence, not a reproducible benchmark.
- [Jev Typewriter launch post](https://x.com/stevekrouse/status/2100287368221659289) — Steve Krouse's playable 16-judgment demo and video.
- [Qwen on Cerebras comparison](https://x.com/iamMrDuncan/status/2100467548298899918) — Shannon's video and source-backed comparison of a structured-output LLM baseline with Jev.
- [Typed Decisions, Not Chat](https://warmersun.com/jev/) — Independent technical walkthrough that distinguishes TypeSafe's published claims from what the public evidence establishes.
- [typesafe-ai-playground](https://github.com/markjaquith/typesafe-ai-playground)

### Jev-Like-Decisions-Engine

- [NanoJev](https://github.com/TianyuCodings/NanoJev) A nano replica of Jev: parallel decisions, dynamic candidates, and an end-to-end training pipeline.
- [OpenJev](https://github.com/TheoLeeCJ/openjev) — Independent open-model research baseline for direct typed option scoring; it reproduces the interface pattern, not Jev's undisclosed model or training.
- [openvons](https://github.com/genai-craft/openvons) a decision layer that answers finite choices with probabilities

### Compute-Use and Mobile-Use
- [mobile-jev](https://github.com/droidrun/mobile-jev) One goal. A real Android phone. Jev makes the decisions.
- [agent-desktop](https://github.com/lahfir/agent-desktop) Agent Desktop gives any agent reliable computer use on the desktop. Built with Rust, it sees any app's real UI structure through OS accessibility trees and operates it — refs stay stable and actions stay safe to retry, instead of guessing from pixels.
- [typesafe-computer-use](https://github.com/awlevin/typesafe-computer-use) Computer use for about $0.0002 a step: OCR the screen, classify the next action with TypeSafe, click. macOS.
- [cua](https://github.com/trycua/cua) Give AI agents computers they can use.
Cua provides open-source desktop automation, isolated cloud desktops, local macOS VMs, and benchmarks for evaluating computer-use agents.

## Video
- [jevmeter](https://github.com/ChetasLua/jevmeter) Put a live Jev (TypeSafe) meter on any video: every sentence scored, rendered as a 16:9 edit