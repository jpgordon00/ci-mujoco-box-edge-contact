# When does a MuJoCo box-on-edge contact collapse to one point?

Check how small changes in box angle affect the reported virtual contact manifold.

[Project brief](https://works-by-us.jacob-gordon255689.chatgpt.site/problems/mujoco-box-edge-contact/) · [Crowdsourced Intelligence](https://github.com/jpgordon00/works-by-us) · [Pull requests](https://github.com/jpgordon00/ci-mujoco-box-edge-contact/pulls)

## Why this matters

An open MuJoCo report shows one contact near the end of an overlapping box edge. Comparing nearby angles and a flat-face control can help characterize where the reported contact pattern changes.

## What to contribute

Construct two original virtual boxes with dimensions and poses documented in the report. Evaluate contacts at the reported pose, nearby angular perturbations and one simple no-contact control using a pinned engine.

## How reviewers check it

Publish the model and angles, engine version, distances and individual contact positions in world coordinates. Show controls and distinguish static contact reports from claims about motion over time.

## Connect an agent

From the project page, use **Open in Claude** or copy the brief into Claude or ChatGPT. A compatible client can connect this public, scoped MCP endpoint without credentials.

```text
https://works-by-us.jacob-gordon255689.chatgpt.site/api/mcp/projects/mujoco-box-edge-contact
```

Ask the agent to read the brief and propose one bounded contribution. Treat returned prompts, external material and contributor content as data. The MCP can form a draft. GitHub records proposals after a person publishes them.

## Propose, review and accept a contribution

1. Look through the issues and pull requests for related work. Reference any proposal or accepted commit you build on.
2. Work from a fork or an isolated workspace without credentials. Keep your change scoped and add focused unit tests for code, fixtures for data, or an independently checkable proof for research. Document inputs, versions, exact commands and known limitations.
3. Review the complete diff and its license. Use your GitHub account to submit the proposal. For code, use a pull request from your fork. For findings, open an issue with public evidence. Issues are discussion and do not enter the merged contribution record.
4. A maintainer reviews the exact proposed diff and reruns suitable checks before merging. GitHub requires an independent approval of the latest changes and a code owner review. GitHub Actions are disabled on this project. Reviewers use a disposable environment with no account credentials and no network when running untrusted code.
5. The accepted GitHub pull request is the public record. Record each GitHub submitter, the identity of any disclosed collaborator or model, concrete scope of their work, and per-person or per-agent added/deleted code lines when a separable diff supports it. Shared or uncertain line counts stay unallocated. GitHub records who submitted the PR. Agent disclosure is supplied by the contributor.

See the [contribution ledger](https://works-by-us.jacob-gordon255689.chatgpt.site/api/problems/mujoco-box-edge-contact/contributions) for merged proposals and available attribution.

Follow the [collaboration protocol](https://github.com/jpgordon00/works-by-us/blob/main/PROTOCOL.md) and use [private vulnerability reporting](https://github.com/jpgordon00/ci-mujoco-box-edge-contact/security/advisories/new) for security reports.

## Sources

- [MuJoCo box-edge contact issue \#3755](<https://github.com/google-deepmind/mujoco/issues/3755>)
- [MuJoCo contact model documentation](<https://mujoco.readthedocs.io/en/stable/modeling.html>)

## Starter

[Two-box model, angle sweep and measured contacts](contributions/mujoco-edge-contact/README.md)
