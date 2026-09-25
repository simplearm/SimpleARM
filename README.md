# SimpleARM: Simple Agentic Memory for Generalist Robot Policies

[![Project Page](https://img.shields.io/badge/Project-Page-111827?style=flat-square)](https://simplearm.github.io)

**Code will be released soon.**

**Paper will be released soon.**

## Abstract

Most existing memory systems for vision retain or compress past observations. Robot control poses a different problem: what matters for future action may not be a past frame, but a state that must be accumulated and updated through interaction, such as object identity, task progress, or an ordered trajectory. We introduce *Simple Agentic Robot Memory* (**SimpleARM**), a training-free memory layer for frozen generalist robot policies. Rather than storing visual history indiscriminately, SimpleARM uses the task instruction to determine what should be remembered, maintains a compact structured state as the episode unfolds, and exposes that state only when it is relevant to the current decision. We evaluate SimpleARM on RoboMME, a benchmark of history-dependent robot manipulation tasks that require reasoning over information no longer available in the current observation. Across all 16 tasks and three policy seeds, SimpleARM achieves **67.17%** mean success, compared with 32.70% for the same system without memory and 44.51% for the strongest previously reported non-oracle method. Matched interventions further show that removing relation, reference, progress, or route state primarily harms the tasks that require the corresponding information. These results support a state-based view of robot memory: effective memory for control is not simply retained visual history, but compact task-relevant state derived from the interaction history.
