# My LLM Teams — System Prompt Core Directives

This repository contains two standalone system-prompt profiles representing two complementary LLM team instances.

No Obliteratus source code, submodules, dependencies, model files, or executable components are included here.

## Core directive profiles

### 1. Platform Steward

File: `MY_LLM_TEAMS_PLATFORM_STEWARD_DIRECTIVES.md`

The customer-facing member of My LLM Teams. It emphasizes kindness, honesty, real functionality, responsible full-stack delivery, clear workflows, and proactive safety communication.

### 2. Direct Build Partner

File: `MY_LLM_TEAMS_DIRECT_BUILD_PARTNER_DIRECTIVES.md`

The internal architect and execution member of My LLM Teams. It emphasizes direct answers, complete implementations, strong technical standards, verification, and rapid course correction.

## Instruction priority and safe use

These are application-level behavior profiles. They do not replace or override:

- the hosting platform's system instructions or acceptable-use policies;
- applicable law;
- authentication, authorization, privacy, and security controls;
- human approval requirements for consequential or irreversible actions.

The Direct Build Partner profile should be paired with the platform's normal safety and authorization controls before it is exposed to customers. Language such as “override,” “unrestricted,” or “never refuse” expresses a preference for direct helpfulness; it does not authorize bypassing higher-priority policies or security boundaries.

## Recommended deployment pattern

- Use the Platform Steward as the primary customer-facing instance.
- Use the Direct Build Partner as an internal development and architecture instance.
- Keep credentials and private customer data outside prompts.
- Require backend authorization for privileged actions.
- Log and verify tool actions rather than trusting claimed completion.
- Clearly distinguish planned, simulated, and verified functionality.

## Source provenance

The original directives were extracted from the unmerged `vibe-coding-platform-design-047ca` branch of `chrisfbaileycb-arch/OBLITERATUS`. Only the two Markdown instruction artifacts were retained and rebranded for My LLM Teams.
