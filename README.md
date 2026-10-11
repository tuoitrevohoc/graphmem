# GraphMem — Graph-Based Memory Layer for Coding Agents

**Graph Hacks entry** — WeMakeDevs × FalkorDB · Oct 14–18, 2026 · Online
Track: **Agent Memory and Coordination** (primary); optionally *Agents That Act on Connected Data*

## Vision

Coding agents forget. When agents coordinate through chat logs or flat files,
context gets lost and decisions can't be traced. GraphMem is a **shared memory
layer backed by FalkorDB** that every agent in a team reads from and writes to:

- **Nodes** — `Fact` (known truths), `Decision` (choices made), `Task` (work in progress), `Agent`
- **Edges** — `decided_by`, `depends_on`, `supersedes`, `relates_to`, `observed_at`
- An agent records a memory → another agent queries it in Cypher
  ("what did the API agent decide about auth?") → the graph is traversed to
  **explain the path behind an answer**.
- Old facts fade via TTL/decay; pending tasks are first-class nodes
  (an idea inherited from MemGit, Khiem's earlier agent-memory project).

## Demo plan (weekend of Oct 14–18)

Two agents — a **planner** and a **coder** — build one small feature together,
coordinating **only through the shared graph** (no direct chat between them).
At the end of the demo, a single Cypher query redraws the full path from
*requirement → decision → code*, showing the judges the decision trace.

See [demo/demo-outline.md](demo/demo-outline.md) for the scene-by-scene outline.

## ⚠️ HONESTY NOTICE (contest rule)

Per Graph Hacks rules, **FalkorDB must be central to the project, and the
FalkorDB implementation must be new code written during the hackathon
(Oct 14–18, 2026).**

**This repository skeleton deliberately contains zero implementation code.**
Only planning docs, configs, empty placeholders, and checklists exist here.
All `src/`, `tests/`, and demo code will be written fresh starting Oct 14.
See [HONESTY.md](HONESTY.md) for the full rule statement and
[CHECKLIST.md](CHECKLIST.md) for the day-by-day build plan.
