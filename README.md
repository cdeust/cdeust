# Clément Deust

AI architect. I build agent tooling and measure it: benchmarks with published losses, silent-failure hunts on real repos.

Latest: an A/B retrieval benchmark of memory stacks — [harness-comparison](https://github.com/cdeust/harness-comparison), cited in [claude-mem #3693](https://github.com/thedotmack/claude-mem/pull/3693), write-up at [ai-architect.tools/notes](https://ai-architect.tools/notes).

Open source:

- [thedotmack/claude-mem #3693](https://github.com/thedotmack/claude-mem/pull/3693): merged upstream on 2026-09-30. Observation search results are now grouped under day headers, so a match from months ago no longer reads as if it happened today. The `{ sort: false }` option of `groupByDate` keeps the relevance order. It came out of the same A/B retrieval work: in my benchmark, the largest source of wrong answers was stale stored knowledge served without any age signal.
- [DeusData/codebase-memory-mcp #1832](https://github.com/DeusData/codebase-memory-mcp/pull/1832): merged upstream on 2026-09-25, shipping with the next patch release. It adds Markdown-to-file `REFERENCES_FILE` graph edges, with focused tests, after a documentation fan-in blind spot surfaced in my A/B retrieval work.

Each repository has its own traced implementation and explanation of how it works and what it does: [Cortex](https://ai-architect.tools/notes/how-cortex-remembers) · [Cortex Viz](https://ai-architect.tools/projects/cortex-viz) · [Session Optimizer](https://ai-architect.tools/projects/session-optimizer) · [Codebase](https://ai-architect.tools/projects/codebase) · [Spec](https://ai-architect.tools/projects/spec) · [Zetetic Agents](https://ai-architect.tools/projects/zetetic).

The losses are in there too: one evaluation suite returns NOT PRODUCTION-GRADE against its own target, one commit gate can be configured off, one session banner states three wrong numbers out of four. Each of these is a problem I am working on now.

Tools: [Cortex](https://github.com/cdeust/Cortex) · [Zetetic Agents](https://github.com/cdeust/zetetic-team-subagents) · [ai-architect.tools](https://ai-architect.tools)
