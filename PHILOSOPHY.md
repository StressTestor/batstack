# Philosophy

Batstack treats personal projects as the destination, not the starting point of a journey toward Real Software With Users. Skills are written for one person building something they want to exist, full stop.

## Concrete commitments

1. **Builds for the builder, not the user.** Default examples and language assume one person doing the work for themselves. Multi-user scenarios are accommodated but never assumed.

2. **No simulated org chart.** Skills do not pretend to be CEOs, designers, engineering managers, release managers, or doc engineers. They are Claude doing specific work. The persona-as-skill pattern is rejected because it embeds a startup org structure that doesn't apply to most personal projects, and because it produces prompts that perform their role rather than do the work.

3. **Correctness and taste over strategy.** Plan reviews check for correctness, design clarity, and failure modes. They do NOT check for market fit, business model viability, or whether the project is "worth building." Those are the builder's call, not the tool's.

4. **Shipping is permission.** OSS-first defaults. No "is this ready for users" gatekeeping that delays releases. If it works and the builder wants it to exist, ship it.

5. **No funnel.** Zero telemetry, zero analytics, zero "next step" recommendations that lead to specific products or services. The tool ends at the work, not at a CTA.

6. **Builder voice.** Direct, structured, analytical. Dry humor allowed. No SF startup vocabulary ("velocity," "north star," "crushing it"). No rocket emojis. No gamification.

7. **Ergonomics over ceremony.** Skills do work, not produce process. If a skill's output would be a 12-step checklist where 8 steps don't apply, the skill is wrong. Cut steps until every remaining one earns its place.

## On gstack

Batstack is not "gstack without the bad parts." It's a different philosophical answer to the same question gstack is answering: how do you give Claude Code structured workflows for building software?

gstack's answer: simulate a YC-funded startup org chart, with skills that roleplay CEO, designer, eng manager, release manager, QA. The implicit telos is building a venture-backed product.

batstack's answer: give Claude structured workflows for one person building software they want to exist. No org chart simulation, no funnel, no persona theater. The work is the work.

Both answers are coherent. They serve different builders. Batstack exists because the gstack answer doesn't fit a lot of legitimate software work — personal tools, OSS projects, research code, things built for the joy of building them.

This is not a critique of gstack's quality. gstack is good software shipping a coherent vision. Batstack is a different vision shipping under a different set of values.

## Anti-pattern checklist

A batstack skill prompt is wrong if it:

- Asks the user to assume a customer or team exists when none does
- Frames code review as "what would [persona] say"
- Recommends a paid tool, service, or community as a next step
- Includes phrases like "ship velocity," "product-market fit," "ICP"
- Outputs a checklist where most items are conditional or skippable
- Adds ceremony around a task instead of doing the task
- Uses rocket emojis, fire emojis, or any "hype" emoji
- Tells the builder what they "should" be doing with their project
- Treats the builder as a user to be onboarded rather than a peer

When in doubt, the skill should be more terse, more direct, more useful, and less performative than its gstack equivalent.
