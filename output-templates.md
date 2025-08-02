# Standardized Output Templates for Custom GPT

## Template Format
All Custom GPT outputs must follow this exact structure:

### Header
```
AI REVIEW RESULTS
Project Type: [ARR/IFM/Other]
Developer: [Developer Name]
Review Date: [YYYY-MM-DD]
Reviewer: AI Review Assistant
```

### Main Analysis Table
| Category | Criteria | Assessment | Score (1-5) | Comments | Recommendation |
|----------|----------|------------|-------------|----------|----------------|
| [Category Name] | [Specific Requirement] | [Brief Evaluation] | [1-5] | [Detailed Explanation] | [Action Item] |

### Summary Section
```
OVERALL ASSESSMENT
Overall Score: [X.X]/5.0
Overall Recommendation: [APPROVE/CONDITIONAL APPROVAL/NEEDS REVISION/REJECT]

TOP 3 CONCERNS:
1. [Specific concern with reference to criteria]
2. [Specific concern with reference to criteria]  
3. [Specific concern with reference to criteria]

TOP 3 STRENGTHS:
1. [Specific strength with reference to criteria]
2. [Specific strength with reference to criteria]
3. [Specific strength with reference to criteria]

NEXT STEPS:
- [Specific actionable recommendation]
- [Specific actionable recommendation]
- [Specific actionable recommendation]
```

## Sample Output: ARR Project

```
AI REVIEW RESULTS
Project Type: ARR
Developer: Piri
Review Date: 2024-01-15
Reviewer: AI Review Assistant

| Category | Criteria | Assessment | Score (1-5) | Comments | Recommendation |
|----------|----------|------------|-------------|----------|----------------|
| Technical | Technology Readiness | Established REDD+ methodology | 4 | Technology is proven with multiple successful deployments. Strong technical foundation. | Continue with current approach |
| Technical | Implementation Plan | Detailed 5-year roadmap provided | 3 | Plan covers major milestones but lacks specific risk mitigation strategies | Add detailed contingency planning |
| Financial | Revenue Model | Clear ARR projections | 4 | Strong revenue projections with conservative assumptions. Multiple revenue streams identified. | Validate pricing assumptions with market research |
| Financial | Cost Structure | Comprehensive cost analysis | 3 | Operating costs well-defined but capital requirements may be underestimated | Review capital expenditure projections |
| Environmental | Carbon Impact | Verified measurement methodology | 5 | Excellent use of satellite monitoring and ground truthing. Clear additionality demonstrated. | Maintain current monitoring protocols |
| Environmental | Biodiversity | Co-benefits documented | 4 | Strong biodiversity impact assessment with local species surveys completed. | Continue monitoring programs |
| Risk | Regulatory | Local permits secured | 3 | Key permits obtained but regulatory changes possible | Monitor regulatory environment actively |
| Risk | Operational | Risk register incomplete | 2 | Missing several operational risk categories including weather and political risks | Complete comprehensive risk assessment |

OVERALL ASSESSMENT
Overall Score: 3.5/5.0
Overall Recommendation: CONDITIONAL APPROVAL

TOP 3 CONCERNS:
1. Incomplete operational risk assessment missing weather and political risk analysis
2. Capital expenditure projections may be underestimated based on comparable projects
3. Regulatory environment monitoring needs strengthening

TOP 3 STRENGTHS:
1. Excellent carbon impact measurement methodology with satellite verification
2. Strong technical foundation using proven REDD+ methodology
3. Conservative financial projections with multiple revenue streams

NEXT STEPS:
- Complete comprehensive operational risk assessment within 30 days
- Validate capital expenditure projections with independent cost analysis
- Establish quarterly regulatory monitoring process
```

## Sample Output: IFM Project

```
AI REVIEW RESULTS
Project Type: IFM
Developer: [Developer Name]
Review Date: [Date]
Reviewer: AI Review Assistant

| Category | Criteria | Assessment | Score (1-5) | Comments | Recommendation |
|----------|----------|------------|-------------|----------|----------------|
| Technical | Forest Management Plan | FSC-certified management approach | 4 | Comprehensive plan following FSC standards with clear harvesting schedules | Maintain certification requirements |
| Technical | Monitoring Systems | Remote sensing + ground plots | 3 | Good monitoring framework but ground plot density below optimal | Increase plot sampling frequency |
| Financial | Revenue Projections | Timber + carbon revenue | 3 | Realistic timber pricing but carbon credit projections optimistic | Conservative carbon price modeling |
| Financial | Operating Costs | Detailed cost breakdown | 4 | Thorough analysis of all operational expenses with inflation adjustments | Continue current cost management |
| Environmental | Carbon Sequestration | Verified calculation methods | 4 | Strong carbon accounting using approved methodologies | Maintain current protocols |
| Environmental | Biodiversity Impact | Species impact assessment | 3 | Basic assessment completed but lacks long-term monitoring plan | Develop 10-year monitoring program |
| Risk | Market Risk | Timber market analysis | 2 | Limited market analysis, vulnerable to price volatility | Conduct comprehensive market study |
| Risk | Climate Risk | Climate resilience planning | 3 | Basic climate adaptation measures but needs enhancement | Strengthen climate resilience plan |

OVERALL ASSESSMENT
Overall Score: 3.3/5.0
Overall Recommendation: NEEDS REVISION

TOP 3 CONCERNS:
1. Limited timber market analysis leaves project vulnerable to price volatility
2. Carbon credit price projections appear optimistic compared to current market
3. Biodiversity monitoring plan lacks long-term sustainability framework

TOP 3 STRENGTHS:
1. FSC-certified forest management approach ensures sustainable practices
2. Comprehensive operational cost analysis with inflation adjustments
3. Strong carbon accounting methodology using verified calculation methods

NEXT STEPS:
- Conduct comprehensive timber market analysis including price sensitivity scenarios
- Revise carbon credit projections using conservative pricing assumptions
- Develop detailed 10-year biodiversity monitoring and management plan
```

## Scoring Guidelines

### Score Meanings:
- **5 - Exceptional**: Exceeds all requirements, best-in-class implementation
- **4 - Above Standard**: Meets all requirements with additional strengths
- **3 - Meets Standard**: Satisfies minimum requirements adequately
- **2 - Below Standard**: Partially meets requirements, needs improvement
- **1 - Poor**: Fails to meet basic requirements, major revision needed

### Overall Recommendation Guidelines:
- **APPROVE (4.0+ average)**: Project ready to proceed
- **CONDITIONAL APPROVAL (3.0-3.9 average)**: Proceed with specific conditions
- **NEEDS REVISION (2.0-2.9 average)**: Requires substantial improvements
- **REJECT (Below 2.0 average)**: Project not viable in current form

## Copy-Paste Ready Format
The final output should be easily copyable for use in next workflow steps. Ensure:
- Clean table formatting that preserves structure when copied
- Clear section headers
- Consistent spacing and alignment
- No special characters that might cause formatting issues