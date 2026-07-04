# India ITR Filing Skills

Two [Agent Skills](https://docs.claude.com/en/docs/claude-code/skills) that guide filing Indian income-tax returns end-to-end on `incometax.gov.in`, distilled from a real filing. Drop them into any Claude Code / agent skills directory.

| Skill | For | Covers |
|---|---|---|
| **`file-itr1-india`** | Salary-only earners (ITR-1 Sahaj) | Doc collection & reconciliation, New Regime + 87A, portal walkthrough, e-verify |
| **`file-itr3-india`** | Salary **+** 44ADA freelance/foreign-contractor income, intraday/F&O trading, or foreign ESOPs/US stocks (ITR-3) | Everything above **+** form-selection logic, 44ADA (receipt basis), speculative income, business codes, Schedule FA (foreign assets), ESOP tax timeline, and fixes for every validation error |

## Install
Copy each skill folder into your skills directory:
```bash
cp -R file-itr1-india file-itr3-india ~/.claude/skills/
```
Then invoke via `/file-itr1-india` or `/file-itr3-india`, or let the agent auto-select based on the situation.

## Which one?
- Only salary (+ small bank interest), no capital gains, no foreign assets → **ITR-1**.
- Any freelance/44ADA income, **any** intraday/F&O trade, or foreign ESOPs/US stocks → **ITR-3**.

## Structure
```
file-itr1-india/SKILL.md          # self-contained, ~55 lines
file-itr3-india/SKILL.md          # workflow + checklists
file-itr3-india/REFERENCE.md      # detailed walkthrough, codes, error fixes, Schedule FA, ESOP tax
```

## ⚠️ Disclaimer
Informational, not professional tax advice. Tax **figures are AY 2026-27 (FY 2025-26)** — slabs, the 87A rebate, standard deduction, business codes, and due dates change yearly, so **re-verify the numbers each year** on the official portal. The *process and methodology* are the durable part; consult a CA for anything non-standard (44ADA eligibility, foreign-asset disclosure, ESOP exercise).
