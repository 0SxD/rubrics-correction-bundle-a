# spec_md_HOT_CACHE_update_2026-04-22_TANDEM_v2.md
# REPLACE the HOT_CACHE block in spec.md with the block below.
# Append the INSIGHTS_LEDGER additions and the new GRAPH_LINKS.
# Supersedes spec_md_HOT_CACHE_update_2026-04-22_TANDEM.md (v2 strips xlsx refs).

---

## REPLACEMENT HOT_CACHE BLOCK

STATUS: Tandem mode active. Orchestrator chat (this one) handling state-changes/instructions update (workstream 1) per project_instructions.md v2.3 (xlsx workflow stripped, standard intake only). Two task chats opening for STANDARD intake (workstreams 2 + 3, not yet started). Goal per onboarding canon both PDFs: 700 additional tasks signed-off by Thu 4/23 10am PT.

SESSION_TYPE: Orchestrator role. Workstream 1 = canon/instructions tightening (THIS chat). Workstreams 2+3 = task chats (per-task spec files trees-upward to canonical). Standard intake workflow only; sprint xlsx workflow not in active use for these chats.

ACTIVE_TASK: workstream 1 (orchestrator). Per-task chats own their spec_TASK_NNN.md files.

NEXT_ACTION: User (a) pastes PROJECT_INSTRUCTIONS_CUTPASTE_v2_3.md code block into Claude Project settings text field, (b) drops bundle files into /mnt/project/ root, (c) opens 2 new chats in this project (each auto-injects v2.3), (d) pastes TASK_CHAT_BOOTSTRAP.md code block into first message of each new chat followed by initial Studio task state.

ACTIVE_VARS:
- workstream_1_state: project_instructions.md v2.3 drafted (xlsx-stripped). PROJECT_INSTRUCTIONS_CUTPASTE_v2_3.md drafted. task_spec_template.md cleaned. tandem_session_orchestration.md cleaned. TASK_CHAT_BOOTSTRAP.md drafted for paste into 2 new chats.
- workstream_2_state: pending user task-state paste in new chat.
- workstream_3_state: pending user task-state paste in new chat.
- night_vs_day_pdf_delta: night PDF adds (a) Cheat Sheet for Edge Cases (3 cases: sanity-check final turns, hedging language, incomplete-info requests) in Reviewer Checklist; (b) April 21 4pm PT entry "Closed onboarding evaluation acceptance period." Both PDFs share new goal "700 additional tasks complete by Thursday 4/23 10am PT."
- task_443_stacking_lesson: TASK_443 was APPROVED then reviewer post-approval simplified R2 (shellfish AND-stacked) and R4 (headings AND food-stops AND USD-prices stacked). Lesson promoted to atomic_split_decision.md + new <atomic_modify_check> rule in project_instructions.md v2.3.
- per_task_spec_pattern: each task chat copies task_spec_template.md to spec_TASK_NNN.md after first user message names the task. Trees-upward via PARENT_REF. Avoids file-write conflict in tandem mode.
- xlsx_workflow_archived: SESSION_HANDOFF_2026-04-22_FINAL_SPRINT_PIVOT.md, final_sprint_workflow.md, autoqc_reverse_graph.md remain in /mnt/project/ for future reference but are NOT loaded by v2.3 protocol. User name not in xlsx column I (verified via CSV scan, 30 unique reviewers, no Austin variant).
- orchestrator_duties: validate cross-task conflict, batch-promote insights at task close, maintain canonical TASK_QUEUE, append Wiki_Log on close.

CONFIDENCE: TRUE=1 for workstream 1 v2.3 bundle as drafted. FALSE=0 on workstreams 2+3 until task state pasted.

---

## INSIGHTS_LEDGER ADDITIONS

### [2026-04-22 W1] insight 25: task_443_post_approval_reviewer_atomic_modify_correction
TASK_443 was APPROVED by auto-QC then reviewer post-approval simplified R2 + R4 because they had AND-stacked requirements. Auto-QC v2 does NOT reliably catch all AND-stacking on Modify rows. Manual atomic-modify scan required pre-submit. EVIDENCE_CLASS: USER_REPORT (user told us reviewer fixed one stacking issue). Promoted to <atomic_modify_check> in project_instructions.md v2.3 + atomic_split_decision.md update.

### [2026-04-22 W1] insight 26: night_pdf_cheat_sheet_three_cases
Night onboarding PDF adds Cheat Sheet for Edge Cases in Reviewer Checklist with 3 cases: sanity-check final turns (cover only what user explicitly asks), hedging language (mirror the hedge), incomplete-info requests (test response within constraints actually given). EVIDENCE_CLASS: DOCUMENT_TEXT. Promoted to <cheat_sheet_edge_cases> in project_instructions.md v2.3.

### [2026-04-22 W1] insight 27: tandem_chat_file_isolation_via_per_task_spec
Multi-chat parallel work conflicts on shared file writes (spec.md, skills.md, Wiki_Log). Solution = per-task spec_TASK_NNN.md files trees-upward to canonical. Orchestrator chat owns canonical, task chats own per-task files. Shared writes batched at task close. EVIDENCE_CLASS: INFERENCE (from file-system semantics + tandem requirement). Promoted to <tandem_workstreams> in project_instructions.md v2.3 + tandem_session_orchestration.md.

### [2026-04-22 W1] insight 28: goal_update_to_700_by_thursday
Both day + night PDFs show "Final Delivery: 700 additional tasks complete by Thursday 4/23 10am PT" (not 1000 by Wed 4/22 EOD). Prior project_instructions.md v2.1 carried the older number. EVIDENCE_CLASS: DOCUMENT_TEXT. Project_instructions.md v2.2+ corrects.

### [2026-04-22 W1] insight 29: xlsx_workflow_not_used_user_not_in_revisor_pool
Verified via Final Sprint CSV scan: 868 rows, 30 unique reviewer names in column I, no "Austin" variant. User confirmed standard intake only. xlsx workflow files retained in /mnt/project/ for future reference but stripped from active protocol v2.3. EVIDENCE_CLASS: DIRECT_OBSERVATION (CSV scan).

---

## COMPACTION_LEDGER ADDITIONS

- [2026-04-22 W1] PRUNED: goal "1,000 tasks by EOD Wednesday 4/22." REPLACEMENT: "700 additional tasks signed-off by Thursday 4/23 10am PT" per onboarding canon both PDFs.
- [2026-04-22 W1] PRUNED: <sessions_parallel_split> A/B file refs (obsolete v2.0 pattern). REPLACEMENT: <tandem_workstreams> per-task spec isolation (v2.2+).
- [2026-04-22 W1] PROMOTED: TASK_443 stacking lesson from user-report to canonical rule (<atomic_modify_check> + atomic_split_decision.md update).
- [2026-04-22 W1] PRUNED v2.3: Final Sprint xlsx workflow refs (<sprint_workflow>, sprint_xlsx canon entry, AHT/bonus refs). Standalone files (final_sprint_workflow.md, autoqc_reverse_graph.md) kept on disk but unlinked from active protocol.

---

## TASK_QUEUE UPDATE

- workstream_1 (orchestrator, this chat): bundle v2.3 drafted, awaiting user drop into project root + paste of CUTPASTE v2.3 into Claude Project settings.
- workstream_2 (task chat A, pending): user pastes TASK_CHAT_BOOTSTRAP + initial task state.
- workstream_3 (task chat B, pending): user pastes TASK_CHAT_BOOTSTRAP + initial task state.
- task_881 v5: status unknown to this chat. Confirm if shipped Approved.
- task_720 + task_883: prior reviewer-pending. Confirm verdict.

---

## GRAPH_LINKS ADDITIONS

- workstream_1_v2.3_bundle: outputs://project_instructions.md (v2.3), outputs://PROJECT_INSTRUCTIONS_CUTPASTE_v2_3.md, outputs://task_spec_template.md (cleaned), outputs://tandem_session_orchestration.md (cleaned), outputs://TASK_CHAT_BOOTSTRAP.md (NEW)
- canon_onboarding_night: project://Rubrics_Correction___Project_Onboarding_copy_2026_04_21_night.pdf
- subskill_tandem: project://tandem_session_orchestration.md (NEW v1.1)
- per_task_spec_template: project://task_spec_template.md (NEW v1.1)
- task_chat_bootstrap_template: outputs://TASK_CHAT_BOOTSTRAP.md (NEW)

---

END_HOT_CACHE_UPDATE
