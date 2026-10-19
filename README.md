<div align="center">

# Saeed

**Entrepreneur · geek · AI obsessive**

Building offline-first Android agents and on-device AI — from scratch, one module at a time.

[Portfolio](https://saeedeeas123.github.io/ExploreZone/) · [Work](https://saeedeeas123.github.io/ExploreZone/work.html) · [Repositories](https://github.com/Saeedeeas123?tab=repositories) · [Email](mailto:saeedatfx@gmail.com)

</div>

---

### About

I'm Saeed, an entrepreneur from Iran. I work with intelligent agents the way other people work with a
team: I evaluate them, compare them, and put them to work writing, building and shipping real software.
I set the architecture and make the decisions — they do the typing.

### What I'm building

A stack of **standalone Android modules**. Each one is written as a module rather than an app feature, so
the next app can pick it up without re-debugging it.

| Module | What it does |
| --- | --- |
| **core-llamacpp** | Runs GGUF models fully on-device through llama.cpp — CPU only, arm64-v8a, with the ARM dot-product kernels enabled in the shipped build. |
| **core-litertlm** | Safe, app-agnostic loader for Google's LiteRT-LM (`.litertlm`) models: it validates the file's magic header before the native layer ever sees it, and never runs on the main thread. |
| **core-llm** | An OpenAI-compatible LLM client for Android with an API-key vault backed by the Android Keystore. Zero third-party dependencies. |
| **minikeys-keyboard** | A modular Android keyboard (IME): the input method, the settings model and a canvas-drawn keyboard view. |
| **stickkeys-edge-keys** | Vertical key strips pinned to both screen edges — tap a key and the sticker, emoji or GIF you picked lands on the clipboard. |
| **minikeys-shortcut** | Always-on edge keys that act on the app in front of you: type into its focused field, send a real key combination, or press that screen's own buttons. |
| **Cosmo** | An offline Android agent: universal navigation and job primitives over the accessibility tree, with no app-specific automation scripts. |

These are developed privately and published once they are stable. The [work page](https://saeedeeas123.github.io/ExploreZone/work.html) is the always-current list.

### Built on a phone

There is no laptop and no Android Studio in this workflow. Every app is written, compiled, installed and
tested **on the device itself** — Android with a Linux container running on the same phone. It is a hard
way to work, and it is exactly why these modules exist: when the build machine fits in your pocket, every
dependency has to earn its place.

### Stack

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![llama.cpp](https://img.shields.io/badge/llama.cpp-on--device-000000)
![LiteRT-LM](https://img.shields.io/badge/LiteRT--LM-on--device-4285F4)

### Where this is going

Toward offline agents that genuinely work on a phone: a device that can read its own screen, decide what
to do next, and then do it — with the model, the voice and the decision logic all running locally, with
no network and no app-specific scripts.

Next: publish the module stack, keep the agent engine app-agnostic, and add offline voice input as a
drop-in component.

### Find me

[Portfolio & lab notebook](https://saeedeeas123.github.io/ExploreZone/) · [Email](mailto:saeedatfx@gmail.com)

<sub>Private by default. Public when it's stable.</sub>
