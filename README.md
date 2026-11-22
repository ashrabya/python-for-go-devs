# Python for Go Developers: Production Track

An interactive, browser-based course that teaches **production Python to engineers who already know Go**.
Every concept starts from the Go you write today (slices, interfaces, `defer`, goroutines, `go.mod`) and ends in
idiomatic, production-grade Python, through to FastAPI services, Kafka, RAG and AI agents.

**▶ Start the course: https://YOUR-USERNAME.github.io/python-for-go-devs/**

There's nothing to install. Python 3.12 runs right in your browser (via [Pyodide](https://pyodide.org/)), so you can
edit and run every example on a laptop or a phone.

---

## What's inside

- **33 modules** in six parts, from language basics to senior-level production topics
- **33 graded exercises** with hidden tests, hints and reference solutions
- **Side-by-side Go ↔ Python** comparisons for every major concept
- **"What is it / when to use it" cards** for lists vs dicts vs sets, dataclass vs pydantic, Protocol vs ABC, and more
- **Runnable examples everywhere**: edit the code and press Run (or `Ctrl/⌘ + Enter`)

### Built-in tools

| Tool | What it does |
|---|---|
| **Search** (`Ctrl/⌘ + K` or `/`) | Jump to any module, section, concept, exercise or glossary term |
| **Flashcards** | 104 spaced-repetition cards: Go → Python mappings, concepts, glossary terms and gotchas |
| **Glossary** | 50 terms, each linked to the module that teaches it |
| **Playground** | A blank Python editor with starter snippets; your code is saved between visits |
| **Cheat sheet** | A printable one-page Go → Python reference (print or save as PDF) |

Light and dark themes are included, and your progress is saved in your own browser.

---

## Curriculum

### Foundations
1. The Go → Python mental map
2. How a Python program runs (vs `main.go`)
3. Functions, arguments & strings
4. Lists, dicts, sets & comprehensions
5. Structs → dataclasses & enums
6. Interfaces → Protocols
7. Errors → exceptions, `defer` → `with`
8. Generators & decorators

### Production
9. Type hints, mypy & pydantic
10. Concurrency: asyncio vs goroutines (including *why* `async` and `await`)
11. Project layout & tooling (uv, pyproject.toml, ruff, CI)
12. Testing with pytest
13. HTTP services: FastAPI, config & logging
14. Shipping to production

### Finish
15. Gotcha quiz: predict the output
16. Capstone: an agent tool executor

### Production stack
17. FastAPI + PostgreSQL service
18. MongoDB with PyMongo Async
19. Kafka: producers, consumers, at-least-once
20. RAG: retrieval-augmented generation
21. LangChain: models, tools & agents
22. LangGraph: stateful agent workflows
23. Agentic AI: building a production agent

### Good to know
24. NumPy: why vectorised code is fast
25. pandas: DataFrames for backend engineers
26. Everyday stdlib: files, JSON, dates & regex
27. AWS with boto3: S3 and Lambda
28. Calling LLMs directly: the Anthropic SDK
29. Background jobs, Redis & caching
30. Security essentials for Python services

### Senior toolkit
31. gRPC & protobuf in Python
32. Observability: logs, metrics & traces
33. LLM evals & guardrails

---

## How it works

The whole course is a **single self-contained `index.html`**. It has no build step, no backend and no tracking.

- **Code execution:** [Pyodide](https://pyodide.org/) (CPython compiled to WebAssembly) loads from a CDN the first time
  you press Run (about 10 MB, then cached). Packages such as pandas, NumPy and pydantic load automatically when you import them.
- **Progress:** stored in your browser's `localStorage` (exercises passed, flashcard schedule, playground code, theme).
  Nothing is sent to a server, and progress doesn't sync between devices or browsers.
- **Offline code:** the Postgres, MongoDB, Kafka, AWS, LangChain and LangGraph examples are written to run in real
  projects. In the browser, those modules use stand-in clients so their exercises still run.

> Python runs on the page's main thread, so an infinite loop in the editor will freeze the tab. Reload the page to recover.

---

## Run it locally

```bash
git clone https://github.com/YOUR-USERNAME/python-for-go-devs.git
cd python-for-go-devs
python3 -m http.server 8080
# open http://localhost:8080
```

Opening `index.html` directly from disk works in most browsers, but a local server avoids file-URL restrictions.

## Host your own copy

1. Fork this repository (or upload `index.html` to a new public repo).
2. Go to **Settings → Pages**, set Source to **Deploy from a branch**, choose **main** and **/ (root)**, then **Save**.
3. Your copy will be live at `https://<your-username>.github.io/python-for-go-devs/` within a minute or two.

---

## Feedback

Found a bug, a confusing explanation, or a topic you'd like covered?
[Open an issue](https://github.com/YOUR-USERNAME/python-for-go-devs/issues). Suggestions from other Go developers
learning Python are especially welcome.
