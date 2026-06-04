---
title: "No Slop"
description: "They asked you. A relay isn't an answer."
layout: default
---

# No Slop

**They asked you. A relay isn't an answer.**

Someone asks you a question. You run it through an AI — that's fine, that's what the tool is for. Then you paste the result into the chat and hit send. That's the mistake.

---

*Question: should we migrate this project to TypeScript?*

**The output:**

> Migrating a JavaScript project to TypeScript is a significant architectural decision with real trade-offs that depend on multiple factors including team size, project maturity, timeline constraints, and long-term maintenance goals. TypeScript is a statically typed superset of JavaScript developed by Microsoft that compiles down to plain JavaScript and is fully compatible with existing JS ecosystems.
>
> The primary benefits of TypeScript include compile-time type checking, improved IDE support (autocomplete, inline documentation, refactoring tools), and reduced likelihood of certain classes of runtime errors. For larger codebases or teams with multiple contributors, these benefits tend to compound over time as the surface area of change grows.
>
> That said, migration carries real cost. Depending on codebase size, a full migration can take anywhere from days to several months. The team needs to be comfortable with TypeScript syntax and type system concepts — generics, union types, utility types, type narrowing — which have a non-trivial learning curve. Incremental adoption (using `allowJs` and migrating file by file) can reduce the risk, but also extends the period of mixed-language inconsistency.
>
> Build tooling also becomes more complex. You'll need to configure `tsconfig.json`, update bundler settings, and potentially adjust lint rules. Third-party libraries may have incomplete or outdated type definitions, requiring `@types/` packages or custom `d.ts` declarations.
>
> In summary: TypeScript tends to pay for itself in projects over a certain size and complexity threshold, especially those expected to grow or be touched by multiple developers over time. For smaller, stable, or short-lived projects the overhead may outweigh the benefit. Evaluate based on your team's familiarity and the expected lifespan of the codebase.

*You didn't read that before you hit send. If even you skipped it — nobody will.*

**The answer:**

Yes — the codebase is big enough now that the type errors will pay back the migration cost inside a month.

---

## Why it matters

There's a real person talking to you. They already know what you know and what you don't — that's why they came to you. They're not asking you to send them how the internet works, or a list of considerations they could have generated themselves. They want to know what *you* think.

**Pasting AI output is not answering. It's skipping your part and handing them the slop.**

When you send the wall of text:

- **You make them do your work.** They have to skim 500 words to find the sentence you could have led with.
- **It signals you didn't form a view — and it doesn't respect their time.** Someone who knows the answer says it in a sentence. A scroll says you didn't bother. That's unprofessional. It's like letting AI write your PR, skipping the review, and shipping it — except now it's them reviewing your slop.
- **They'll lose your point — and lose respect for you.** Your actual answer is buried in the wall. What they remember isn't your insight — it's the effort it cost them to look for it.

The right move: use AI to think faster, then send your conclusion. One sentence. Yours.

---

## Where this shows up

This isn't only a chat problem. Anywhere people are expected to think and instead paste — the same disrespect lands on the reader.

- **Specs and PRDs.** Generated bulk can fill pages without any of the decisions those pages are supposed to capture.
- **Design docs.** Easy to mistake output for analysis — a lot of options listed, little judgment applied.
- **Bug investigations.** A natural place for generated plausibility to stand in for actual investigation.

The medium changes. The problem doesn't.

---

> **If they need AI to decode what you sent, you didn't answer. You assigned homework.**

---

*Inspired by [nohello](https://aka.ms/nohello).*
