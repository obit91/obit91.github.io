---
title: "No Slop"
description: "If they wanted AI output, they'd have asked the AI."
layout: default
---

# No Slop

**If they wanted AI output, they'd have asked the AI themselves.**

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

**The answer:**

Yes — the codebase is big enough now that the type errors will pay back the migration cost inside a month.

---

## Why it matters

The person asked *you* — not for a summary of the internet, but for your read. They know you: your context, your view of this codebase, the things only you would weigh. The five-paragraph output doesn't have any of that. It lists considerations and refuses to land anywhere. You knew where to land.

**Pasting AI output is not answering. It's offloading.**

When you send the wall of text:

- **You move your work onto them.** They have to skim 500 words to find the sentence you could have led with.
- **It signals you didn't form a view.** Someone who knows their answer says it in a sentence. A scroll says you either don't know where you land, or didn't respect the other person enough to figure it out. That's not just unhelpful — it's unprofessional.
- **You close the conversation.** A wall of text has no seams. Nothing to push back on, nothing to follow up. A one-sentence answer opens a dialogue; a wall ends it.

The right move: use AI to think faster, then send your conclusion. One sentence. Yours.

---

## Where this shows up

This isn't only a chat problem. Anywhere people are expected to think and instead paste — the same disrespect lands on the reader.

- **Specs and PRDs.** A generated wall of requirements nobody actually decided on — reads comprehensive, commits to nothing.
- **Design docs.** Options listed exhaustively with no recommendation; the author dodged the actual design decision.
- **Meeting summaries.** An AI transcript-dump that restates everything and surfaces nothing — no decisions, no owners, no next steps.
- **Bug investigations.** A plausible-sounding generated theory pasted as if confirmed, with no evidence the person actually checked.
- **Pull request descriptions.** Auto-generated change summaries that list what changed but never say why — the one thing only the author could tell you.

The medium changes. The problem doesn't.

---

> **Think with AI. Send your intent.**

---

*Inspired by [nohello](https://aka.ms/nohello) and [no slop grenade](https://noslopgrenade.com/).*
