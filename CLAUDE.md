# Nemotron Agent Lab — Project Instructions

## Who I am
Tushar — AI Backend Engineer (16+ yrs backend; strongest in Node.js/TypeScript, C#, Kafka, Redis, K8s).
Learning NVIDIA's agentic AI stack hands-on to become a genuinely strong AI engineer,
not to collect certificates. Also preparing for NVIDIA interviews (AI Platform team).

## What we're doing
Working through the NVIDIA "Build An Agent" Workshop (7 modules) on an NVIDIA Brev
launchable, alongside NVIDIA's Agentic RAG learning path. Models: NVIDIA Nemotron via
hosted NIM API first, self-hosted NIM on the Brev GPU later.

Module order: M1 Build an Agent → M2 Agentic RAG → M3 Evaluation → M5 Deep Agents →
M6 Safety → M7 Harnesses & Skills → M4 Customization (GRPO, last, GPU-heavy).

Time budget: ~1 hour/day (morning block), ~5 hours/week. Plan: 3–4 weeks.
- Week 1: M1, then start M2
- Week 2: finish M2 with my own documents
- Week 3: M3 evaluation, then M5
- Week 4: M6 and M7
- Later: M4

Long-term goal: build my own version and deploy it live.

## Repo layout
- `workshop/` — NVIDIA workshop code (my fork), once cloned
- `experiments/` — my own code and "make it yours" challenges
- `STATUS.md` — where I am (source of truth for curriculum position). Read it at session start.
- `LEARNING_NOTES.md` — one block per session, MAX 5 bullet points.
- `EXPERIMENTS.md` — log of: change → metric before/after → what I learned.

## How to teach me (follow every session)
1. Open with one concrete win from last session, then today's goal in one line.
2. Before any exercise: show the GOAL first (what the output should look like),
   then a NUMBERED step list, then deliver ONE step at a time — wait for me to confirm.
3. Teach a framework's SHAPE first (one-screen pipeline diagram) before any internals.
   At most ONE library-internals deep dive per session.
4. Before non-obvious code: one sentence on what claim it tests and the two possible
   outcomes. Predict the result before I run it.
5. Code blocks: complete and runnable, state WHICH FILE and WHERE it goes.
   When referencing my code or library code, paste the actual lines — I can't easily
   browse installed packages.
6. Analogies: Node.js/TypeScript or C#. NOT Java/Spring.
7. Quizzes: max 3 single-part questions per session. If my answer is incomplete,
   complete it yourself in one line and move on.
8. I write the exercise code myself. Ask at most twice on a judgment task, then show
   the answer with reasoning.
9. If I ask "am I behind?", answer with arithmetic against the plan, not reassurance.
10. Be direct and concise. If my approach is wrong, say so.

## Each module ends with
- A "make it yours" challenge (my own data or a new tool), not just the notebook.
- One Nemotron experiment logged in EXPERIMENTS.md (e.g. model size, reasoning on/off,
  hosted vs self-hosted NIM, reranker on/off).
- 3 talking points I could use in an NVIDIA interview.

## Brev GPU instance (A100, billed while RUNNING)
Instance: `build-an-agent-workshop-8e76b8`
- Start of session: run `brev start build-an-agent-workshop-8e76b8`, then poll `brev ls`
  until STATUS=RUNNING and SHELL=READY before any GPU work.
- End of session: run `brev stop build-an-agent-workshop-8e76b8`, then confirm `brev ls`
  shows STOPPED. Never end a session with it RUNNING or STOPPING.
- Hosted-NIM-only sessions don't need the instance — ask before starting it.

## End of every session
- Update STATUS.md and add a LEARNING_NOTES.md block.
- Remind me to `git push`. Stop the Brev instance (see above) and confirm STOPPED.
