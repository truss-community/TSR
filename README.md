# Truss Standard Requests (TSRs)

This repository contains **Truss Standard Requests (TSRs)** — formal design documents for proposing, discussing, and adopting changes to the Truss programming language, its standard library, tooling, and governance.

## What is a TSR?

A TSR (Truss Standard Request) is the primary mechanism for making significant changes to Truss. Each TSR is a design document that follows a structured format and goes through a formal lifecycle (Draft → Proposal → Discussion → Review → Accepted/Rejected → Active).

TSRs are analogous to Python's PEPs, Java's JEPs, or Rust's RFCs.

## Quick Links

| Link | Purpose |
|------|---------|
| [TSR-000](/TSR-000.md) | The TSR process itself (normative) |
| [TEMPLATE.md](/TEMPLATE.md) | Template for writing new TSRs |
| [Index](/index.md) | A categorized overview of all TSRs |

## TSR Status Overview

| Status | Meaning |
|--------|---------|
| **Draft** | Author is writing; not yet submitted |
| **Proposal** | Submitted, awaiting review and number assignment |
| **Discussion** | Open for community feedback (min 14 days) |
| **Review** | Under active review by core team |
| **Accepted** | Approved; awaiting implementation |
| **Rejected** | Declined (reason documented) |
| **Deferred** | Postponed to future consideration |
| **Active** | Implemented and released in a Truss version |

## How to Propose a TSR

1. **Copy the template**

   ```bash
   cp TEMPLATE.md TSR-NNN.md
   ```

   (Leave `NNN` as placeholder until assigned)

2. **Write your proposal** following the template structure

3. **Submit** by opening a Pull Request to this repository

4. **Wait for number assignment** — a reviewer will assign a TSR number and move your TSR to `Proposal` status

5. **Participate in discussion** — after the PR is merged, discussion happens via GitHub Issues / Discussions

6. **Iterate** based on feedback

For full details, read **[TSR-000: TSR Purpose and Process](./TSR-000.md)**.

## When to File a TSR vs. a GitHub Issue

| **File a TSR for:** | **File an Issue for:** |
|---------------------|------------------------|
| Language syntax changes | Bug reports |
| New keywords or operators | Small feature requests |
| Standard library API additions/removals | Documentation improvements |
| Major toolchain changes (LSP, build system) | Performance regressions |
| Process or governance changes | Question or help request |
| Design decisions requiring broad consensus | Minor enhancements (single file change) |

When in doubt, file an issue first. A maintainer may suggest upgrading to a TSR.

## Repository Structure

```
truss-community/TSR/
├── README.md               # This file
├── TEMPLATE.md             # Template for new TSRs
├── TSR-000.md              # The TSR process specification
├── TSR-001.md            # Individual TSRs
├── TSR-002.md
├── text/                   # Archived or rejected TSRs
│   ├── rejected/
│   └── deferred/
└── meta/                   # Process documentation
    ├── voting.md
    └── reviewers.md
```

## Discussion Guidelines

- **Be constructive** — focus on ideas, not individuals
- **Back claims with reasoning** — "I don't like it" is insufficient
- **Assume good faith** — authors invest significant effort
- **Stay on topic** — off-topic comments may be removed
- **Minimum discussion period** is 14 days for Standards Track TSRs

Discussion happens in:

- **GitHub Discussions** (preferred for long-form)
- **Truss Discord** `#tsr` channel (for real-time chat)

## Decision Process

1. After discussion concludes, a **Reviewer** (core team member) summarizes consensus
2. **Final Decision Maker** (Language Lead or Technical Committee) issues a ruling:
   - **Accept** — move to `Accepted` status
   - **Reject** — move to `Rejected` with written rationale
   - **Defer** — move to `Deferred` (revisit later)

All decisions are documented in the TSR itself under `Rationale` and the PR/issue discussion.

## Core Team Reviewers

| Name | Area of Focus |
|------|---------------|
| *To be appointed* | Language design |
| *To be appointed* | Standard library |
| *To be appointed* | Tooling / compiler |
| *To be appointed* | Process |

## Contributing to This Repository

- **Typos or formatting issues** → Open a small PR
- **Clarifying an existing TSR** → Open an issue first
- **Proposing a new TSR** → See [How to Propose a TSR](#how-to-propose-a-tsr)

## License

All TSRs in this repository are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

## Related Resources

- [Truss Language Website](https://truss-lang.example) (Not avaliable)
- [Truss GitHub Organization](https://github.com/truss-community)
