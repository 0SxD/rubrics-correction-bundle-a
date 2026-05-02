# rubrics-correction-bundle-a

A rubric correction methodology bundle: project instructions, tandem session orchestration spec, wiki log, task spec template, and session bootstrap artifacts for structured rubric review work.

## Status

R&D. Maintained by Sage / 0SxD as part of an ongoing research portfolio focused on prompt engineering, agent skills, and LLM evaluation.

## What this is

This bundle documents a methodology for iterative rubric correction in LLM evaluation contexts. The core insight is that rubric quality degrades under two failure modes: AND-stacked criteria (a single rubric row tests two independently-failable requirements) and false-positive auto-QC flags (~7-8% observed rate). The protocol addresses both systematically through a structured intake workflow, a pre-submit gate, and a multi-turn questioning discipline. The artifacts here are the working documents from an active rubric correction workstream, published as a methodology reference.

## Approach

- Multi-turn confidence loop: agent blocks on uncertainty rather than proceeding with assumptions
- Coverage Map methodology: four columns (Source Prompt rules, User Turn requirements, carry-forward facts, carry-forward preferences) before any correction action
- Keep / Modify / Discard / Add action taxonomy with one-sentence justification per row
- Atomic-modify check: every Modify row is scanned for AND-stacked requirements before submission
- False-positive triage protocol: distinguishes verbatim-prompt-match flags, known FP patterns, and real defects
- Tandem workstream orchestration: parallel chat sessions with conflict-free file ownership

## Layout

- `project_instructions.md` - canonical protocol v2.3 with all XML directive tags
- `PROJECT_INSTRUCTIONS_CUTPASTE_v2_3.md` - paste-ready version for project settings injection
- `TASK_CHAT_BOOTSTRAP.md` - bootstrap block for task-chat initialization in tandem mode
- `tandem_session_orchestration.md` - multi-chat coordination spec (orchestrator + task chat roles)
- `task_spec_template.md` - per-task spec template (copy one per task)
- `spec_md_HOT_CACHE_update_2026-04-22_TANDEM_v2.md` - canonical state snapshot from active workstream
- `Wiki_Log_append_2026-04-22_v2.md` - insight ledger entries from the workstream

## Usage / How to read this

This repo is a documentation and methodology bundle. Open `project_instructions.md` first.

To adopt the methodology: read `project_instructions.md` for the full protocol, then use `task_spec_template.md` as the per-task working document. In a Claude project context, paste the code block from `PROJECT_INSTRUCTIONS_CUTPASTE_v2_3.md` into project settings for auto-injection into every chat.

## Prior art and citations

This methodology bundle does not directly cite external papers. The structured rubric correction approach is informed by the broader rubric-as-evaluation research context:

- Rubrics as Rewards (RaR), arXiv:2507.17746 - rubric quality and evaluation methodology background
- Adaptive Precise Boolean Rubrics (Google), arXiv:2503.23339 - boolean-atomic decomposition that motivates the atomic-modify check

See also: [ce-rd-os](https://github.com/0SxD/ce-rd-os) for the broader Trinity rubric scoring framework this bundle composes with.

## License

CC-BY-4.0. Copyright (c) 2026 Sage / 0SxD.
Author: Sage / 0SxD

## Notes

This repo is part of an active R&D portfolio. Content may move, change, or be withdrawn. Issues and PRs welcome but reviews are best-effort.
