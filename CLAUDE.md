# suveryn-connector-sdk

The contract, a template and a test harness for connectors to [suveryn-core](https://github.com/suveryn/suveryn-core), written by sūveryn or by third parties. Apache-2.0.

**Empty by design.** Connectors are not built yet: they are the most security-critical part of sūveryn (they are how data could leave an appliance), and the order of work puts the notary playbooks first (core's [docs/design/platform.md](https://github.com/suveryn/suveryn-core/blob/main/docs/design/platform.md)). Don't scaffold, design or add code here unless a tracker issue says the connector work has started.

Start with the private [suveryn-handbook](https://github.com/suveryn/suveryn-handbook/blob/main/context/development-context.md#start-here), its *Start here*: the design principles, the project's words, and how a change reaches `main`. Its §5.7 says what is decided about connectors (an id, a version, scopes and a licence declared by each; outbound connectors off by default, with their egress declaration shown and agreed).

## Before you start

<!-- shared: copied from suveryn-handbook/context/claude-md-shared.md; change it there, never here -->

1. **Read the handbook's [*Start here*](https://github.com/suveryn/suveryn-handbook/blob/main/context/development-context.md#start-here)** before any work: the design principles, the project's words, how a change reaches `main`. If you can't open it, stop and say so. In a long session, read it again when the conversation has been summarised.
2. **One issue, one branch, one PR.** The change has an issue in suveryn-tracker and the branch is named for it. No branch is built on an unmerged branch. A coding agent never pushes: it delivers its branch into the founder's local clone without switching that clone's branch, and only the founder pushes and merges.
3. **Before you ask for a merge**, say which design principle the change bends, if any, and why. A bent principle needs the founder's decision in the handbook before the merge.

<!-- /shared -->

## Rules

- **Copy** follows the brand's [Wording and spelling](https://github.com/suveryn/suveryn-brand/blob/main/guidelines/brand-guidelines.md#wording-and-spelling).
