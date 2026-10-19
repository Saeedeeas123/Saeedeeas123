<div align="center">

# Saeed

**Entrepreneur · geek · AI obsessive**

Building offline-first Android software and on-device AI — from scratch, one module at a time.

[Site](https://saeedeeas123.github.io/ExploreZone/) · [Articles](https://saeedeeas123.github.io/ExploreZone/articles.html) · [Work](https://saeedeeas123.github.io/ExploreZone/work.html) · [Email](mailto:saeedatfx@gmail.com)

</div>

---

### About

I'm Saeed, an entrepreneur from Iran. I work with intelligent agents the way other people work with a
team: I evaluate them, compare them, and put them to work writing, building and shipping real software.
I set the architecture and make the decisions — they do the typing.

I write about what I learn. The first piece explains [what an LLM actually is](https://saeedeeas123.github.io/ExploreZone/posts/llm-intro.html) —
seven stages from rule-based software to agents, with seven working interactive tools that show each
stage rather than describing it. It also exists in Persian on [explorezone.ir](https://explorezone.ir/).

---

### The main project: Ideasmo

> **A tool for idea makers.**

[**Ideasmo**](https://github.com/Saeedeeas123/ideasmo) is what I'm working on. Capture an idea, give it
structure, keep it in one place — a touch-first **board** of node cards joined by **typed relations**.

Most note apps hand you a list, and a list has exactly one dimension: order. Ideas do not live in one
dimension. They depend on each other, contradict each other, cause each other, and arrive in clusters.
So the relation is the first-class object here: 7 families and 42 types — "depends on", "is a",
"contradicts", "causes" — each with its own line style, arrow mode and colour role, editable exactly
where you find it.

**Where it is now:** v0.17.0 — a complete, usable single-user tool. The board, the typed relations, a
private file store with shelves and search, notes and images and files on any node, multi-select, a
read-only view mode, and a durable log with an in-app viewer.

**Where it is going:** next is **Group** (waiting on one design answer — a frame that holds the nodes,
or a merge of them), **Schema** (a per-branch direction stored on the node), and an undo that survives a
session. After that: the Z axis, a force-directed pass in Arrange, an interactive minimap, and visual
verification tooling.

The full roadmap, and the honest limits, are on the [project page](https://github.com/Saeedeeas123/ideasmo#roadmap).

Android · Kotlin · Jetpack Compose M3 · **offline** — no account, no cloud, no network permission.

---

### What I'm building

A stack of **standalone Android modules**. Each one is written as a module rather than an app feature,
so the next app can pick it up without re-debugging it.

| Module | What it does |
| --- | --- |
| [**core-llamacpp**](https://github.com/Saeedeeas123/llamachat) | Runs GGUF models fully on-device through llama.cpp — CPU only, arm64-v8a, with the ARM dot-product kernels enabled in the shipped build. |
| [**core-litertlm**](https://github.com/Saeedeeas123/core-litertlm) | Safe, app-agnostic loader for Google's LiteRT-LM (`.litertlm`) models: it validates the file's magic header before the native layer ever sees it, and never runs on the main thread. |
| [**core-llm**](https://github.com/Saeedeeas123/minikeys) | An OpenAI-compatible LLM client for Android with an API-key vault backed by the Android Keystore. Zero third-party dependencies. |
| [**Laya**](https://github.com/Saeedeeas123/laya-module) | A decision engine as a reusable Android module — choice / score / noul — with its tokenizer, prompt builder and ONNX runtime inside the module. |

A module's repository is the repository of the app that proved it: `core-llamacpp` lives in the LlamaChat
repository and `core-llm` lives in the MiniKeys repository, because that is where they were built and
tested. Splitting them out would create a second copy of the same code, which is how modules drift apart.

---

### Built on a phone

There is no laptop and no Android Studio in this workflow. Every app is written, compiled, installed and
tested **on the device itself** — Android with a Linux container running on the same phone. It is a hard
way to work, and it is exactly why these modules exist: when the build machine fits in your pocket, every
dependency has to earn its place.

It is also why every project here carries a durable log file and an in-app log viewer. When you have no
PC, the app's own log is the only diagnostic channel you have.

---

### Stack

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![llama.cpp](https://img.shields.io/badge/llama.cpp-on--device-000000)
![LiteRT-LM](https://img.shields.io/badge/LiteRT--LM-on--device-4285F4)

---

### Where this is going

Toward offline software that genuinely works on a phone: a device that understands its own screen,
decides what to do next, and does it — with the model, the voice and the decision logic all running
locally, with no network and no app-specific scripts.

The products of that are the ones above. Ideasmo is the one I'm building now.

---

### Find me

- **Site** — [English edition](https://saeedeeas123.github.io/ExploreZone/) · [Persian edition](https://explorezone.ir/)
- **Articles** — [what an LLM is, with seven interactive tools](https://saeedeeas123.github.io/ExploreZone/posts/llm-intro.html)
- **Email** — [saeedatfx@gmail.com](mailto:saeedatfx@gmail.com)

<sub>Private by default. Public when it's stable.</sub>
