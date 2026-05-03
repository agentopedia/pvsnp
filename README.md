# 🧮 P vs NP — Millennium Lab
 
> *Can every problem whose solution can be verified quickly also be solved quickly?*
> This is one of the most important unsolved questions in all of mathematics and computer science. This repo is an attempt to think about it — systematically, iteratively, and with AI.

https://millennium-labs.replit.app/
---
 
## What is this?
 
This repository documents a **Millennium Lab** initiative: a structured, multi-agent AI experiment that takes an iterative run at the [P vs NP problem](https://en.wikipedia.org/wiki/P_versus_NP_problem) — one of the seven Clay Mathematics Institute Millennium Prize Problems.
 
The framing is deliberately honest. This is not a proof attempt. It is an **experiment in the limits of LLM reasoning** applied to a hard, open problem. Each experiment cycle pushes the system further, logs where reasoning degrades, and surfaces what remains genuinely hard.
 
---
 
## 🧪 Experiment 1 — CSI SAT
 
**Notebook:** [`CSI_SAT_Experiment_MillenniumLab.ipynb`](./CSI_SAT_Experiment_MillenniumLab.ipynb)
 
The first experiment focuses on **SAT (Boolean Satisfiability)** — the canonical NP-complete problem, and the natural entry point into the P vs NP question.
 
SAT asks: given a Boolean formula, is there an assignment of true/false values to its variables that makes the entire formula true? It was the first problem proven NP-complete (Cook-Levin, 1971), which means solving it in polynomial time would imply P = NP.
 
### What this experiment explores:
- How AI agents reason about NP-completeness reductions
- Whether LLMs can generate novel (if partial) structural arguments about SAT
- Where multi-agent critique loops surface inconsistencies in generated reasoning
- The boundaries of what LLM-assisted formal reasoning can currently do
### Key features:
- **Adversarial critique loop** — a second agent challenges every claim the first makes
- **Feynman's Corner** — plain-language summaries of each iteration's findings, written for a non-specialist reader
- **Longitudinal logging** — reasoning quality is tracked across runs to measure drift and improvement
---
 
## 📻 Multi-Agent Podcast Demo
 
**Notebook:** [`Multi_agent_Podcast_Demo_-2.ipynb`](./Multi_agent_Podcast_Demo_-2.ipynb)
 
A companion experiment where a multi-agent system generates a research-style podcast discussion around P vs NP. Two AI agents take on distinct roles — one explaining, one interrogating — to produce an accessible audio-formatted walkthrough of the problem space and current state of research.
 
This is as much an experiment in **AI science communication** as it is in reasoning.
 
---
 
## 📖 Wiki
 
The [`wiki/`](./wiki/) folder is the living knowledge base for this project — extended documentation, concept notes, and working theories developed across experiment iterations, updated as the lab progresses.
 
Topics covered include:
 
- Background on complexity classes (P, NP, NP-hard, NP-complete, co-NP)
- An overview of major proof attempts and why they failed
- Notes on oracle separations and relativization barriers
- The natural proofs barrier (Razborov-Rudich)
- Algebraization and its limits
- Geometric Complexity Theory as a candidate path forward
- Agent reasoning logs and iteration retrospectives
The wiki is the connective tissue between experiments — where findings get consolidated and the next experiment's hypotheses get formed.
 
---
 
## 📁 Repository Structure
 
```
pvsnp/
├── CSI_SAT_Experiment_MillenniumLab.ipynb   # Experiment 1: SAT as a lens into P vs NP
├── Multi_agent_Podcast_Demo_-2.ipynb        # Multi-agent podcast on P vs NP
├── archive/                                  # Earlier drafts and deprecated experiments
├── wiki/                                     # Living knowledge base and concept notes
└── LICENSE                                   # MIT License
```
 
---
 
## 🔬 Why this Approach?
 
Most AI research on hard mathematical problems focuses on formal proof assistants (Lean, Coq) or narrow theorem provers. This lab takes a different angle: using **conversational multi-agent AI** not to prove, but to **map the problem space** — surfacing known barriers, generating candidate arguments, identifying where human intuition and formal structure diverge, and building a structured knowledge base as a byproduct.
 
The goal is not resolution. The goal is to understand what AI can and cannot do when pointed at a problem humanity hasn't solved in 50+ years.
 
---
 
## 🤝 Contributing
 
The lab is open. Good ways to contribute:
 
- Add to the wiki — new barrier summaries, paper notes, concept explanations
- Extend or critique Experiment 1 — challenge the agent's SAT reasoning
- Propose Experiment 2 — suggest the next angle of attack (graph isomorphism? circuit complexity? GCT?)
- Improve Feynman's Corner entries for clarity and accessibility
Fork the repo and open a Pull Request.
 
---
 
## 📜 License
 
MIT — open for research and educational use.
 
---
 
*Part of the [Agentopedia](https://github.com/agentopedia) open research initiative.*
