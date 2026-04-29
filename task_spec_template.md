# task_spec_template.md | per-task spec template
# Version: 1.1 | 2026-04-22 | xlsx refs removed
# Purpose: Each task chat copies this file to spec_TASK_NNN.md after first user message naming the task.
# Trees-upward to canonical spec.md via PARENT_REF link.
# Avoids file-write conflict in tandem multi-chat operation.

---

# spec_TASK_NNN.md | per-task state
<!-- replace NNN with actual task number; update PARENT_REF; fill HOT_CACHE -->

## PARENT_REF
- canonical: project://spec.md
- protocol_canon: project://project_instructions.md (v2.3+)
- skill_tree: project://skills.md
- wiki_log: project://Rubric_Correction_Wiki_Log.md

## TASK_META
- task_id: <Task NNN | task_<hash>>
- world: <B1 | Onboarding Evaluation | other>
- claimed_at: <ISO timestamp>

## HOT_CACHE
<!-- max 500 words | next actions + active vars | overwrite each turn -->

STATUS: <one-sentence current state>
SESSION_TYPE: <intake | revision | hard-fail-recovery | submit-pending | reviewer-pending>
ACTIVE_TASK: <Task NNN>
NEXT_ACTION: <single concrete next step>

ACTIVE_VARS:
- task_NNN_intake_summary: <SP rules count, UT count, existing rows count, suggested-add count>
- task_NNN_coverage_map: <Column A SP / B final-UT / C carry-forward facts / D earlier-turn prefs>
- task_NNN_kmda_plan: <K count + M count + D count + A count, with rationale per row>
- task_NNN_qc_state: <P1 result / P2 result / P3 result, last run timestamp>
- task_NNN_known_FPs: <list any flags overridden as false positive with reason>
- task_NNN_writer_comments: <pending text to paste into Writer Comments box>

CONFIDENCE: TRUE=1 <ship-ready> | FALSE=0 <reason blocking>

## GRAPH_LINKS
<!-- task-specific files only -->
- cutpaste: outputs://Rubric_Correction_Task_NNN_<slug>_<date>_CUTPASTE.md
- analysis: outputs://Rubric_Correction_Task_NNN_<slug>_<date>_ANALYSIS.md
- coverage_map: outputs://Rubric_Correction_Task_NNN_<slug>_<date>_COVERAGE_MAP.md

## INSIGHTS_LOCAL
<!-- mine 1 pattern minimum per turn; promote to canonical spec.md INSIGHTS_LEDGER at task close -->

[task NNN insight 1] <pattern observed + evidence-class tag (DIRECT_OBSERVATION / USER_REPORT / DOCUMENT_TEXT / INFERENCE / SPECULATION)>

## OPEN_Q
<!-- blocking questions to user; clear when answered -->

## RULES_INVOKED
<!-- subset of canonical project_instructions.md rules active for this task -->
- standard_intake: invoked
- pre_submit_gate: invoked
- atomic_modify_check: invoked
- fp_triage_first: invoked (if any QC v2 flags appear)
- cheat_sheet_edge_cases: invoked (if any of 3 cases apply)
- evidence_class_tagging: always invoked

## TASK_CLOSE_PROMOTION
<!-- on task submit, orchestrator copies these to canonical -->
- insights_to_promote: <list from INSIGHTS_LOCAL>
- skill_updates: <list any skill .md files updated or suggested>
- wiki_log_entry: <draft Wiki_Log line for orchestrator to append>

END_TASK_SPEC
