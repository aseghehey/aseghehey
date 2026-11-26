# Emanuel Aseghehey

**Distributed systems · cloud infrastructure · developer tooling**

I'm a software engineer at AWS in Austin, working on the infrastructure behind Amazon OpenSearch Service. Most of my days go to control-plane work: capacity and auto-scaling, workflows that have to recover cleanly when something fails halfway, and the tests and tooling that make that kind of change safe to ship.

Outside of that, I contribute to an open-source AWS emulator and build small tools for working alongside coding agents.

## Floci — local AWS emulation

[Floci](https://github.com/floci-io/floci) is an open-source emulator for AWS services. I contribute through [Andre Kurait's fork](https://github.com/AndreKurait/floci), where I have [over 50 merged pull requests](https://github.com/AndreKurait/floci/pulls?q=is%3Apr+is%3Amerged+author%3Aaseghehey). The aim is that code written against real AWS behaves the same way locally.

- **EC2 networking.** IPv6 for dual-stack VPCs and guests ([#1149](https://github.com/AndreKurait/floci/pull/1149), [#1148](https://github.com/AndreKurait/floci/pull/1148)), attaching network interfaces to running instances ([#1169](https://github.com/AndreKurait/floci/pull/1169)), and VPC endpoint services ([#1152](https://github.com/AndreKurait/floci/pull/1152)).
- **IAM and KMS authorization.** Evaluating `aws:ResourceTag` against each resource's stored tags ([#1178](https://github.com/AndreKurait/floci/pull/1178)), verifying SigV4A signatures ([#1133](https://github.com/AndreKurait/floci/pull/1133)), and cross-account key use through grants ([#1154](https://github.com/AndreKurait/floci/pull/1154)).
- **Service coverage.** SSM Session Manager sessions with a data-channel relay ([#1160](https://github.com/AndreKurait/floci/pull/1160)), ACM Private CA subordinate CAs ([#1144](https://github.com/AndreKurait/floci/pull/1144)), and Smithy RPC v2 CBOR for services that support it ([#1253](https://github.com/AndreKurait/floci/pull/1253)).

## Agent tooling

- **[encontra](https://github.com/aseghehey/encontra)** — a Rust CLI for full-text search over Claude Code session logs. It indexes incrementally with Tantivy, returns JSON, and can page or follow multi-hundred-MB logs by byte offset, locally or over SSH.
- **[sheepy](https://github.com/aseghehey/sheepy)** — a Tauri app that shows the Claude Code sessions running in [Herdr](https://herdr.dev) terminals as live chats, on this machine or others, and lets you reply to them.
- **[herdr-chat](https://github.com/aseghehey/herdr-chat)** — a chat window for Herdr that sits over Claude Code and Codex agents, with the terminal one click away.

## Other

- Added vector search parameters to [OpenSearch Benchmark workloads](https://github.com/opensearch-project/opensearch-benchmark-workloads/pull/334).
- Older projects from school and side work: [ratio-bot](https://github.com/aseghehey/ratio-bot), [firm-dbms](https://github.com/aseghehey/firm-dbms), [page-replacement-algorithms](https://github.com/aseghehey/page-replacement-algorithms).

[LinkedIn](https://www.linkedin.com/in/aseghehey) · [Buy me a coffee](https://www.buymeacoffee.com/emanuelase)
