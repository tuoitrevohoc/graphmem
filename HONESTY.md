# Honesty Statement — Graph Hacks (WeMakeDevs × FalkorDB)

## The rule (from the organizers)

- FalkorDB must be **central** to the submitted project.
- The FalkorDB implementation must be **new code written during the hackathon
  (Oct 14–18, 2026)**. Re-submitting a pre-built project is not allowed.
- Coding assistants (AI helpers) **are** allowed.

## What this means for GraphMem

**Allowed before Oct 14 (and all that exists in this repo today):**
- Planning documents (vision, schema design, query sketches, demo outline)
- Empty repo scaffolding (folders, empty `__init__.py`, configs, checklists)
- Environment setup (Docker, FalkorDB local instance for learning the tool)

**NOT allowed before Oct 14 — and therefore absent from this repo:**
- Any Python implementation of the memory read/write API
- Any executable Cypher query code wired to FalkorDB
- Any agent logic (planner/coder), demo scripts in code form
- Copying the MemGit codebase and re-submitting it

**What will be written fresh during Oct 14–18:**
- The FalkorDB adapter (memory write/read API)
- Cypher queries executed against a live graph
- The 2-agent coordination demo
- The demo video and submission blog post

The *idea* of graph-based agent memory is prior art (from MemGit) and is
allowed. Only the implementation must be new. This skeleton exists so that
on Oct 14, building can start immediately — with a clean conscience.
