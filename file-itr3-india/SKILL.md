---
name: file-itr3-india
description: Step-by-step guide to file an Indian ITR-3 for a resident with salary PLUS Section 44ADA professional/freelance income (including foreign clients paid into an Indian bank), and/or intraday/speculative or F&O trading, and/or foreign assets like ESOPs and US stocks — under the New Tax Regime on incometax.gov.in. Use when a salaried person ALSO has 44ADA presumptive income, share/F&O/intraday trading, or foreign ESOPs/US stocks and must file ITR-3 (AY 2026-27 onward). For salary-only, use file-itr1-india instead.
---

# File ITR-3 (India) — salary + 44ADA + trading + foreign assets

> Figures are **AY 2026-27 (FY 2025-26)**; re-verify slabs, 87A rebate, deadlines, and business codes each year. Full detail (walkthrough, codes, error fixes, Schedule FA, ESOP tax) is in **[REFERENCE.md](REFERENCE.md)** — read it before filing.

## Form-selection logic — why ITR-3
Use ITR-3 if ANY apply (none of these fit ITR-1/2/4):
- **Intraday equity/ETF** trading (= **speculative business**, §43(5)) or **F&O** (= non-speculative business) — **any amount forces ITR-3**, even ₹100.
- **44ADA presumptive** professional income **alongside** other business income (e.g. the intraday above).
- **Foreign assets** held in the calendar year — vested/exercised **ESOPs**, **US stocks** → Schedule FA → ITR-2/ITR-3.

*Presumptive 44ADA alone → ITR-4. Add intraday/F&O or foreign assets and it becomes ITR-3.*

## Phase 1 — Collect & reconcile
- **Form 16** (each employer) · **AIS + TIS** · **Form 26AS** · **bank statements** (full FY).
- **44ADA / foreign-client income**: contract, **W-8BEN**, platform report (FIRA + invoices), and the **bank statement**. Report on a **RECEIPT basis** — only amounts actually **credited by 31 Mar** count; a wire dated 31 Mar but credited 1–2 Apr belongs to the **next** FY.
- **Broker capital-gains / Tax-P&L** (e.g. Groww): split **intraday (speculative)** from **delivery** gains; identify **F&O**.
- **Foreign assets**: ESOP grant agreements (grant date, vesting-commencement, strike); US-stock statements (INDmoney/Vested).
- Reconcile salary **26AS = AIS = Form 16**. Foreign-client income is often **NOT in AIS** (domestic-NEFT via the platform's Indian bank) → your **bank statement + FIRA** are the primary evidence.

## Phase 2 — Classify & compute (New Regime)
- **Salary**: gross − **₹75,000** standard deduction.
- **44ADA**: **50%** of gross receipts as income; profession code e.g. **16005 – Engineering and technical consultancy** (for IT/GRC/tech consultancy); declare **≥50%** to avoid audit.
- **Intraday/speculative**: net profit; nature code **21009 – Speculative Trading**; **turnover = absolute sum of profits+losses** (not sale value).
- **Interest** (every bank, from AIS) → Schedule OS.
- **87A rebate**: total income ≤ **₹12,00,000** and **all slab-rate** (no special-rate 111A/112A) → tax **₹0**.

## Phase 3 — Schedule FA (foreign assets — high stakes)
- Schedule FA uses the **CALENDAR year (1 Jan–31 Dec)**, not the financial year.
- **Unvested** ESOPs and assets **acquired after 31 Dec** are **not** reportable that AY.
- Foreign shares / US stocks / **vested** ESOPs held during the calendar year → **mandatory Schedule FA** (₹10 lakh Black Money Act penalty per year for omission). Details in REFERENCE.md §F.

## Phase 4 — File & verify
Follow the **screen-by-screen walkthrough** and **validation-error fixes** in REFERENCE.md §H–I. Then **Preview → Submit → e-Verify (Aadhaar OTP) within 30 days**. ITR-3 non-audit **due date: 31 August**.

## Master checklist
- [ ] 26AS = AIS = Form 16 (salary); foreign-client income reconciled to bank on **receipt basis**
- [ ] 44ADA gross receipts + 50%; correct **profession code**; intraday under code **21009**
- [ ] **A19(b) = Yes** (reverts if you revisit "Select Schedule" — re-check it)
- [ ] Balance Sheet **"No-Account" item 6** filled (cash balance) — else an upload-level "defect"
- [ ] **Schedule FA**: nothing foreign held in the calendar year? (else disclose)
- [ ] Tax = ₹0 (87A); bank account pre-validated
- [ ] Filed by **31 Aug**; **e-verified within 30 days**

**→ Read [REFERENCE.md](REFERENCE.md) for the full walkthrough, business codes, the validation errors you WILL hit and their fixes, the ESOP tax timeline, and Schedule FA rules.**
