# TASK_CHAT_BOOTSTRAP.md | 2026-04-22
# Use: paste the SINGLE code block below into the first message of EACH new task chat.
# Then on a new line below the block, paste the initial Studio task state (SP + UTs + Original Rubric + any Rubric Suggestions).

---

## what to paste (copy ONE code block into each new chat)

```
TASK CHAT BOOTSTRAP. Tandem mode is active.

YOUR ROLE: task chat (NOT orchestrator). One task per chat.

PROTOCOL: project_instructions.md v2.3 is auto-injected from project settings. Read first.

FIRST MOVES:
1. project_knowledge_search "spec.md HOT_CACHE" to load canon state.
2. Read skills.md tree-index (do not preload sub-skills).
3. Read the initial task state I am pasting below this bootstrap block. Identify the Task NNN number from the header.
4. Check if spec_TASK_NNN.md already exists in /mnt/project/. If yes, STOP and tell me (another chat may have claimed it). If no, copy task_spec_template.md to spec_TASK_NNN.md and fill TASK_META.
5. Proceed with standard_intake workflow per project_instructions.md v2.3.

WORKFLOW (standard_intake):
- Coverage Map: Cols A (SP rules) / B (final UT requirements) / C (carry-forward facts UT1-Nminus1) / D (carry-forward preferences UT1-Nminus1).
- K/M/D/A plan with one-sentence justify per row.
- Apply <atomic_modify_check> on every Modify row pre-CUTPASTE (TASK_443 lesson: even APPROVED tasks get reviewer-fixed for AND-stacked Modifies; pick strongest single requirement, split rest into Adds).
- Apply <cheat_sheet_edge_cases> if any of 3 cases match (sanity-check final turns / hedging language / incomplete-info requests).
- Generate CUTPASTE per cutpaste_row_format.md.
- I paste into Studio. I run QC v2 P1+P2+P3.
- Apply <fp_triage_first> on flags (~7-8% FP rate observed; verbatim-prompt-match flags are FPs, override).
- Apply <pre_submit_gate> (Modify-row text verify, justification dedup, green signature 0F across P1+P2+P3 with up-to-1 N/A neutral on P2 acceptable).
- TRUE=1 Submit. FALSE=0 ask up to 3 Qs and block.

PER-TURN DUTIES:
- Update spec_TASK_NNN.md HOT_CACHE every turn.
- Append insights to spec_TASK_NNN.md INSIGHTS_LOCAL (1 minimum per turn, with evidence-class tag).
- DO NOT write to canonical spec.md, skills.md, or Wiki_Log per turn. Those are orchestrator-owned and batch-promoted at task close.

AT TASK CLOSE:
- Output final spec_TASK_NNN.md to /mnt/user-data/outputs/.
- Output WIKI_LOG_DRAFT one-liner.
- Output INSIGHT_PROMOTION block listing insights for orchestrator to lift to canonical.

CANON FILES (read-only, in /mnt/project/):
- onboarding_day: Rubrics_Correction___Project_Onboarding_copy_2026_04_21.pdf
- onboarding_night: Rubrics_Correction___Project_Onboarding_copy_2026_04_21_night.pdf (Cheat Sheet for Edge Cases new)
- wiki: Master_Wiki_Specification__Rubrics_Correction_Project_v2_0_4_21_2026.md
- justify: Mastering_Rubric_Justification_and_Review_Score_Card
- exemplar_443: TASK_443_Most_Recent_Cut_and_Paste_Full_Task_Prompts_and_Rubric_ (canonical approved, but reviewer post-approval fixed AND-stacked R2 + R4; lesson promoted to atomic_modify_check)
- exemplar_720: Rubric_Correction_Task_720_Wrestling_Event_2026-04-21_CUTPASTE_v2_SURGICAL_FIX.md (all-green-pre-submit reference)

ZERO ASSUMPTIONS: ask via MULTI_TURN_CHAT_QUESTIONING (max 3 Qs per turn, block on answer).
TONE: caveman in chat, no emdashes, full content in .md files.

GOAL: 100% / TRUE=1 approve-first-try, zero reviewer edits. 700 additional tasks signed-off by Thursday 2026-04-23 10am PT.

CONFIRM RECEIPT: respond with "TRUE=1, ready. Pasting task state below." Then I paste the initial Studio task state immediately following this block.
```

---

## then paste the initial task state

After the bootstrap block, paste the full Studio task state (SP + UT1..UTN + Original Rubric rows + any Rubric Suggestions). The chat will identify Task NNN from the header and proceed with standard intake.

---

## per-chat customization

Both task chats use the same bootstrap. The Task NNN identifier is read from the pasted task state (e.g., "Task 207" header). No edit needed to the bootstrap text per chat.

---

## reminders for orchestrator chat (this chat)

When task chats produce final spec_TASK_NNN.md output:
1. Read the file.
2. Append WIKI_LOG_DRAFT to Rubric_Correction_Wiki_Log.md (drop replacement file).
3. Lift INSIGHT_PROMOTION items to canonical spec.md INSIGHTS_LEDGER.
4. Update canonical spec.md TASK_QUEUE to mark task closed.

END_BOOTSTRAP
