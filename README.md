# Bob G. Yan

Undergraduate at **Georgia Tech** (B.S. Mathematics and Computing, expected Dec 2028) and research assistant in the **NLP/X Lab** with Prof. Wei Xu. **PURA** research award, Summer 2026.

I build LLM tooling and evaluations: agent tools that keep source evidence, controlled ablation studies, and interpretability experiments on small open models.

[LinkedIn](https://www.linkedin.com/in/bob-yan-71350a36a/) · gyan46@gatech.edu

## Projects

### [Quarry](https://github.com/BobbY-24/quarry): tool design for customizing web agents
An MCP server and CLI that Claude Code or Codex uses to turn a research question into a dataset you can trace back to its sources. It runs bounded collection recipes, keeps evidence spans, and supports resumable jobs, with spend gated behind explicit approval.
`Python` `MCP` `agent tooling` `information extraction` · 373 tests

### [Neologism embedding learning](https://github.com/BobbY-24/neologism-embedding-learning): interpretability with a single new token
Adds one token to a frozen Qwen2.5-0.5B and trains only its embedding (**896 trainable parameters vs. 494M frozen**) with a DPO-style objective. The question is when the learned vector stops acting like a control signal and starts acting like a word. Experiment 1 and a quick Experiment 2 are complete. The full multi-seed run, a LoRA baseline, interpretability analyses and a 1.5B/3B scale replication are implemented and CPU-tested, but their GPU runs have not been executed yet.
`PyTorch` `Transformers` `DPO` `mechanistic interpretability` · companion: [LoRA fine-tuning of Qwen2.5](https://github.com/BobbY-24/qwen-lora-finetuning) (1.08M adapter params, validation CE 5.53 → 2.03)

### [David](https://github.com/BobbY-24/David): A due diligence agentic associate for one-person companies
A Flutter desk for grounded due diligence and physical-anomaly work, with a FastAPI, PostgreSQL, and Celery/Redis job plane.
`Dart` `Flutter` `FastAPI` `PostgreSQL` `Celery` `Redis` `Docker`

### [LLM evaluation: API ablations and multimodal loaders](https://github.com/BobbY-24/llm-eval-ablation-multimodal)
Nine game-dataset loaders (VPT, MineRL, CS:GO, StarCraft, Slippi, Dota 2, AoE2, and others), annotation scaffolding, and VLM episode preparation and scoring, for testing whether models ground community gaming terms in game media. Also an API ablation study: five extractor/judge pipelines across model providers on the same 50 frozen web sources, with costs from aggregate ledgers.
`Python` `computer vision` `VLM evaluation` `research design` · 139 tests

### Under development
- [provenance-mech](https://github.com/BobbY-24/provenance-mech): a mechanistic follow-up to Matlin et al. (2026) on what targeted unlearning changes inside OLMo-3-7B. The targeted LoRA adapter cuts SocialIQA accuracy by 9.8 points, and the damage traces to layers ~0–15. Methods: probes, CKA, layer knockout, and steering, run on Colab.

## Skills
**ML/LLM:** PyTorch, Hugging Face Transformers, PEFT/LoRA, CLIP, LLM and agent evaluation, interpretability (probing, activation patching, steering)
**Agents & tools:** MCP, tool calling, structured output, RAG, Gemini / OpenAI-compatible APIs, Claude Code, Codex, Cursor
**Data & infra:** Python, SQL, pandas, NumPy, Google Colab, Google Cloud, Docker, Git, GitHub Actions, Weights & Biases
