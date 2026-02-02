# Section 2: Credit Risk - RAROC Pricing Models

> **Navigation**: [Home](../../README.md) > [Sections](../README.md) > Section 2: Credit Risk

## 📌 Overview

This section focuses on credit risk management through Risk-Adjusted Return on Capital (RAROC) pricing models. You'll evaluate a corporate loan application using sophisticated financial modeling techniques to determine profitability and optimal pricing.

## 🎯 Objectives

1. Understand credit risk fundamentals and key metrics
2. Build amortization schedules for loan repayment analysis
3. Calculate RAROC to assess loan profitability
4. Optimize pricing using Goal Seek analysis
5. Perform sensitivity analysis on risk parameters
6. Make data-driven lending decisions

## 📖 Background

### What is Credit Risk?

Credit risk refers to the possibility that a borrower will fail to meet their contractual obligations to repay a loan or other credit facility. This is one of the most significant risks in banking because lending is a core activity.

**Impact of Default**:
- Direct financial losses
- Reduced profitability
- Capital adequacy impacts
- Regulatory concerns

### Key Credit Risk Metrics

#### Probability of Default (PD)
The likelihood that a client will fail to meet their loan obligations, typically defined as missing payments for 3 consecutive months.

```
PD = Number of Defaults / Total Number of Borrowers
```

#### Exposure at Default (EAD)
The total value the bank is exposed to at the time of default, including:
- Outstanding principal
- Accrued interest
- Fees and charges

```
EAD = Outstanding Balance + Accrued Interest + Fees
```

#### Loss Given Default (LGD)
The percentage of the EAD that the bank expects to lose after accounting for recoveries such as collateral or guarantees.

```
LGD = (EAD - Recoveries) / EAD × 100%
```

#### Expected Loss (EL)
```
Expected Loss = PD × EAD × LGD
```

### What is Risk-Based Pricing?

Risk-based pricing is a strategy where interest rates and terms offered to a borrower are determined based on their perceived credit risk.

**Key Principles**:
- Higher risk → Higher interest rates
- Lower risk → Lower interest rates
- Compensates bank for risk taken
- Aligns pricing with default probability

**Factors Considered**:
- Credit history
- Income and cash flow
- Debt-to-income ratio
- Collateral value
- Industry and market conditions

## 💼 Case Study: EnergiCore (Pty) Ltd

### Company Background

**EnergiCore (Pty) Ltd** is a corporate investment client requesting financing for a major sustainable industrial complex development.

**Project Description**:
- Manufacturing facilities
- Office spaces
- Renewable energy infrastructure
  - Solar panels on rooftops
  - Battery storage systems
  - Smart energy management systems

**Sustainability Goals**:
- Reduce carbon emissions
- Lower long-term energy costs
- Support industry sustainability objectives
- Improve operational efficiency

### Loan Structure

| Parameter | Value |
|-----------|-------|
| **Loan Amount** | R100,000,000 |
| **Loan Term** | 120 months (10 years) |
| **Interest Rate** | 13.75% per annum |
| **Initiation Fee** | R1,250,000 (once-off, paid in Month 1) |
| **Monthly Fee** | R12,500 |
| **Repayment Type** | Fully amortizing (principal + interest) |

## 📊 Tasks & Requirements

### Task 1.1: Risk Assessment

Assess the potential risks associated with the EnergiCore project:

**Market Risks**:
- Construction industry volatility
- Demand for industrial space
- Competition from existing facilities

**Economic Risks**:
- Economic downturn impacts
- Interest rate fluctuations
- Currency exchange rate impacts (if applicable)
- Inflation effects on construction costs

**Operational Risks**:
- Project delays
- Cost overruns
- Technology implementation challenges
- Contractor performance

**Sustainability Risks**:
- Renewable energy technology evolution
- Regulatory changes in green building standards
- Market acceptance of sustainable features

**Financial Risks**:
- Client cash flow adequacy
- Debt servicing capacity
- Covenant breaches

**Format**: Provide comprehensive written analysis in Excel workbook.

---

### Task 1.2: RAROC Calculation

Calculate the RAROC for the EnergiCore loan using the provided Excel template.

#### Step 1: Create Amortization Schedule

The amortization schedule shows how the loan is repaid over time through regular payments.

**Monthly Payment Formula**:
```
M = P × [r(1 + r)^n] / [(1 + r)^n - 1]
```

Where:
- M = Monthly payment
- P = Principal loan amount (opening balance)
- r = Interest rate / 12
- n = Total number of payments

**For Each Month, Calculate**:

1. **Interest Amount**:
```
Interest = Opening Balance × (Interest Rate / 12)
```

2. **Principal Payment**:
```
Principal = Monthly Payment - Interest Amount
```

3. **Closing Balance**:
```
Closing Balance = Opening Balance - Principal Payment
```

**Process**:
- Month 1: Opening Balance = R100,000,000
- Month 2: Opening Balance = Month 1 Closing Balance
- Continue for all 120 months
- Final Closing Balance should be ≈ R0

#### Step 2: Calculate Monthly Cash Flows

For each month in the pricing model:

**Net Interest Income (NII)**:
```
NII = Opening Balance × (Interest Rate - CoF) / 12
```
Where CoF (Cost of Funding) = Prime Rate

**Non-Interest Revenue (NIR)**:
```
NIR = Monthly Fee + (Initiation Fee in Month 1 only)
```

**Operating Income**:
```
Operating Income = NII + NIR
```

**Operating Expenses**:
```
Operating Expenses = Operating Income × Cost-to-Income Ratio
```

#### Step 3: Calculate Economic Capital (ECAP)

**Credit Risk ECAP**:
```
Credit Risk ECAP = EAD × (Cap Rate / 12) × Credit Risk Diversification Factor
```

**Business Risk ECAP**:
```
Business Risk ECAP = (NII + NIR) × Business Risk ECAP Multiplier
```

**Operational Risk ECAP**:
```
Operational Risk ECAP = (NII + NIR) × Operational Risk ECAP Multiplier
```

**Total ECAP**:
```
Total ECAP = Credit Risk ECAP + Business Risk ECAP + Operational Risk ECAP
```

#### Step 4: Calculate Risk-Adjusted Headline Earnings

```
Risk-Adjusted Headline Earnings = Operating Income - Total Expenses - Expected Loss
```

**Expected Loss**:
```
Expected Loss = PD × EAD × LGD
```

#### Step 5: Apply Discount Factor

```
Discount Factor = (1 + Risk Free Rate / 12)^(-months)
```

Apply discount factor to future cash flows to get present values.

#### Step 6: Calculate RAROC

```
RAROC = Risk-Adjusted Headline Earnings / Total ECAP
```

**Decision Rule**:
- RAROC > Hurdle Rate → Accept the loan
- RAROC < Hurdle Rate → Reject or renegotiate
- Typical Hurdle Rate: 15% for banks

#### Step 7: Calculate Economic Profit (EP)

```
EP = Risk-Adjusted Headline Earnings - Cost of Capital
```

Where:
```
Cost of Capital = Total ECAP × Hurdle Rate
```

---

### Task 1.3: Goal Seek - Target RAROC

**Objective**: Determine what interest rate should be charged to achieve a RAROC of 17%.

**Method**: Use Excel's Goal Seek function

**Steps**:
1. Create a copy of your EnergiCore pricing model
2. Go to Data → What-If Analysis → Goal Seek
3. Set Parameters:
   - **Set Cell**: RAROC cell
   - **To Value**: 17% (or 0.17)
   - **By Changing Cell**: Interest Rate cell
4. Click OK and record the result

**Analysis Questions**:
- What is the required interest rate?
- Is this rate competitive in the market?
- How much higher is it than the original 13.75%?
- What are the implications for client negotiations?

---

### Task 1.4: Goal Seek - Break-Even Point

**Objective**: Determine the interest rate needed to achieve an Economic Profit of R0.

**Method**: Use Excel's Goal Seek function

**Steps**:
1. Create another copy of your EnergiCore pricing model
2. Go to Data → What-If Analysis → Goal Seek
3. Set Parameters:
   - **Set Cell**: Economic Profit (EP) cell
   - **To Value**: 0
   - **By Changing Cell**: Interest Rate cell
4. Click OK and record the result

**Analysis Questions**:
- What is the break-even interest rate?
- How does this compare to the current rate (13.75%)?
- What does this tell us about our pricing margin?
- How would you use this result in negotiations?

**Practical Application**:
The break-even rate represents the minimum rate at which the bank should lend. Any rate below this results in negative economic profit. This is crucial for:
- Setting pricing floors
- Negotiation boundaries
- Risk assessment
- Portfolio management

---

### Task 1.5: Sensitivity Analysis - PD vs RAROC

**Objective**: Investigate how changes in Probability of Default (PD) affect RAROC.

**Method**: Scenario analysis with data visualization

**Steps**:

1. **Create Alternative PD Scenarios**
   - Generate 10 different PD values (all below 100%)
   - Example range: 0.5%, 1%, 2%, 5%, 10%, 15%, 20%, 30%, 50%, 75%
   - Or create team-specific scenarios based on risk appetite

2. **Calculate RAROC for Each PD**
   - Replace the current PD with each alternative value
   - Recalculate the entire pricing model
   - Record the resulting RAROC

3. **Create Data Table**

| PD (%) | RAROC (%) | Decision |
|--------|-----------|----------|
| 0.5    | ?         | ?        |
| 1.0    | ?         | ?        |
| 2.0    | ?         | ?        |
| ...    | ...       | ...      |

4. **Plot the Relationship**
   - X-axis: Probability of Default (PD)
   - Y-axis: RAROC
   - Create line chart or scatter plot
   - Add hurdle rate line (15%) for reference

5. **Interpret the Results**

**Analysis Questions**:
- What is the shape of the PD-RAROC curve?
- Is the relationship linear or non-linear?
- At what PD does RAROC fall below the hurdle rate?
- What is the rate of RAROC decline as PD increases?

**Implications**:

For **Pricing**:
- How should we adjust interest rates for different PD levels?
- What premium should high-risk clients pay?
- What is the maximum PD we can accept?

For **Risk Management**:
- How sensitive is profitability to credit quality deterioration?
- What PD threshold requires enhanced monitoring?
- How much risk buffer exists in current pricing?

For **Portfolio Management**:
- What is the optimal mix of PD levels?
- How should capital be allocated across risk segments?
- What are the concentration risk implications?

---

## 📦 Deliverables

### 1. Excel Workbook
**File Name**: `Group#_Sec2_Part1.xlsx`

**Required Worksheets**:
1. **Risk Assessment**: Written analysis of project risks
2. **Amortization Schedule**: 120-month repayment schedule
3. **Base Case Model**: Original RAROC calculation (13.75%)
4. **Goal Seek - 17% RAROC**: Model with target RAROC
5. **Goal Seek - Break-Even**: Model with EP = 0
6. **Sensitivity Analysis**: PD scenarios and RAROC results
7. **Charts**: PD-RAROC visualization

**Quality Requirements**:
- All formulas clearly documented
- Professional formatting
- Clear labels and headers
- Color coding for key outputs
- Summary dashboard (optional but recommended)

### 2. PowerPoint Presentation
**File Name**: `Group#_Sec2_Part2.pptx`

**Suggested Slide Structure**:
1. Title Slide
2. Case Study Overview
3. Risk Assessment Summary
4. RAROC Methodology
5. Base Case Results (13.75% rate)
6. Goal Seek Analysis - 17% RAROC Target
7. Goal Seek Analysis - Break-Even Point
8. Sensitivity Analysis - PD vs RAROC
9. Key Insights and Interpretation
10. Recommendations
11. Conclusion

**Presentation Tips**:
- Use clear visualizations
- Highlight key numbers
- Tell a story with your analysis
- Focus on business implications

### 3. Video Recording
**File Name**: `Group#_video2`

**Requirements**:
- Maximum 5 minutes
- All team members present
- Cameras on
- Screen share presentation
- Professional delivery

**Content Flow**:
1. Introduction (30 sec)
2. Risk assessment (45 sec)
3. RAROC calculation walkthrough (90 sec)
4. Goal Seek results (60 sec)
5. Sensitivity analysis insights (60 sec)
6. Conclusion and recommendation (45 sec)

---

## 🔑 Key Concepts Reference

### Time Value of Money
Money available now is worth more than the same amount in the future due to its earning potential.

### Discounting Cash Flows
Calculating the present value of future cash inflows/outflows by applying a discount rate.

```
PV = FV / (1 + r)^n
```

### Economic Profit (EP)
Net profit after accounting for all costs, including opportunity cost of capital.

```
EP = Return - (Capital × Cost of Capital)
```

### Hurdle Rate
Minimum rate of return required to justify an investment or loan. Acts as a filter for decision-making.

### Capital Adequacy
Banks must maintain sufficient capital to absorb losses. RAROC helps ensure capital is deployed efficiently.

## 🎯 Success Criteria

A successful Section 2 submission will:

1. ✅ Demonstrate accurate amortization calculations
2. ✅ Show correct RAROC methodology application
3. ✅ Present meaningful Goal Seek analysis
4. ✅ Provide insightful sensitivity analysis
5. ✅ Deliver clear business recommendations
6. ✅ Show strong quantitative skills
7. ✅ Present professionally

## 📚 Additional Resources

### Financial Modeling Best Practices
- Clear structure and layout
- Formula auditing
- Sensitivity tables
- Scenario comparisons
- Executive summaries

### Excel Functions to Master
- PMT: Calculate loan payments
- IPMT: Calculate interest portion
- PPMT: Calculate principal portion
- NPV: Net present value
- IRR: Internal rate of return
- Goal Seek: Optimization

### RAROC Industry Standards
- Typical hurdle rates: 12-18%
- Top-tier banks target: 15-20%
- Minimum acceptable: 10-12%

---

## 📚 See Also

- **[Section 1: Operational Risk](../section1_operational_risk/README.md)** - Employee attrition analysis
- **[Section 3: ESG Analysis](../section3_esg/README.md)** - Environmental, Social, and Governance comparison
- **[Reference Documentation](../../docs/README.md)** - Quick reference and concepts guide
- **[Deliverables](../../deliverables/README.md)** - View completed work

---

**Remember**: The goal is not just to calculate numbers, but to understand what they mean for lending decisions and how they align with the bank's risk appetite and profitability targets.
