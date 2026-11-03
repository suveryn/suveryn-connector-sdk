# suveryn-connector-sdk

The contract, a template and a test harness for connectors to [suveryn-core](https://github.com/suveryn/suveryn-core), written by sūveryn or by third parties. Apache-2.0.

**Empty by design.** Connectors are not built yet: they are the most security-critical part of sūveryn (they are how data could leave an appliance), and the order of work puts the notary playbooks first (core's [docs/design/platform.md](https://github.com/suveryn/suveryn-core/blob/main/docs/design/platform.md)). Don't scaffold, design or add code here unless a tracker issue says the connector work has started.

Start with the private [suveryn-handbook](https://github.com/suveryn/suveryn-handbook/blob/main/context/development-context.md#start-here), its *Start here*: the design principles, the project's words, and how a change reaches `main`. Its §5.7 says what is decided about connectors (an id, a version, scopes and a licence declared by each; outbound connectors off by default, with their egress declaration shown and agreed).

## Rules

- **One branch and PR per change.** Merge only when the founder says so. Never change repository settings, secrets or CI. A coding agent never pushes: it delivers a patch, applied in a separate worktree, as *Start here* says.
- **Copy** follows the brand's [Wording and spelling](https://github.com/suveryn/suveryn-brand/blob/main/guidelines/brand-guidelines.md#wording-and-spelling).
