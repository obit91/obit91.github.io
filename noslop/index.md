---
title: "No Slop"
description: "Send the point, not the pile."
layout: default
---

# No Slop

**Send the point, not the pile.**

Someone asks you a question. Using AI to think it through is fine. Pasting the whole machine answer back at them isn't.

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

*Be honest — you didn't read that. Nobody does.*

**The answer:**

Yes — migrate incrementally, starting with high-churn files; our refactors are already costing more than the type work will.

---

## Why it matters

A real person asked for your judgment. Not a search result. Not a balanced essay. Your answer is the part where you decide what all the context means.

**Pasting AI output isn't answering. It's skipping your part and handing them the slop.**

When you send the wall of text:

- **You make them do your work.** They have to skim 500 words to find the sentence you could have led with.
- **You didn't land anywhere — and it shows.** Their time was cheaper than yours. It's the review version of shipping an AI-written PR without reading it, then asking someone else to find the problems.
- **Your point gets weaker while your credibility takes the hit.** The useful sentence is buried, and what they remember is the chore.

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
