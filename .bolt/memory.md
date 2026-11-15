# Project memory

## Product intent & audience

- C Programs Code Library Website: a responsive site presenting C programs as individual pages with editable code.
- Homepage uses cards (originally 5, being expanded to 8) that link to per-program pages.
- Each program page includes a dark-themed editable code editor and a copy-to-clipboard button.
- Audience: learners/developers referencing and experimenting with C code samples.

## Brand personality & voice

- Practical, educational, straightforward reference tool.
- Code is the primary content; UI is functional and minimal.

## Visual design & UX direction

- Responsive layout; homepage is card-based grid.
- Program pages feature dark-themed code editor with copy-to-clipboard action.
- Shared stylesheet and shared homepage across all program pages — updates must merge, not replace.
- Cards are the primary navigation pattern.

## Decisions, constraints & rationale

- User has manually edited programs 1–5 directly in GitHub; those edits must not be overwritten.
- Homepage and stylesheet are shared with programs 1–5 — changes require careful merge, not wholesale replacement.
- Bolt cannot push directly to GitHub from chat; recommended path is GitHub import to open the repo as a new Bolt project, then sync.
- Plan: add only programs 6–8, their homepage cards, and matching style updates; leave programs 1–5 untouched.
- Framework: DEFAULT_TO_DEV.

## Open questions & assumptions

- Whether user will proceed with GitHub import plan or choose another sync method.
- Exact current state of shared homepage/stylesheet in GitHub after user's manual edits (not yet seen).
- Whether programs 6–8 already exist in the local Bolt project or still need to be created.
- Specific C program content for programs 6–8 is unspecified.
- Repository URL/identity not yet provided.