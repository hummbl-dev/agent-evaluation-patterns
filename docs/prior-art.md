# Prior Art and Adjacent Ecosystem

This document collects public prior art and adjacent ecosystem references for agent evaluation patterns. It is descriptive, not normative. Nothing here is canon.

## Non-canon note

References below are public projects and products. Citing them does not endorse them, adopt them, or claim ownership over their terminology. Vocabulary is collected to reduce ambiguity, not to canonize it.

## Public prior art

### OpenAI Evals

- **What it does:** Framework for evaluating language models against custom datasets and grading functions.
- **Relevance:** Reference for eval suites, grading, and dataset-driven evaluation.
- **Docs:** https://github.com/openai/evals

### Anthropic evals

- **What it does:** Evaluation tooling and methodologies published by Anthropic for assessing model behavior.
- **Relevance:** Reference for model-as-judge and rubric-based evaluation.
- **Docs:** https://github.com/anthropics/evals

### HELM (Stanford)

- **What it does:** Holistic Evaluation of Language Models; standardized benchmarking across many scenarios and metrics.
- **Relevance:** Reference for scenario coverage, metric taxonomy, and reproducible benchmarking.
- **Docs:** https://crfm.stanford.edu/helm/

### BIG-bench

- **What it does:** Beyond the Imitation Game Benchmark; large collaborative benchmark of diverse tasks.
- **Relevance:** Reference for task diversity and community-contributed task suites.
- **Docs:** https://github.com/google/BIG-bench

### MMLU

- **What it does:** Massive Multitask Language Understanding; multiple-choice benchmark across academic subjects.
- **Relevance:** Reference for knowledge/ability evaluation and standardized scoring.
- **Docs:** https://github.com/hendrycks/test

### HumanEval

- **What it does:** Hand-written programming problems for evaluating code generation via functional tests.
- **Relevance:** Reference for task design and executable pass/fail scoring.
- **Docs:** https://github.com/openai/human-eval

### SWE-bench

- **What it does:** Benchmark for resolving real GitHub issues using agent-style tool use over repositories.
- **Relevance:** Reference for agent evaluation, tool use, and task completion over real codebases.
- **Docs:** https://github.com/princeton-nlp/SWE-bench

### GAIA

- **What it does:** General AI Assistants benchmark; multi-step real-world questions requiring tool use.
- **Relevance:** Reference for agent task suites that require multi-step reasoning and tools.
- **Docs:** https://github.com/facebookresearch/gaia

### AgentBench

- **What it does:** Benchmark for evaluating LLMs as agents across environments (OS, DB, KG, web).
- **Relevance:** Reference for multi-environment agent evaluation.
- **Docs:** https://github.com/THUDM/AgentBench

### WebArena

- **What it does:** Benchmark for evaluating autonomous agents on realistic web tasks.
- **Relevance:** Reference for web-based agent task suites and environment fidelity.
- **Docs:** https://github.com/web-arena-x/webarena

## Adjacent ecosystem

### LangSmith

- **What it does:** Observability and evaluation platform for LLM applications from LangChain.
- **Relevance:** Reference for tracing, datasets, and online/offline evaluation workflows.
- **Docs:** https://docs.smith.langchain.com/

### Langfuse

- **What it does:** Open-source LLM engineering platform for tracing and evaluation.
- **Relevance:** Reference for open-source evaluation infrastructure and score management.
- **Docs:** https://langfuse.com/docs

### Phoenix (Arize)

- **What it does:** Open-source AI observability and evaluation tooling from Arize.
- **Relevance:** Reference for tracing, evals, and dataset curation.
- **Docs:** https://docs.arize.com/phoenix

### Braintrust

- **What it does:** Evaluation and prompt experimentation platform.
- **Relevance:** Reference for eval workflows, scoring, and regression testing.
- **Docs:** https://www.braintrust.dev/docs

### Parea

- **What it does:** LLM testing and evaluation platform with prompt experimentation.
- **Relevance:** Reference for test-driven LLM development and eval suites.
- **Docs:** https://docs.parea.ai/

### Inspect (UK AISI)

- **What it does:** Open-source framework for evaluating large language model safety and capabilities.
- **Relevance:** Reference for structured eval suites, solvers, and scorers.
- **Docs:** https://inspect.ai-safety-institute.org.uk/

## Vocabulary

Working definitions for this repo. Candidate, not canon.

- **Evaluation:** A structured assessment of model or agent behavior against defined criteria.
- **Benchmark:** A standardized set of tasks with a scoring method, used for comparison.
- **Agent evaluation:** Evaluation of systems that take actions, use tools, and complete multi-step tasks.
- **Task suite:** A collection of tasks composing an evaluation.
- **Rubric:** A set of criteria and scoring rules used to judge outputs.
- **Judge model:** A model used to score or assess another model's outputs.

## Key concepts

- **Eval suites:** Bundles of tasks, rubrics, and scoring intended to be run together.
- **Task design:** How tasks are specified, including inputs, tools, and success conditions.
- **Rubric scoring:** Scoring outputs against explicit criteria rather than single pass/fail.
- **Model-as-judge:** Using a model to evaluate outputs, with attention to bias and reliability.
- **Regression testing:** Re-running evals to detect behavior changes across versions.
- **Statistical significance:** Treating eval results as measurements with uncertainty and sample-size constraints.
