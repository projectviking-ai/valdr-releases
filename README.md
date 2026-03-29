# Valdr Releases

Valdr is a local-first control plane for engineers using AI agents in real work.

It gives teams structure around agent execution so work does not disappear into chat history or depend on whoever remembers the most context. Plans persist, tasks stay tied to requirements, reviews are explicit, and agent sessions leave an inspectable trail.

This repository is the public home for official Valdr release artifacts and release notes.

## What Valdr Is

Valdr helps you run agent-driven work with the same expectations you already have for engineering work: traceability, reviewability, and operational control.

Instead of treating agent output like a disposable conversation, Valdr turns it into a governed workflow with:

- persistent plans and requirements
- tasks that stay linked to execution
- review and approval checkpoints
- reusable capabilities and prompts
- inspectable agent sessions and outcomes

The goal is not novelty. The goal is making agent work reliable enough to use on systems that matter.

## Why Teams Use Valdr

Teams adopt Valdr when ad-hoc prompting stops being enough.

Common reasons include:

- keeping agent behavior aligned with team conventions
- avoiding repeated context setup every session
- making handoffs and reviews visible
- preserving evidence of what changed, why it changed, and who approved it
- keeping execution local-first on infrastructure you control

## What This Repository Contains

This repository is focused on distribution.

You can expect it to contain:

- official Valdr release artifacts
- release notes and version history
- installation guidance for supported distribution paths
- links to broader product documentation as the public docs expand

If you want the packaged binaries for a specific version, start with the [Releases page](https://github.com/projectviking-ai/valdr-releases/releases).

## Install with Homebrew

Homebrew is the primary public install path for the first pass of Valdr distribution.

Initial packaged releases are focused on macOS running on Apple silicon.

```bash
brew tap projectviking-ai/valdr https://github.com/projectviking-ai/homebrew-valdr.git
brew insall valdr
valdr version
```

For now, use this repository's [Releases page](https://github.com/projectviking-ai/valdr-releases/releases) to track published versions and release notes.

## After Installation

Once Valdr is installed, the typical next steps are:

1. Confirm the CLI is available with `valdr --version`.
2. Add license key to ~/.valdr/valdr.lic (signup for a key at https://valdr.ai).
3. Launch the UI with `valdr --port 7777 --pm-home ~/.valdr/pm`
4. Configure Valdr for your local environment and approval posture.
5. Start with a small, traceable workflow instead of trying to automate everything at once.
6. Keep risky actions gated by approvals until your workflow is proven.

Valdr is designed to work well in local-first and private-network setups. If your goal is controlled adoption rather than maximal automation, start there.

## Getting Started with Valdr

Valdr is most useful when you treat agent workflows like engineering systems.

A typical path looks like this:

1. Install the CLI.
2. Define the conventions and capabilities your agents should follow.
3. Plan work with explicit requirements and acceptance criteria.
4. Run agent tasks with review points and approvals.
5. Inspect session history and outcomes so the next run starts with better context than the last one.

## Release Notes

Each published version should include release notes describing what changed in that release. If you are evaluating Valdr for the first time, start with the latest stable release on the [Releases page](https://github.com/projectviking-ai/valdr-releases/releases).

## Current Status

Public distribution is being rolled out incrementally. This README is the first pass of the public-facing release documentation, with Homebrew as the primary install path to document first.
