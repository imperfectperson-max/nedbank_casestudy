# Key Concepts & Definitions
## Nedbank QYF Virtual Internship 2025

This document provides comprehensive definitions of all key concepts used throughout the case study.

---

## 📊 Risk Management Fundamentals

### Risk
The possibility of loss or adverse outcomes resulting from various factors including internal failures, external events, or market conditions.

### Risk Management
The process of identification, assessment, and prioritization of risks followed by coordinated application of resources to minimize, monitor, and control the probability or impact of adverse events.

### Basel Framework
International regulatory standards developed by the Basel Committee on Banking Supervision to strengthen regulation, supervision, and risk management within the banking sector.

---

## 🔴 Operational Risk

### Operational Risk (Basel Definition)
The risk of loss resulting from inadequate or failed internal processes, people, and systems, or from external events that disrupt business operations.

**Examples**:
- Employee errors
- Fraud (internal and external)
- System failures
- Natural disasters
- Cybersecurity breaches
- Process breakdowns

### Operational Risk Types (Basel)

#### CPBP - Clients, Products and Business Practices
Losses from unintentional or negligent failure to meet professional obligations to clients, or from the nature or design of products.

#### DPA - Damage to Physical Assets
Losses from natural disasters or other events causing damage to physical assets.

#### EF - External Fraud
Losses due to acts of fraud, misappropriation of property, or circumvention of regulations by third parties.

#### IF - Internal Fraud
Losses due to acts of fraud, misappropriation of property, or circumvention of regulations involving at least one internal party.

### Operational Risk Capital
Capital that banks must allocate to cover potential operational risk losses, calculated using the Advanced Measurement Approach (AMA).

### Advanced Measurement Approach (AMA)
Sophisticated approach to calculating operational risk capital that uses internal loss data, scenario analysis, business environment factors, and internal control factors.

---

## 👥 Employee Attrition

### Attrition
The gradual reduction in workforce size through resignations, retirements, or other departures (not including terminations).

### Attrition Rate
```
Attrition Rate = (Number of Employees Who Left / Average Number of Employees) × 100%
```

### Types of Attrition

#### Voluntary Attrition
Employee chooses to leave the organization (resignation, retirement).

#### Involuntary Attrition
Organization terminates employment (layoffs, termination for cause).

#### Functional Attrition
Departure of underperforming employees (beneficial for organization).

#### Dysfunctional Attrition
Loss of high-performing, valuable employees (detrimental to organization).

### Institutional Knowledge
Accumulated understanding of systems, processes, clients, and organizational culture that exists within experienced employees.

### Turnover Cost
Total cost of replacing an employee, including recruitment, hiring, training, and productivity loss during transition.

---

## 💳 Credit Risk

### Credit Risk
The possibility that a borrower will fail to meet their contractual obligations to repay a loan or other credit facility.

### Default
Failure to meet the legal obligations or conditions of a loan, typically defined as missing 3+ consecutive payments.

### Probability of Default (PD)
The likelihood that a borrower will default on their debt obligations within a specific time period (usually 12 months).

```
PD = Number of Defaults / Total Number of Borrowers
```

### Exposure at Default (EAD)
The total value the bank is exposed to at the time a borrower defaults.

```
EAD = Outstanding Principal + Accrued Interest + Fees
```

### Loss Given Default (LGD)
The percentage of the exposure at default that the bank expects to lose after accounting for recoveries.

```
LGD = (EAD - Recoveries) / EAD × 100%
```

Where:
- Recoveries = Collateral value + Guarantees + Collections

### Expected Loss (EL)
The amount a bank statistically expects to lose on a loan.

```
Expected Loss = PD × EAD × LGD
```

**Example**:
- PD = 2%
- EAD = R1,000,000
- LGD = 40%
- EL = 0.02 × R1,000,000 × 0.40 = R8,000

### Unexpected Loss (UL)
Losses that exceed expected losses, covered by economic capital.

---

## 💰 Pricing & Profitability Concepts

### Risk-Based Pricing
Strategy where interest rates and loan terms are determined based on the borrower's creditworthiness and associated risk level.

**Principle**: Higher Risk → Higher Interest Rate

### Creditworthiness
Assessment of a borrower's ability and willingness to repay debt, based on:
- Credit history
- Income and cash flow
- Debt-to-income ratio
- Collateral
- Employment stability

### Prime Rate
The interest rate commercial banks charge their most creditworthy corporate customers. Used as a benchmark for many loan products.

### Cost of Funding (CoF)
The interest rate a bank pays to obtain funds, typically aligned with the prime rate.

### Spread
The difference between the interest rate charged to borrowers and the cost of funding.

```
Spread = Lending Rate - Cost of Funding
```

### Net Interest Income (NII)
Revenue generated from the difference between interest earned on loans and interest paid on deposits/funding.

```
NII = Interest Income - Interest Expense
```

Or in monthly pricing models:
```
NII = Opening Balance × (Interest Rate - CoF) / 12
```

### Non-Interest Revenue (NIR)
Income from sources other than interest, including:
- Fees (monthly, transaction, initiation)
- Service charges
- Commission income

### Operating Income
Total income before expenses.

```
Operating Income = Net Interest Income + Non-Interest Revenue
```

### Operating Expenses
Costs incurred in running the bank's operations, including:
- Salaries and benefits
- Technology and systems
- Occupancy costs
- Marketing and advertising

### Cost-to-Income Ratio
Efficiency metric showing operating expenses as a percentage of operating income.

```
Cost-to-Income Ratio = Operating Expenses / Operating Income
```

**Benchmark**: Lower is better; top banks target <50%

---

## 📈 Capital & Return Metrics

### Economic Capital (ECAP)
The amount of capital a bank determines it needs to hold to absorb unexpected losses at a certain confidence level.

**Components**:
1. **Credit Risk ECAP**: Capital for credit losses
2. **Business Risk ECAP**: Capital for revenue volatility
3. **Operational Risk ECAP**: Capital for operational failures

```
Total ECAP = Credit Risk ECAP + Business Risk ECAP + Operational Risk ECAP
```

### Capital Adequacy
Regulatory requirement ensuring banks hold sufficient capital to absorb losses and protect depositors.

### Risk-Adjusted Return on Capital (RAROC)
A risk-based profitability measurement framework that adjusts returns for the risks taken.

```
RAROC = Risk-Adjusted Return / Economic Capital
```

**Decision Rule**:
- RAROC > Hurdle Rate → Accept investment/loan
- RAROC < Hurdle Rate → Reject investment/loan

**Typical Benchmarks**:
- Excellent: >20%
- Good: 15-20%
- Acceptable: 12-15%
- Marginal: 10-12%
- Poor: <10%

### Risk-Adjusted Headline Earnings (RAHE)
Earnings after adjusting for expected losses and other risk factors.

```
RAHE = Operating Income - Operating Expenses - Expected Loss
```

### Hurdle Rate
The minimum rate of return required to justify an investment or loan, considering the associated risks.

**Also Known As**:
- Required rate of return
- Minimum acceptable rate
- Cost of capital
- Benchmark rate

**Purpose**: Acts as a threshold for investment decisions.

### Economic Profit (EP)
Profit after accounting for both explicit and implicit costs, including the opportunity cost of capital.

```
Economic Profit = RAHE - Cost of Capital
```

Where:
```
Cost of Capital = Total ECAP × Hurdle Rate
```

**Interpretation**:
- EP > 0: Creating value
- EP = 0: Break-even (covering cost of capital)
- EP < 0: Destroying value

### Return on Equity (ROE)
Traditional profitability metric.

```
ROE = Net Income / Shareholders' Equity × 100%
```

**RAROC vs ROE**:
- RAROC adjusts for risk
- ROE does not account for risk differences
- RAROC is more sophisticated for risk-based decisions

---

## 💱 Time Value of Money

### Time Value of Money
Fundamental financial principle: Money available now is worth more than the same amount in the future due to its earning potential.

**Reasons**:
1. Investment opportunity
2. Inflation erodes purchasing power
3. Risk of non-payment
4. Preference for liquidity

### Present Value (PV)
The current worth of a future sum of money or stream of cash flows, discounted at a specific rate.

```
PV = FV / (1 + r)^n
```

Where:
- FV = Future Value
- r = Discount rate
- n = Number of periods

### Future Value (FV)
The value of a current sum of money at a future date, given a specific rate of return.

```
FV = PV × (1 + r)^n
```

### Discounting
The process of determining the present value of future cash flows.

### Discount Rate
The interest rate used to discount future cash flows to present value. Reflects:
- Time value of money
- Risk premium
- Opportunity cost

### Discount Factor
The multiplier used to convert future cash flows to present value.

```
Discount Factor = 1 / (1 + r)^n
```

Or:
```
Discount Factor = (1 + r)^-n
```

**In Monthly Models**:
```
Discount Factor = (1 + Risk-Free Rate / 12)^-months
```

### Risk-Free Rate
The theoretical rate of return on an investment with zero risk, typically based on government bond yields.

**Purpose**: Baseline for calculating required returns on risky investments.

---

## 🏦 Loan Amortization

### Amortization
The process of paying off a loan through regular installments that cover both principal and interest.

### Fully Amortizing Loan
Loan that is completely paid off by the end of the term through regular payments.

### Amortization Schedule
A table showing each loan payment's breakdown into principal and interest, and the remaining balance.

**Columns**:
- Month
- Opening Balance
- Payment Amount
- Interest Portion
- Principal Portion
- Closing Balance

### Monthly Payment Formula
```
M = P × [r(1 + r)^n] / [(1 + r)^n - 1]
```

Where:
- M = Monthly payment
- P = Principal loan amount
- r = Monthly interest rate (annual rate / 12)
- n = Total number of payments

### Interest Portion
```
Interest = Opening Balance × (Annual Interest Rate / 12)
```

### Principal Portion
```
Principal = Monthly Payment - Interest
```

### Remaining Balance
```
Closing Balance = Opening Balance - Principal Payment
```

**Becomes next month's Opening Balance**

### Loan Term
The length of time until the loan is fully repaid.

**Common Terms**:
- Personal loans: 1-5 years (12-60 months)
- Home loans: 20-30 years (240-360 months)
- Business loans: 5-10 years (60-120 months)

---

## 🌍 Environmental, Social & Governance (ESG)

### ESG
Framework for evaluating a company's sustainability and ethical impact across three dimensions:
1. Environmental
2. Social
3. Governance

### Sustainability
Meeting present needs without compromising the ability of future generations to meet their own needs.

---

## 🌱 Environmental Pillar

### Carbon Emissions
Release of carbon dioxide (CO2) and other greenhouse gases into the atmosphere, contributing to climate change.

**Measured In**: Tons of CO2 equivalent (CO2e)

### Carbon Footprint
Total greenhouse gas emissions caused directly and indirectly by an individual, organization, or product.

### Net-Zero
Achieving a balance between carbon emissions produced and carbon removed from the atmosphere.

**Target**: Most organizations aim for 2030-2050

### Renewable Energy
Energy from sources that are naturally replenishing:
- Solar power
- Wind power
- Hydroelectric power
- Geothermal energy

### Renewable Energy Usage
Percentage of total energy consumption from renewable sources.

```
Renewable % = Renewable Energy / Total Energy Consumption × 100%
```

### Green Bonds
Fixed-income instruments specifically earmarked to raise money for climate and environmental projects.

### Green Financing
Lending and investment activities that promote environmental sustainability.

### Climate Risk
Financial risks from climate change, including:
- **Physical Risk**: Direct damage from weather events
- **Transition Risk**: Changes in policy, technology, market
- **Liability Risk**: Legal claims for climate damage

---

## 👥 Social Pillar

### Diversity
Representation of different groups within an organization based on:
- Gender
- Race and ethnicity
- Age
- Disability status
- Sexual orientation
- Religion

### Inclusion
Creating an environment where all individuals feel welcomed, respected, valued, and able to participate fully.

### Workforce Diversity Metrics
```
Women % = Number of Female Employees / Total Employees × 100%
Minority % = Number of Minority Employees / Total Employees × 100%
```

### Corporate Social Responsibility (CSR)
Company's commitment to operate ethically and contribute to economic development while improving quality of life for workforce, community, and society.

### CSR Investment Ratio
```
CSR Ratio = CSR Spending / Annual Profits × 100%
```

**Typical Ranges**: 1-3% of profits

### Employee Wellness Programs
Initiatives to support physical, mental, and financial health of employees:
- Health screenings
- Mental health support
- Fitness programs
- Financial education

### Professional Development
Ongoing education and training to enhance employee skills and career growth:
- Technical training
- Leadership development
- Certifications and qualifications
- Mentorship programs

---

## ⚖️ Governance Pillar

### Board Diversity
Variety in board composition across dimensions like gender, race, professional background, and expertise.

```
Board Diversity = Diverse Board Members / Total Board Members × 100%
```

**Best Practice**: Aim for 30-40% minimum diverse representation

### Independent Directors
Board members with no material financial or personal relationship with the company, providing objective oversight.

### Cybersecurity
Protection of computer systems, networks, and data from digital attacks, damage, or unauthorized access.

**Key Elements**:
- Encryption
- Access controls
- Threat monitoring
- Incident response
- Regular updates

### Data Privacy
Practices and policies governing collection, use, storage, and sharing of personal information.

**Regulations**: POPIA (South Africa), GDPR (EU), CCPA (California)

### Whistleblower Program
System allowing employees to report unethical behavior, violations, or illegal activities without fear of retaliation.

**Components**:
- Anonymous reporting channels
- Protection against retaliation
- Investigation procedures
- Corrective action processes

### Compliance
Adherence to laws, regulations, standards, and ethical practices relevant to the organization.

### Risk Management Framework
Structured approach to identifying, assessing, monitoring, and mitigating risks.

**Components**:
1. Risk identification
2. Risk assessment
3. Risk response
4. Risk monitoring
5. Risk reporting

### Internal Controls
Processes and procedures to ensure:
- Financial reporting accuracy
- Operational efficiency
- Compliance with laws
- Asset protection

---

## 📊 ESG Performance Measurement

### ESG Score
Composite rating of a company's ESG performance, typically on a scale (e.g., 0-100).

**Calculation Methods**:
- Weighted average of E, S, G scores
- Third-party ratings (MSCI, Sustainalytics)
- Custom internal scoring

### ESG Materiality
Issues that are most significant to a company's business and stakeholders.

**Varies By**:
- Industry
- Geography
- Business model
- Stakeholder priorities

### Greenwashing
Misleading marketing that portrays a company as more environmentally friendly than it actually is.

**Red Flags**:
- Vague claims
- Lack of evidence
- Overemphasis on minor initiatives
- Ignoring significant negative impacts

---

## 🔬 Analysis Techniques

### Comparative Analysis
Systematic comparison of two or more entities across multiple dimensions.

**Steps**:
1. Define comparison criteria
2. Collect data
3. Standardize metrics
4. Compare and contrast
5. Draw conclusions

### Sensitivity Analysis
Examination of how changes in input variables affect output results.

**Purpose**:
- Understand relationships
- Identify key drivers
- Assess risk
- Support decision-making

**Example**: How does RAROC change as PD increases?

### Scenario Analysis
Evaluation of outcomes under different potential future situations.

**Types**:
- Base case
- Best case
- Worst case
- Custom scenarios

### Goal Seek
Excel tool that determines the input value needed to achieve a desired output.

**Use Cases**:
- Finding break-even point
- Determining target pricing
- Optimizing returns

**Steps**:
1. Data → What-If Analysis → Goal Seek
2. Set cell: Output to target
3. To value: Desired result
4. By changing cell: Input to adjust

---

## 📈 Financial Formulas Summary

### Loan Payment
```
M = P × [r(1 + r)^n] / [(1 + r)^n - 1]
```

### Net Interest Income
```
NII = Opening Balance × (Interest Rate - CoF) / 12
```

### Operating Income
```
Operating Income = NII + NIR
```

### Expected Loss
```
EL = PD × EAD × LGD
```

### Economic Capital
```
Total ECAP = Credit Risk ECAP + Business Risk ECAP + Operational Risk ECAP
```

### Risk-Adjusted Headline Earnings
```
RAHE = Operating Income - Operating Expenses - Expected Loss
```

### RAROC
```
RAROC = RAHE / Total ECAP × 100%
```

### Economic Profit
```
EP = RAHE - (Total ECAP × Hurdle Rate)
```

### Discount Factor
```
Discount Factor = (1 + Risk-Free Rate / 12)^-months
```

---

## 🎯 Decision Frameworks

### RAROC Decision Rule
```
IF RAROC > Hurdle Rate:
    Accept loan/investment
ELSE IF RAROC < Hurdle Rate:
    Reject or renegotiate
ELSE IF RAROC = Hurdle Rate:
    Break-even point
```

### Economic Profit Decision Rule
```
IF EP > 0:
    Creating value → Proceed
ELSE IF EP = 0:
    Break-even → Marginal
ELSE IF EP < 0:
    Destroying value → Reject
```

### ESG Investment Decision
Consider:
1. Financial returns (RAROC, EP)
2. ESG impact (E, S, G scores)
3. Strategic alignment
4. Stakeholder expectations
5. Regulatory requirements
6. Competitive positioning

---

This comprehensive reference should support your understanding and analysis throughout all three sections of the case study.
