# Wiki_Log entries for orchestrator append (v2)
# Append the following block to /mnt/project/Rubric_Correction_Wiki_Log.md
# Supersedes Wiki_Log_append_2026-04-22.md (v2 reflects v2.3 xlsx-stripped pivot)

---

## [2026-04-22 W1] orchestrator | tandem mode setup
3 parallel workstreams initiated. Workstream 1 (orchestrator, instructions/state-changes update). Workstreams 2 + 3 (task chats, pending user task-state paste). Per-task spec_TASK_NNN.md isolation pattern adopted to prevent file-write conflict. New skill: tandem_session_orchestration.md (v1.1). New template: task_spec_template.md (v1.1). New chat-bootstrap: TASK_CHAT_BOOTSTRAP.md.

## [2026-04-22 W1] insight | TASK_443 atomic-modify post-approval reviewer-correction
TASK_443 was APPROVED by auto-QC. Reviewer post-approval simplified R2 (shellfish AND-stacked) and R4 (headings AND food-stops AND USD-prices stacked). Auto-QC v2 does NOT reliably catch all AND-stacking on Modify rows. Manual atomic-modify scan required pre-submit. Promoted to <atomic_modify_check> in project_instructions.md v2.3 + atomic_split_decision.md update.

## [2026-04-22 W1] canon-delta | night onboarding PDF additions
Night PDF adds (a) Cheat Sheet for Edge Cases in Reviewer Checklist with 3 cases (sanity-check final turns, hedging language, incomplete-info requests); (b) April 21 4pm PT entry "Closed onboarding evaluation acceptance period." Both day + night PDFs share new goal "700 additional tasks complete by Thursday 4/23 10am PT." Promoted to <cheat_sheet_edge_cases> + <goal> update in project_instructions.md v2.3.

## [2026-04-22 W1] update | project_instructions.md v2.3
Bumped from v2.2. Removed all Final Sprint xlsx references (workflow not in active use for this user, confirmed via CSV scan: 868 rows, 30 unique reviewers, no name match). <fp_triage_first> reframed as RLS QC v2 FP triage discipline (~7-8% FP rate). Removed <sprint_workflow> block. Removed sprint_xlsx from <canon_read_only>. <goal> simplified. All other v2.2 additions retained. Matching CUTPASTE v2.3 generated for Claude Project settings.

## [2026-04-22 W1] artifact | TASK_CHAT_BOOTSTRAP.md
New artifact for tandem mode: single bootstrap code block user pastes into first message of EACH new task chat, followed by initial Studio task state. Sets task-chat role, references v2.3 protocol, lists standard_intake workflow steps, names canon files for read-only reference. Both task chats use the same bootstrap; Task NNN identifier is read from pasted task state header.

END_WIKI_LOG_APPEND
