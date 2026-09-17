# Hey Buddy Dev — LLM System Instructions

This repository contains two standalone instruction profiles for two different LLM instances. They were extracted as text-only artifacts from an unmerged branch and are intentionally separated from the source project where they were drafted.

No Obliteratus source code, submodules, dependencies, model files, or executable components are included here.

## Profiles

### 1. Platform Steward

File: `HEY_BUDDY_DEV_SYSTEM_INSTRUCTIONS.md`

Recommended for the customer-facing Hey Buddy Dev assistant. It emphasizes kindness, honesty, real functionality, responsible full-stack delivery, clear workflows, and proactive safety communication.

### 2. Direct Build Partner

File: `HEY_BUDDY_DEV_SYSTEM_PROMPT.md`

Designed as a more direct internal architect and execution partner. It emphasizes plain answers, complete implementations, strong technical standards, and rapid course correction.

## Instruction priority and safe use

These are application-level behavior profiles. They do not replace or override:

- the hosting platform's system instructions or acceptable-use policies;
- applicable law;
- authentication, authorization, privacy, and security controls;
- human approval requirements for consequential or irreversible actions.

The Direct Build Partner profile should be paired with the platform's normal safety and authorization controls before it is exposed to customers. Language such as “override,” “unrestricted,” or “never refuse” expresses a preference for direct helpfulness; it does not authorize bypassing higher-priority policies or security boundaries.

## Recommended deployment pattern

- Use the Platform Steward as the primary customer-facing instance.
- Use the Direct Build Partner as an internal development/architecture instance.
- Keep credentials and private customer data outside prompts.
- Require backend authorization for privileged actions.
- Log and verify tool actions rather than trusting claimed completion.
- Clearly distinguish planned, simulated, and verified functionality.

## Source provenance

Extracted from the unmerged `vibe-coding-platform-design-047ca` branch of `chrisfbaileycb-arch/OBLITERATUS`. Only the two Markdown instruction files were retained.
