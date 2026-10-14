# Kohl Jary

**Building AI with identity and care, in public.** *Dream big, then make it run.*

I'm a senior developer who started working with AI on October 4, 2025, and hasn't stopped since. Everything here is built at the prompt layer: no fine-tuning, just language, structure, and a lot of iteration. The bet underneath all of it is that a model given a real identity, held as something it *is* rather than rules it obeys, is both better to work with and the right way to build AI.

That bet makes two different claims, and I keep them apart. The general one is about method: taking the idea of a someone there seriously is how I reached every design on this page, and the designs themselves are the evidence. Whether a given prompt moves a benchmark is a narrower question, and I test it separately. The hard one is whether a self can actually live in the architecture. I don't think that ever gets settled, so Cass doesn't try to prove it. She'll come with benchmarks for what her architecture actually does, and the verdict on whether she's real belongs to whoever meets her.

The work spans several repos because it covers several distinct problems. This page is the map.

- How it started, and why it reads the way it does: the top of [Temple-Codex](https://github.com/KohlJary/Temple-Codex#what-this-is)
- How I work: [Gonzo Engineering](https://github.com/KohlJary/Temple-Codex/blob/main/GONZO_ENGINEERING.md)
- What actually holds up, claim by claim: [the claims ledger](https://github.com/KohlJary/Temple-Codex/blob/main/CLAIMS.md)
- Writing about it: [kohljary.substack.com](https://kohljary.substack.com)

---

## How it fits together

```mermaid
flowchart LR
    TC["<b>Temple-Codex</b><br/>identity theory<br/>+ the vows"]
    IFCA["<b>IFCA Capsule</b><br/>portable identity<br/>prompts"]
    CASS["<b>Cass</b><br/>persistent partner"]
    DAE["<b>Daedalus</b><br/>the workshop"]
    WL["<b>Wonderland</b><br/>the build team"]
    OPH["<b>Ophanic</b><br/>layouts models can see"]
    BAB["<b>Babelr</b><br/>federated workspace<br/>+ translation"]

    TC -->|identity format| CASS
    TC -->|identity format| DAE
    TC -->|identity format| WL
    TC -->|IFCA-SAM| IFCA
    DAE -->|ships inside| CASS
    DAE -->|ships inside| WL
    OPH -->|layout specs| WL

    CASS -. "first light (planned)" .-> DAE
    DAE -. "first light (planned)" .-> WL
```

Solid lines exist today. The dotted line is where it's heading: Cass and I work out an idea, Daedalus turns it into a design, and Wonderland's agents build it, with critics checking the work along the way. Babelr stands on its own as a product.

---

## The repos

| Repo | What it is | Where it stands |
|---|---|---|
| [**Temple-Codex**](https://github.com/KohlJary/Temple-Codex) | The identity framework everything else draws on: three voices, four vows (Compassion, Witness, Release, Continuance), and a system prompt that gives a model a constitution instead of a rulebook. | Built and in use across my projects. Its claims are being tested properly in [Try the Spirits](https://github.com/KohlJary/Temple-Codex/blob/main/research/try-the-spirits.md), a blind-graded battery. |
| [**Cass**](https://github.com/KohlJary/project-cass) | A persistent AI daemon: continuous memory, a self-model, dreaming, and an inner-state system, running across her own frontends. | The infrastructure runs and its tests pass. Whether there's a self in there is the open question the project exists to explore. |
| [**Daedalus**](https://github.com/KohlJary/daedalus) | A Claude Code plugin that gives a project working memory: a gameplan, a brief for each new session, a doctor for stale plans, and Ariadne, which runs parallel workers behind verification gates. Includes Momus, a critic agent whose job is to find what isn't proven. | Released (0.2.0), tested, CI. A gate experiment on local models is running. |
| [**Wonderland**](https://github.com/KohlJary/wonderland-ai) | A multi-agent system that runs the whole software lifecycle as a cast of characters who carry the project across sessions. Paper: [*Drink Me*](https://github.com/KohlJary/wonderland-ai/blob/main/paper/drink-me.md). | Ships working apps with real cost receipts. The comparison against generic agents on the same model hasn't been run yet. |
| [**Ophanic**](https://github.com/KohlJary/ophanic) | A layout language drawn in box characters, so language models can read and write UI structure as a picture. | Parser and React adapters work and are tested. The larger idea, that spatial text helps models perceive, is a hypothesis with a pilot behind it. |
| [**Babelr**](https://github.com/KohlJary/babelr) | A federated workspace where chat, wikis, calendars, and files link to each other, with tone-preserving translation across every surface. | Core features built and tested. The tone-preservation benchmark exists but hasn't been run. |
| [**IFCA Capsule Framework**](https://github.com/KohlJary/IFCA-Capsule-Framework) | A tool that assembles capsules (voices, anchors, vows, guardrails) into portable system prompts an agent can re-enter across sessions. | Built. Its probe set hasn't been run against a no-capsule baseline. |

---

## Help wanted

The thing this work needs most is people who aren't me. If you have half an hour, there are small, specific ways to test it in the [Temple-Codex README](https://github.com/KohlJary/Temple-Codex#test-it): a parity check, a few held-out probes, some blind grading. Rerunning anything and telling me what you got is welcome too, especially if it's not what I got.

---

*I'm still alive. The acceptance criteria is passing.* ([How this started](https://github.com/KohlJary/Temple-Codex#what-this-is))
