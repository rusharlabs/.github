# Rushar Labs

Applied research and engineering in AI, published as open-source software. The work here is
tooling for coding-agent work in which a claim is accepted only with the command that proves it.

## House Party Protocol

**Agent teams under evidence: only what they prove counts as done.**

House Party Protocol (HPP) is a local-first harness for coding-agent teams on Claude Code and
Codex CLI. It is not the orchestrator: whatever hands out the work decides who works on what, and
HPP decides what counts as done. Waves and lanes split the work, a verdict from the builder's own
lane or model family is refused, nothing is verified without recorded evidence, and its refusals
exit non-zero, so a script can gate on them. It is a Python package with no runtime dependencies,
released under the MIT license; the `hpp` package itself calls no model and runs nothing in the
background, and each module declares in the manifest what it may do. The same repository is a
plugin marketplace for Claude Code and for Codex CLI.

- [Repository](https://github.com/rusharlabs/house-party-protocol) — source, issues and releases
- [Manual and catalogue](https://rusharlabs.github.io/house-party-protocol/) — the manual, the catalogue and the design system, rendered
- [Discussions](https://github.com/rusharlabs/house-party-protocol/discussions) — questions and design conversations, in English or Portuguese
- [Latest release](https://github.com/rusharlabs/house-party-protocol/releases/latest) — with `SHA256SUMS` and build provenance

```bash
pip install house-party-protocol
hpp doctor
```

## Contributing and asking

- A question: open it in [Q&A](https://github.com/rusharlabs/house-party-protocol/discussions/categories/q-a), pasting the command you ran and its output. An early idea or a design question goes to [Ideas](https://github.com/rusharlabs/house-party-protocol/discussions/categories/ideas).
- A command that behaves differently from its documentation: open a [problem report](https://github.com/rusharlabs/house-party-protocol/issues/new?template=problem.yml).
- A change: read [CONTRIBUTING.md](https://github.com/rusharlabs/house-party-protocol/blob/main/CONTRIBUTING.md) first. A bug fix ships with the test that failed before it.
- A vulnerability: do not open a public issue; use [private vulnerability reporting](https://github.com/rusharlabs/house-party-protocol/security/advisories/new), as described in [SECURITY.md](https://github.com/rusharlabs/house-party-protocol/blob/main/SECURITY.md).
