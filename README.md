# Working Capital & Cash Conversion Cycle Analyzer

## 1. Problem Definition
* **Target User:** Small business owners, residential property managers, and corporate finance students.
* **Problem Addressed:** Small businesses often struggle to visualize how shifting inventory turnover, accounts receivable (AR) collection periods, and accounts payable (AP) payment terms ripple into immediate cash flow needs and short-term borrowing costs. This tool bridges accounting formulas with practical liquidity management.

## 2. Core Function
* An interactive financial calculator that allows users to adjust operating variables (Revenue, COGS, DSO, DIO, DPO, and Borrowing Rate) via sliders and input fields. It instantly calculates the Cash Conversion Cycle (CCC), net working capital requirements, annual financing carrying costs, and scenario deltas.

## 3. Testing Summary
* **Normal Operation:** Tested baseline inputs (Revenue: $1,200,000; COGS: $800,000; AR: 45 days; Inventory: 30 days; AP: 30 days) yielding a CCC of 45 days and $98,630 in locked working capital. **[PASS]**
* **Contrasting Scenario:** Adjusted AR Days via interactive sliders to observe dynamic real-time updates to cash flow impact. **[PASS]**
* **Boundary / Invalid Input:** Tested negative numbers and non-numeric inputs; application successfully caught invalid data and prevented calculation crashes. **[PASS]**
* **Mobile Display:** Verified that the responsive grid stacks cleanly on mobile viewports without horizontal scrolling. **[PASS]**
* **Independent Verification:** Manually recalculated baseline scenarios using standard financial management formulas, verifying a variance of $0.00 against application outputs. **[PASS]**

## 4. Improvement & Iteration
* **Feedback Received:** Initial users noted that financial acronyms (such as DSO and DIO) were unclear without prior finance background knowledge.
* **Revision Made:** Added clear informational helper text and tooltips beside each input metric explaining what the metric represents and how it directly affects cash flow.

## 5. Limitations & Future Scope
* **Limitations:** Assumes steady-state annual operations and constant cost structures. It does not account for seasonal fluctuations or sudden supply chain shocks.
* **Future Scope:** Real-world implementation would require integration with live accounting data feeds (e.g., Sage 50 / QuickBooks APIs) for automated metric pulls.

## 6. AI Use & Contributions
* **AI Tools Used:** Google AI Studio (Gemini) was used to generate the initial HTML, Tailwind CSS, and JavaScript code scaffolding.
* **Human Oversight & Decisions:** The group defined all underlying financial formulas, independently verified calculation accuracy against financial principles, wrote custom input validation checks, and directed UI design refinements based on user testing.
