# basic-medical-qa

## Motivation
My idea was to first build a basic application that answers medical questions using an LLM to get a feel for the domain and the technologies involved. It does not need to use RAG or GQA.

## Goal
Build a simple LLM-based app that answers medical questions.
Since we’re focusing on a pure LLM-based QA system, the main goal is to:

- Test how well an LLM answers medical questions without external retrieval.
- Identify potential weaknesses like hallucinations or factual inaccuracies.
- Establish a baseline before adding retrieval (RAG) later.

## Initial Setup
Using one general LLM + one fine-tuned medical model allows us to:

- Compare general knowledge (e.g., GPT-4) vs. domain expertise (e.g., BioGPT).
- Identify hallucination risks in general models.
- Leverage medical-specific models for more accurate extractions.

## Phase 1: Compare Model Outputs

1. Ask both GPT-4 and BioGPT the same medical question.
2. Compare answers to detect hallucinations vs. evidence-based responses.

## Phase 2: Hybrid QA System (optional)

- Use BioGPT to extract facts from medical texts.
- Let GPT-4 format responses into more readable answers.

