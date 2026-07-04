# ITR-3 Filing Reference (India)

> Companion to SKILL.md. Numbers are **AY 2026-27**; re-verify each year. This encodes a real filing: salary (2 employers) + 44ADA foreign-contractor income + accidental intraday ETF trades + unvested foreign ESOPs + US stocks bought after the FY.

## A. Document reconciliation
| Doc | Where | Notes |
|---|---|---|
| Form 16 | Employer / payroll portal | May lag; **AIS + 26AS already confirm salary + TDS**, so you can file without it. |
| AIS + TIS | portal → AIS | PDF password = **PAN-lowercase + DDMMYYYY DOB**. TIS is the summary. |
| Form 26AS | e-File → ITR → View 26AS | The tax-credit statement. |
| Bank statements | net-banking | Full FY. The **primary evidence** for foreign-client receipts. |
| FIRA + invoices | cross-border payment platform | Proof of inward remittance for 44ADA receipts. |
| Broker Tax-P&L | Groww/Zerodha etc. | Splits intraday (speculative) vs delivery vs F&O. |

**Golden rule:** reconcile salary **26AS = AIS = Form 16**. Note: foreign-client income often is **NOT** in AIS (it arrives as domestic NEFT/IMPS from the platform's Indian correspondent/nostro bank rather than as a classic SWIFT inward remittance), so bank statement + FIRA are your evidence. Watch AIS for interest across **every** bank and any SFT (securities purchases, LRS remittances — a foreign debit-card charge can show as an "LRS remittance").

## B. Form-selection decision tree
- Only salary/interest, no CG, no foreign assets → **ITR-1**.
- Capital gains or foreign assets, but no business income → **ITR-2**.
- Presumptive 44AD/44ADA/44AE **only** → **ITR-4**.
- **Any** of: intraday/F&O (speculative or business), 44ADA + other business income, foreign assets requiring Schedule FA → **ITR-3**.
- A single ₹100 intraday trade → **ITR-3** (speculative income can't live in ITR-1/2/4). Filing the wrong form risks a **§139(9) defective-return** notice.

## C. Section 44ADA (presumptive profession)
- Eligible: professions under §44AA(1) — legal, medical, **engineering**, architecture, accountancy, **technical consultancy**, IT, etc. IT/security/GRC consulting fits "**technical consultancy**".
- **Receipt basis**: gross receipts = INR actually **credited to the bank by 31 Mar**. A wire dated 31 Mar but credited 1–2 Apr → **next FY**. Reconcile against the bank statement, not the platform's "transaction date".
- Declare **≥50%** as income (exactly 50% is fine; declaring **less** triggers mandatory books + tax audit).
- **Profession code**: enter in **Part A-P&L item 62**. Use e.g. **16005 – Engineering and technical consultancy**. Avoid **16019 (n.e.c.)** and software-*business* codes (14xxx) — they weaken the "profession" position.
- Receipts breakup in item 62: put the whole amount in **row A** (a/c payee / electronic modes) if paid by bank.
- Foreign-client income is **Indian-source professional income** (services rendered from India) → 44ADA + ITR-3 is fine. A **W-8BEN** on file means no US withholding → **no Form 67 / FTC** needed.
- Keep the signed contract as evidence for the "technical consultancy" classification.

## D. Intraday / speculative / F&O
- **Intraday** equity/ETF (squared off same day, no delivery) = **speculative business** (§43(5)). Intent ("it was a mistake") doesn't change the tax character.
- **Turnover** for speculative = **absolute sum of profits and losses** per trade (NOT sale value). Brokers label this "turnover" in the Tax-P&L.
- Nature-of-business codes (added AY 2025-26): **21009 – Speculative Trading** (intraday), **21010 – F&O**, **21011 – delivery-based share trading (as business)**. Don't use old generic codes (09028/13018) — the dept cross-checks SEBI data.
- Enter net profit in **Part A-P&L item 64/65 "No-Account Case → speculative activity"** (turnover, gross profit, net income). It flows to **Schedule BP section B** automatically.
- **Audit info** (Part A-General): a1 (maintain books §44AA) = **No**; a2 (income **only** presumptive) = **No** (because you also have speculative); a2i turnover range = **Up to ₹1 crore**; b (44AB audit) = **No**; 92E = **No**.

## E. New Regime + Section 87A
- AY 2026-27 slabs: 0–4L nil · 4–8L 5% · 8–12L 10% · 12–16L 15% · 16–20L 20% · 20–24L 25% · >24L 30%.
- **Standard deduction ₹75,000**; **87A rebate up to ₹60,000** for total income **≤ ₹12,00,000** → **₹0 tax**.
- Rebate applies only to **slab-rate** income — NOT special-rate (111A STCG, 112/112A LTCG, 115BB). Presumptive + speculative + salary + interest are all slab-rate, so the rebate applies fully.
- Stay in the new regime → do **NOT** file Form 10-IEA; in Part A answer "opt out of new regime" = **No**.
- Just above ₹12L, **marginal relief** caps the extra tax at the income over ₹12L.

## F. Schedule FA — foreign assets (Black Money Act stakes)
- **Reporting window = the CALENDAR year (1 Jan–31 Dec)** falling in the FY — unique to Schedule FA; every other schedule uses Apr–Mar.
- Report anything held **at any time** in that calendar year: foreign shares, US stocks (INDmoney/Vested = foreign broker + foreign equity), vested ESOP shares, foreign bank/wallet balances. **No minimum value** — one fractional share counts.
- **Unvested** ESOP options and assets **acquired after 31 Dec** → **not** reportable that AY (they roll into next year).
- A foreign debit-card subscription (e.g. Twitter/X) shows in AIS as an "LRS remittance" but is **spending, not an asset** — not Schedule FA.
- Schedule FA lives only in **ITR-2/ITR-3**. Omitting it = **₹10 lakh penalty per year** under the Black Money Act (relief if total movable foreign assets < ₹20 lakh, but the disclosure duty remains). FATCA/CRS means the dept gets the data anyway.

## G. Foreign ESOP tax timeline (private/foreign company)
- **Grant** = no tax. **Vesting** of *options* = no tax. **Exercise** = perquisite tax on (FMV − strike) × shares, added to **salary** that year (you owe tax on a paper gain before any cash — plan for it). **Sale** = capital gains (foreign shares: LTCG >24 months @ 12.5%, else STCG at slab).
- Private company (e.g. PE/VC-backed, not publicly listed) = **illiquid**: no cash until a sale/IPO/buyback.
- The grant's **India appendix** typically requires (FEMA) repatriating sale/dividend proceeds and declaring the shares in **Schedule FA**.
- Once vested/exercised → Schedule FA every year → you're on **ITR-3** going forward.

## H. Portal walkthrough (screen by screen)
1. Login → **e-File → Income Tax Returns → File Income Tax Return** → AY → **Online** → **Individual** → **ITR-3**.
2. Reason → "Taxable income is more than the basic exemption limit."
3. **Select Schedule**: tick Salary, Other Sources, **Part A-P&L, Part A-Balance Sheet, Schedule BP**; keep mandatory CYLA/BFLA/CFL/AMTC/Part B-TI/TTI/Verification; **untick** 5A, House Property, Capital Gains, FA (if no CY foreign asset), AL, **Tax deferred on ESOP**, depreciation.
4. **Schedule questions wizard**: Form 10-IEA = No; opt out of new regime = No; salary exemptions = No; **Business: 44ADA = Yes** (others No); Deductions (80CCD(2)/80CCH) = No.
5. **Part A-General**: verify personal info; **A19(b) business income = Yes**; residential status = **Resident**; Director/Partner/Unlisted/FPI = **No**; audit info (§C above); **Nature of Business → add the intraday** with code 21009; **Bank Details** → a pre-validated account.
6. **Part A-P&L**: item **62** = 44ADA (gross receipts, 50% income, profession code 16005); item **64/65** = speculative (turnover, net income). Skip items 13–60.
7. **Part A-Balance Sheet**: **item 6 only** (No-Account) — debtors/creditors/stock = 0, **cash balance = your 31-Mar bank balance**.
8. **Schedule Salary**: verify pre-fill; set **Nature of employer = "Others"** for each private employer.
9. **Schedule OS**: all interest (savings + FD + others).
10. Confirm auto schedules (CYLA/BFLA/CFL/AMTC/VI-A). **Part B-TI** → verify total income. **Part B-TTI** → verify **tax = ₹0** (87A rebate line populated); foreign-asset question 14 = No.
11. **Preview → Proceed to Verification → e-Verify (Aadhaar OTP) within 30 days.**

## I. Validation errors you WILL hit — and the fix
| Error | Fix |
|---|---|
| "Select Yes at A19(b)… business income present" | Part A-General **A19(b) = Yes**. It **reverts to No** if you revisit "Select Schedule" — always re-check and re-confirm Part A-General after any schedule change. |
| "Nature of employer / perquisites / profit-in-lieu" in Salary | Set those dropdowns in Schedule Salary (even for ₹0 fields); **Nature of employer = "Others"** for private companies. |
| "Balance sheet is not filled" (upload-level, Category B/D — *allows* upload) | Fill **Part A-Balance Sheet item 6** (cash balance). It's a soft defect but **fix it** to avoid a §139(9) notice. |
| "Tax deferred on ESOP" demands startup PAN/DPIIT | That schedule is only for **§80-IAC eligible-startup** ESOP deferral. **Uncheck its rows / remove the schedule**; never invent a PAN/DPIIT. |
| All schedules vanish after revisiting "Select Schedule" | Data is **preserved server-side** — just re-select the schedules and re-confirm; entered figures reappear. |

## J. Deadlines & aftercare
- Due dates AY 2026-27: **ITR-1/2 → 31 Jul**, **ITR-3/4 non-audit → 31 Aug**, audit → 31 Oct, TP → 30 Nov. **e-Verify within 30 days.**
- Nil tax → no advance tax, no 234B/234C. Filing late (income > ₹5L) → ₹5,000 fee u/s 234F.
- Keep the full evidence pack ~6–8 years.
- **Next year:** foreign assets (US stocks / vested ESOPs) → **Schedule FA mandatory**; if you **exercise** ESOPs → perquisite tax; **F&O/speculative losses** carry forward only if you file by the due date; watch **20% TCS** on LRS remittances > ₹10L (claim in ITR).
