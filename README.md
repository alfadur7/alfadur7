## LLM Wiki Newsroom

**Harness engineering applied to knowledge production.** Drop articles, notes, and PDFs into a folder, run one command, and a multi-agent "newsroom" running on [Claude Code](https://www.anthropic.com/claude-code) reads them, extracts entities, concepts, and relationships, and organises everything into a cross-linked, human-readable markdown wiki — a structured, persistent alternative to RAG. Local-first, plain markdown and git.

[![Stars](https://img.shields.io/github/stars/alfadur7/llm-wiki-newsroom?style=flat&labelColor=0d1117&color=58a6ff)](https://github.com/alfadur7/llm-wiki-newsroom/stargazers)
[![License](https://img.shields.io/badge/license-MIT-58a6ff?style=flat&labelColor=0d1117)](https://github.com/alfadur7/llm-wiki-newsroom/blob/main/LICENSE)

**[Site](https://alfadur7.github.io/llm-wiki-newsroom/)** · **[Repository](https://github.com/alfadur7/llm-wiki-newsroom)** · **[The Knowledge Factory](https://alfadur7.github.io/llm-wiki-newsroom/knowledge-factory/)** · **[Browsable example wiki](https://github.com/alfadur7/llm-wiki-newsroom/wiki)** · **[한국어](https://alfadur7.github.io/llm-wiki-newsroom/ko/)**

[![The interactive knowledge graph browser — every page a node, every wikilink an edge, auto-grouped into colour-coded clusters](https://raw.githubusercontent.com/alfadur7/llm-wiki-newsroom/main/docs/knowledge-graph.png)](https://github.com/alfadur7/llm-wiki-newsroom/wiki)

### What's different

The wiki is produced by five roles modelled on a newspaper staff — reporter, columnist, desk, copy editor, editor-in-chief — but the lever isn't the head count. **The agent that writes a page is never the one that reviews it**, and the reviewer gets the finished draft and the rubric, never the writer's reasoning. Nor is every seat a model passing judgement: the desk holds the only independent LLM verdict, the copy editor is a deterministic Python script, and the rest is writing work or orchestration. The real mechanism is context isolation, not instance count.

### Four loops

| Loop | When | What it does |
|---|---|---|
| **Inner** | while drafting | the agent's own fast checks, before anything is submitted |
| **Outer** | at publication | deterministic lint first, then an independent desk review |
| **Meta** | over time | recurring defects get promoted into the authoring rules themselves |
| **Reground** | after publication | published pages come back around as input once they go stale |

The first three mirror the software-factory playbook for AI-assisted coding. The fourth exists because knowledge, unlike code, keeps decaying after you ship it — sources change, a claim's own deadline matures, or two pages quietly start contradicting each other. [The full argument is here](https://alfadur7.github.io/llm-wiki-newsroom/knowledge-factory/).

### Where it stands

New, and hedged on purpose. The repository went public on 2026-06-26 and ships a deliberately small 15-node example corpus — the debate over what "open source" means for AI — so you can read the output before installing anything. The differentiators (writer/reviewer separation, the self-evolving guideline loop) are design arguments being measured, not settled claims. The Python tooling runs locally with no external API keys; the agent itself runs on your own Claude Code.

---

*한국어: [소개](https://alfadur7.github.io/llm-wiki-newsroom/ko/) · [지식 팩토리 — 하니스 엔지니어링을 지식 생산에 적용하기](https://alfadur7.github.io/llm-wiki-newsroom/ko/knowledge-factory/) · [FAQ](https://alfadur7.github.io/llm-wiki-newsroom/ko/faq/)*

<!-- profile README -->
