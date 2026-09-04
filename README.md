# TSA-X (AI Engineering OS)

TSA-X is a high-performance AI Engineering Operating System designed to transform AI assistants into expert engineering partners. By utilizing a strict contract-driven approach and a minimized two-file system, it ensures technical correctness, simplicity, and maintainability. It acts as an orchestration layer between humans and AI, providing a structured environment for complex engineering tasks while maintaining persistent project memory and rigorous validation protocols.

## Stack
* **Game Engine**: HTML5 Canvas / DOM + Vanilla JavaScript
* **AI Engine**: TSA-X Framework (v6.3)
* **Memory System**: TSA Persistent Work Memory
* **LLM Integration**: Optimized for Claude, ChatGPT, Gemini, Cursor, Windsurf, Aider.

## Quick Start
1. **Initialize Project**: Use the command `TSA INIT [AppName] [stack]` to generate the folder structure and configuration.
2. **Setup AI Assistant**:
   * **ChatGPT**: Paste the `[CONTRACT]` from `TSA-X.md` into Custom Instructions.
   * **Claude / Gemini**: Attach `TSA-X.md` and `.ai/memory.md` at the start of every session.
   * **Cursor / Windsurf**: Add `TSA-X.md` to AI Rules or reference it via `@`.
   * **Aider**: Run `aider --read TSA-X.md --read .ai/memory.md`.
3. **Execution**: Define your task, the AI will declare its **MODE** (Patch, Feature, Architect, or Review), and execute according to the contract.
4. **Update Memory**: After each session, copy the `=== MEMORY UPDATE ===` block from the AI's response and paste it into the `[LOG]` section of `memory.md`.

## Architecture
TSA-X operates on a minimalist **2-file system** to maintain context and rules without repo-wide scanning:
* **TSA-X.md**: The permanent contract and scaffold engine. It contains the locked operating rules, engineering behaviors, and protocol keywords that the AI must follow.
* **.ai/memory.md**: The living project memory. It tracks open issues, execution logs, file indices, and environmental constraints. It is the single source of truth for the project's current state.

## Features
* **Contract-Driven Engineering**: A locked `[CONTRACT]` ensures the AI prioritizes correctness and simplicity over all else.
* **Intelligent Mode Selector**: Dynamically switches focus between `PATCH` (small fixes), `FEATURE` (new capabilities), `ARCHITECT` (major changes), and `REVIEW` (analysis).
* **Automated Debug Loop**: A self-healing protocol that classifies, groups, and fixes bugs through iterative validation cycles.
* **Rate Limit Protocol**: Multi-tiered protection (Exponential Backoff, Token Buckets, Daily Counters) for external API calls, specifically optimized for Gemini API tiers.
* **Scaffold Engine**: Instant project initialization with standardized documentation and folder structures.

## Folder Structure
```text
game_anak_edukasi/
├── .ai/
│   └── memory.md           # Persistent work memory (CRITICAL)
├── TSA-X.md                # AI Engineering OS Contract
├── README.md               # This file
└── index.html              # Main game file (Pintar Kata - Entry Point)
```

## Env Vars
* `GEMINI_API_KEY`: Required for projects utilizing the Gemini API stack.
* API quotas and limits are tracked in `memory.md` under `[KNOWN LIMITS]`.

## License
MIT License. Refer to the original repository at [github.com/anoramyid/TSA](https://github.com/anoramyid/TSA) for updates and community contributions.
