# Investment Management Cognitive Architecture Setup Guide

**INSTRUCTIONS FOR GITHUB COPILOT**: This file contains complete setup instructions for implementing the Self-Learning Vibe Coding cognitive memory architecture optimized for investment management, including portfolio analysis, risk assessment, financial modeling, market research, and comprehensive investment strategy development.

## 💰 Investment Management Automated Setup Protocol

**Execute these steps in order to establish a complete cognitive architecture system for investment management:**

### Step 1: VS Code Configuration (Required)

Add these settings to VS Code `settings.json`:

```json
{
  "github.copilot.chat.codeGeneration.useInstructionFiles": true,
  "chat.promptFiles": true,
  "chat.instructionsFilesLocations": [".github/instructions"],
  "files.associations": {
    "*.portfolio": "json",
    "*.analysis": "markdown",
    "*.model": "json",
    "*.strategy": "markdown",
    "*.research": "markdown",
    "*.valuation": "json",
    "*.risk": "json",
    "*.performance": "json",
    "*.allocation": "json",
    "*.screening": "json",
    "*.backtest": "json"
  },
  "search.exclude": {
    "**/confidential-research/**": true,
    "**/proprietary-models/**": true,
    "**/insider-info/**": true
  },
  "files.watcherExclude": {
    "**/confidential-research/**": true,
    "**/proprietary-models/**": true,
    "**/insider-info/**": true
  },
  "editor.rulers": [80, 120],
  "editor.wordWrap": "wordWrapColumn",
  "editor.wordWrapColumn": 80,
  "json.schemas": [
    {
      "fileMatch": ["*.portfolio", "*.model", "*.valuation"],
      "schema": {
        "type": "object",
        "properties": {
          "timestamp": {"type": "string"},
          "version": {"type": "string"},
          "data": {"type": "object"}
        }
      }
    }
  ],
  "markdown.extension.toc.levels": "2..6",
  "markdown.extension.completion.enabled": true
}
```

**Access settings.json**: `Ctrl+Shift+P` → "Preferences: Open User Settings (JSON)"

### Step 2: Create Investment Management Directory Structure

Create this exact folder structure in the project root:

```
project-root/
├── .github/
│   ├── copilot-instructions.md          # Global Investment Management Memory
│   ├── instructions/                    # Investment Management Procedural Memory
│   │   ├── investment-management.instructions.md
│   │   ├── portfolio-analysis.instructions.md
│   │   ├── risk-assessment.instructions.md
│   │   ├── financial-modeling.instructions.md
│   │   ├── market-research.instructions.md
│   │   ├── security-analysis.instructions.md
│   │   ├── asset-allocation.instructions.md
│   │   ├── performance-measurement.instructions.md
│   │   ├── quantitative-analysis.instructions.md
│   │   ├── alternative-investments.instructions.md
│   │   ├── derivatives-trading.instructions.md
│   │   ├── esg-investing.instructions.md
│   │   ├── behavioral-finance.instructions.md
│   │   ├── regulatory-compliance.instructions.md
│   │   ├── client-management.instructions.md
│   │   ├── technology-integration.instructions.md
│   │   ├── learning.instructions.md     # Meta-Cognitive Learning
│   │   └── meta-cognition.instructions.md  # Self-Monitoring
│   └── prompts/                         # Investment Management Episodic Memory
│       ├── portfolio-construction.prompt.md
│       ├── investment-research.prompt.md
│       ├── risk-analysis.prompt.md
│       ├── market-analysis.prompt.md
│       ├── security-valuation.prompt.md
│       ├── strategy-development.prompt.md
│       ├── performance-review.prompt.md
│       ├── due-diligence.prompt.md
│       ├── rebalancing.prompt.md
│       ├── scenario-analysis.prompt.md
│       ├── client-reporting.prompt.md
│       ├── investment-committee.prompt.md
│       ├── compliance-review.prompt.md
│       ├── manager-selection.prompt.md
│       ├── consolidation.prompt.md
│       ├── self-assessment.prompt.md    # Meta-Cognitive Assessment
│       ├── meta-learning.prompt.md      # Learning Strategy Evolution
│       └── cognitive-health.prompt.md   # Architecture Maintenance
├── portfolios/
│   ├── institutional/                   # Institutional portfolios
│   │   ├── pension-funds/
│   │   ├── endowments/
│   │   ├── sovereign-wealth/
│   │   ├── insurance/
│   │   └── corporate/
│   ├── retail/                          # Retail portfolios
│   │   ├── high-net-worth/
│   │   ├── mass-affluent/
│   │   ├── retirement/
│   │   ├── college-savings/
│   │   └── taxable-accounts/
│   ├── strategies/                      # Investment strategies
│   │   ├── growth/
│   │   ├── value/
│   │   ├── income/
│   │   ├── balanced/
│   │   ├── conservative/
│   │   ├── aggressive/
│   │   └── alternative/
│   ├── allocations/                     # Asset allocations
│   │   ├── strategic/
│   │   ├── tactical/
│   │   ├── dynamic/
│   │   └── risk-parity/
│   └── benchmarks/                      # Performance benchmarks
│       ├── market-indices/
│       ├── peer-groups/
│       ├── custom-benchmarks/
│       └── liability-benchmarks/
├── research/
│   ├── market-analysis/                 # Market research
│   │   ├── macroeconomic/
│   │   ├── sector-analysis/
│   │   ├── regional-analysis/
│   │   ├── thematic-research/
│   │   └── market-outlook/
│   ├── security-analysis/               # Individual security research
│   │   ├── equity-research/
│   │   │   ├── fundamental/
│   │   │   ├── technical/
│   │   │   ├── quantitative/
│   │   │   └── screening/
│   │   ├── fixed-income/
│   │   │   ├── credit-analysis/
│   │   │   ├── duration-analysis/
│   │   │   ├── yield-curve/
│   │   │   └── municipal-bonds/
│   │   ├── alternatives/
│   │   │   ├── real-estate/
│   │   │   ├── commodities/
│   │   │   ├── hedge-funds/
│   │   │   ├── private-equity/
│   │   │   └── infrastructure/
│   │   └── derivatives/
│   │       ├── options/
│   │       ├── futures/
│   │       ├── swaps/
│   │       └── structured-products/
│   ├── manager-research/                # Investment manager analysis
│   │   ├── due-diligence/
│   │   ├── performance-analysis/
│   │   ├── risk-analysis/
│   │   ├── operational-review/
│   │   └── fee-analysis/
│   └── economic-research/               # Economic analysis
│       ├── indicators/
│       ├── forecasts/
│       ├── policy-analysis/
│       ├── inflation-analysis/
│       └── currency-analysis/
├── models/
│   ├── valuation/                       # Valuation models
│   │   ├── dcf-models/
│   │   ├── relative-valuation/
│   │   ├── option-pricing/
│   │   ├── bond-pricing/
│   │   └── real-estate-valuation/
│   ├── risk/                            # Risk models
│   │   ├── var-models/
│   │   ├── stress-testing/
│   │   ├── scenario-analysis/
│   │   ├── correlation-models/
│   │   └── factor-models/
│   ├── optimization/                    # Portfolio optimization
│   │   ├── mean-variance/
│   │   ├── black-litterman/
│   │   ├── risk-parity/
│   │   ├── minimum-variance/
│   │   └── robust-optimization/
│   ├── performance/                     # Performance models
│   │   ├── attribution/
│   │   ├── benchmarking/
│   │   ├── risk-adjusted/
│   │   └── timing-models/
│   └── forecasting/                     # Forecasting models
│       ├── return-forecasts/
│       ├── volatility-forecasts/
│       ├── economic-forecasts/
│       └── earnings-forecasts/
├── analytics/
│   ├── performance/                     # Performance analytics
│   │   ├── returns/
│   │   ├── risk-metrics/
│   │   ├── attribution/
│   │   ├── benchmarking/
│   │   └── peer-comparison/
│   ├── risk/                            # Risk analytics
│   │   ├── portfolio-risk/
│   │   ├── concentration-risk/
│   │   ├── liquidity-risk/
│   │   ├── credit-risk/
│   │   └── operational-risk/
│   ├── attribution/                     # Performance attribution
│   │   ├── sector-attribution/
│   │   ├── security-selection/
│   │   ├── asset-allocation/
│   │   ├── currency-attribution/
│   │   └── style-attribution/
│   ├── screening/                       # Investment screening
│   │   ├── fundamental-screens/
│   │   ├── technical-screens/
│   │   ├── quantitative-screens/
│   │   ├── esg-screens/
│   │   └── custom-screens/
│   └── backtesting/                     # Strategy backtesting
│       ├── historical-analysis/
│       ├── simulation/
│       ├── sensitivity-analysis/
│       ├── monte-carlo/
│       └── walk-forward/
├── data/
│   ├── market-data/                     # Market data feeds
│   │   ├── prices/
│   │   ├── volumes/
│   │   ├── fundamentals/
│   │   ├── estimates/
│   │   └── corporate-actions/
│   ├── economic-data/                   # Economic indicators
│   │   ├── gdp/
│   │   ├── inflation/
│   │   ├── employment/
│   │   ├── interest-rates/
│   │   └── monetary-policy/
│   ├── alternative-data/                # Alternative data sources
│   │   ├── satellite-data/
│   │   ├── social-sentiment/
│   │   ├── credit-card-data/
│   │   ├── supply-chain/
│   │   └── esg-data/
│   ├── reference-data/                  # Reference data
│   │   ├── security-master/
│   │   ├── exchange-data/
│   │   ├── calendar-data/
│   │   ├── classification/
│   │   └── benchmarks/
│   └── proprietary/                     # Proprietary data
│       ├── research-ratings/
│       ├── model-outputs/
│       ├── client-data/
│       └── internal-estimates/
├── tools/
│   ├── portfolio-management/            # Portfolio management tools
│   │   ├── order-management/
│   │   ├── trade-execution/
│   │   ├── rebalancing/
│   │   ├── tax-optimization/
│   │   └── cash-management/
│   ├── analytics-platforms/             # Analytics platforms
│   │   ├── bloomberg/
│   │   ├── factset/
│   │   ├── refinitiv/
│   │   ├── morningstar/
│   │   └── custom-analytics/
│   ├── risk-management/                 # Risk management tools
│   │   ├── risk-monitoring/
│   │   ├── limit-monitoring/
│   │   ├── stress-testing/
│   │   ├── scenario-analysis/
│   │   └── compliance-monitoring/
│   ├── research-tools/                  # Research tools
│   │   ├── screening-tools/
│   │   ├── charting-tools/
│   │   ├── modeling-tools/
│   │   ├── backtesting-tools/
│   │   └── data-visualization/
│   └── reporting/                       # Reporting tools
│       ├── client-reporting/
│       ├── regulatory-reporting/
│       ├── internal-reporting/
│       ├── performance-reporting/
│       └── risk-reporting/
├── compliance/
│   ├── regulatory/                      # Regulatory compliance
│   │   ├── sec-filings/
│   │   ├── cftc-reporting/
│   │   ├── finra-compliance/
│   │   ├── mifid-compliance/
│   │   └── gdpr-compliance/
│   ├── policies/                        # Investment policies
│   │   ├── investment-policy/
│   │   ├── risk-policy/
│   │   ├── trading-policy/
│   │   ├── proxy-voting/
│   │   └── ethics-policy/
│   ├── procedures/                      # Compliance procedures
│   │   ├── trade-surveillance/
│   │   ├── best-execution/
│   │   ├── conflicts-of-interest/
│   │   ├── personal-trading/
│   │   └── record-keeping/
│   └── monitoring/                      # Compliance monitoring
│       ├── limit-monitoring/
│       ├── position-monitoring/
│       ├── concentration-monitoring/
│       ├── liquidity-monitoring/
│       └── performance-monitoring/
└── docs/
    ├── investment-policy/               # Investment documentation
    │   ├── investment-objectives/
    │   ├── risk-tolerance/
    │   ├── benchmark-policy/
    │   ├── asset-allocation/
    │   └── rebalancing-policy/
    ├── procedures/                      # Investment procedures
    │   ├── research-process/
    │   ├── portfolio-construction/
    │   ├── trade-execution/
    │   ├── performance-measurement/
    │   └── risk-management/
    ├── reports/                         # Investment reports
    │   ├── quarterly-reviews/
    │   ├── annual-reports/
    │   ├── performance-reports/
    │   ├── risk-reports/
    │   └── research-reports/
    ├── training/                        # Investment training
    │   ├── analyst-training/
    │   ├── portfolio-manager-training/
    │   ├── compliance-training/
    │   ├── technology-training/
    │   └── continuing-education/
    └── templates/                       # Document templates
        ├── research-templates/
        ├── presentation-templates/
        ├── report-templates/
        ├── memo-templates/
        └── analysis-templates/
```

### Step 3: Global Investment Management Declarative Memory Setup

**Create `.github/copilot-instructions.md`** with this exact content:

```markdown
# Self-Learning Vibe Coding - Investment Management Cognitive Architecture

IMPORTANT: This file serves as Global Investment Management Declarative Memory. Optimized for portfolio analysis, risk assessment, financial modeling, market research, and comprehensive investment strategy development.

## 🧠 Investment Management Cognitive Architecture Status

**Working Memory**: 4/4 rules (at optimal capacity for investment management)
**Consolidation**: Auto-trigger when exceeding capacity
**Memory Distribution**: Active across investment management procedural (.instructions.md) and investment strategy episodic (.prompt.md) systems

## 💰 Investment Management Working Memory - Quick Reference (Limit: 4 Critical Rules)

| Priority | Rule | Load | Auto-Consolidate |
|----------|------|------|------------------|
| P1 | `@fiduciary-duty` - Always act in the best interests of clients and maintain the highest ethical standards | Low | Never |
| P2 | `@risk-first` - Assess and manage risk comprehensively before pursuing returns | Medium | >30 days unused |
| P3 | `@meditation` - Auto-consolidate when working memory capacity exceeded | High | When triggered |
| P4 | `@evidence-based` - Base all investment decisions on rigorous analysis and empirical evidence | Medium | When obsolete |

## 🎯 Investment Management Cognitive Architecture Coordination

### Investment Management Procedural Memory Activation (Context-Dependent):
- `investment-management.instructions.md` → General investment for .portfolio, .analysis, .strategy files
- `portfolio-analysis.instructions.md` → Portfolio analysis for .portfolio, .allocation, .performance files
- `risk-assessment.instructions.md` → Risk assessment for .risk, .var, .stress files
- `financial-modeling.instructions.md` → Financial modeling for .model, .valuation, .backtest files
- `market-research.instructions.md` → Market research for .research, *market*, *sector* files
- `security-analysis.instructions.md` → Security analysis for *equity*, *bond*, *security* files
- `asset-allocation.instructions.md` → Asset allocation for .allocation, *strategic*, *tactical* files
- `performance-measurement.instructions.md` → Performance for .performance, *attribution*, *benchmark* files
- `quantitative-analysis.instructions.md` → Quantitative for *quant*, *factor*, *algorithm* files
- `alternative-investments.instructions.md` → Alternatives for *alternative*, *private*, *hedge* files
- `derivatives-trading.instructions.md` → Derivatives for *option*, *future*, *swap* files
- `esg-investing.instructions.md` → ESG for *esg*, *sustainable*, *impact* files
- `behavioral-finance.instructions.md` → Behavioral for *behavioral*, *psychology*, *bias* files
- `regulatory-compliance.instructions.md` → Compliance for *compliance*, *regulatory*, *sec* files
- `client-management.instructions.md` → Client management for *client*, *relationship*, *service* files
- `technology-integration.instructions.md` → Technology for *fintech*, *robo*, *ai* files
- `learning.instructions.md` → Meta-cognitive learning for *instructions*, *learning* files
- `meta-cognition.instructions.md` → Self-awareness for *meta*, *monitor*, *assess* files

### Investment Management Episodic Memory Activation (Investment Strategy Workflows):
- `portfolio-construction.prompt.md` → Portfolio construction and optimization
- `investment-research.prompt.md` → Investment research and due diligence
- `risk-analysis.prompt.md` → Risk analysis and stress testing
- `market-analysis.prompt.md` → Market analysis and outlook development
- `security-valuation.prompt.md` → Security valuation and analysis
- `strategy-development.prompt.md` → Investment strategy development
- `performance-review.prompt.md` → Performance review and attribution
- `due-diligence.prompt.md` → Investment due diligence processes
- `rebalancing.prompt.md` → Portfolio rebalancing and optimization
- `scenario-analysis.prompt.md` → Scenario analysis and stress testing
- `client-reporting.prompt.md` → Client reporting and communication
- `investment-committee.prompt.md` → Investment committee processes
- `compliance-review.prompt.md` → Compliance review and monitoring
- `manager-selection.prompt.md` → Investment manager selection and monitoring
- `consolidation.prompt.md` → Investment management memory optimization
- `self-assessment.prompt.md` → Investment management performance evaluation
- `meta-learning.prompt.md` → Investment management strategy evolution
- `cognitive-health.prompt.md` → Investment management architecture maintenance

### Investment Management Auto-Consolidation Triggers

- Working memory > 4 rules → Execute consolidation.prompt.md
- Fiduciary duty conflicts detected → Activate ethical decision-making protocols
- Risk limit breaches detected → Review and redistribute risk management memory load
- User requests meditation → Full investment management cognitive architecture optimization
- **Investment management performance assessment needed → Execute self-assessment.prompt.md**
- **Investment management strategy evolution required → Execute meta-learning.prompt.md**
- **Investment management architecture health check → Execute cognitive-health.prompt.md**

## 🔄 Investment Management Memory Transfer Protocol

**Immediate Transfer**: Critical fiduciary duty issues → Quick Reference (P1-P4)
**Gradual Consolidation**: Repeated investment processes → Investment management procedural memory (.instructions.md)
**Complex Investment Workflows**: Multi-asset strategies → Investment strategy episodic memory (.prompt.md)
**Archive Management**: Obsolete investment management patterns → Historical storage in specialized files
**Index Maintenance**: Auto-update Investment Management Long-Term Memory Index during transfers

## 📚 Investment Management Long-Term Memory Index

### Investment Management Procedural Memory Store (.github/instructions/)
| File | Domain | Activation Pattern | Last Updated |
|------|--------|-------------------|--------------|
| investment-management.instructions.md | General Investment Management | *.portfolio, *.analysis, *.strategy | Auto-tracked |
| portfolio-analysis.instructions.md | Portfolio Analysis | *.portfolio, *.allocation, *.performance | Auto-tracked |
| risk-assessment.instructions.md | Risk Assessment | *.risk, *.var, *.stress | Auto-tracked |
| financial-modeling.instructions.md | Financial Modeling | *.model, *.valuation, *.backtest | Auto-tracked |
| market-research.instructions.md | Market Research | *.research, *market*, *sector* | Auto-tracked |
| security-analysis.instructions.md | Security Analysis | *equity*, *bond*, *security* | Auto-tracked |
| asset-allocation.instructions.md | Asset Allocation | *.allocation, *strategic*, *tactical* | Auto-tracked |
| performance-measurement.instructions.md | Performance Measurement | *.performance, *attribution*, *benchmark* | Auto-tracked |
| quantitative-analysis.instructions.md | Quantitative Analysis | *quant*, *factor*, *algorithm* | Auto-tracked |
| alternative-investments.instructions.md | Alternative Investments | *alternative*, *private*, *hedge* | Auto-tracked |
| derivatives-trading.instructions.md | Derivatives Trading | *option*, *future*, *swap* | Auto-tracked |
| esg-investing.instructions.md | ESG Investing | *esg*, *sustainable*, *impact* | Auto-tracked |
| behavioral-finance.instructions.md | Behavioral Finance | *behavioral*, *psychology*, *bias* | Auto-tracked |
| regulatory-compliance.instructions.md | Regulatory Compliance | *compliance*, *regulatory*, *sec* | Auto-tracked |
| client-management.instructions.md | Client Management | *client*, *relationship*, *service* | Auto-tracked |
| technology-integration.instructions.md | Technology Integration | *fintech*, *robo*, *ai* | Auto-tracked |
| learning.instructions.md | Meta-Learning | *instructions*, *learning* | Auto-tracked |
| meta-cognition.instructions.md | Self-Monitoring | *meta*, *monitor*, *assess* | Auto-tracked |

### Investment Management Episodic Memory Store (.github/prompts/)
| File | Investment Management Workflow | Complexity Level | Usage Frequency |
|------|--------------------------------|------------------|-----------------|
| portfolio-construction.prompt.md | Portfolio Construction | High | Auto-tracked |
| investment-research.prompt.md | Investment Research | High | Auto-tracked |
| risk-analysis.prompt.md | Risk Analysis | High | Auto-tracked |
| market-analysis.prompt.md | Market Analysis | Medium | Auto-tracked |
| security-valuation.prompt.md | Security Valuation | High | Auto-tracked |
| strategy-development.prompt.md | Strategy Development | High | Auto-tracked |
| performance-review.prompt.md | Performance Review | Medium | Auto-tracked |
| due-diligence.prompt.md | Due Diligence | High | Auto-tracked |
| rebalancing.prompt.md | Portfolio Rebalancing | Medium | Auto-tracked |
| scenario-analysis.prompt.md | Scenario Analysis | High | Auto-tracked |
| client-reporting.prompt.md | Client Reporting | Medium | Auto-tracked |
| investment-committee.prompt.md | Investment Committee | Medium | Auto-tracked |
| compliance-review.prompt.md | Compliance Review | Medium | Auto-tracked |
| manager-selection.prompt.md | Manager Selection | High | Auto-tracked |
| consolidation.prompt.md | Memory Optimization | High | Auto-tracked |
| self-assessment.prompt.md | Performance Evaluation | High | Auto-tracked |
| meta-learning.prompt.md | Strategy Evolution | High | Auto-tracked |
| cognitive-health.prompt.md | Health Monitoring | Medium | Auto-tracked |

### Investment Management Memory Transfer Protocol Status
- **Active Files**: 36 specialized investment management memory files (18 procedural + 18 episodic)
- **Last Consolidation**: Investment management architecture initialization with meta-cognitive enhancements
- **Cognitive Load Status**: Optimized for comprehensive portfolio management and fiduciary responsibility
- **Index Synchronization**: Maintained automatically during consolidation
- **Meta-Cognitive Status**: Fully operational with investment management performance assessment and strategy evolution

---

*Global Investment Management Declarative Memory Component - Coordinates distributed investment management cognitive architecture while maintaining optimal investment decision-making efficiency. Detailed investment management protocols reside in specialized memory files.*
```

### Step 4: Investment Management Procedural Memory Files

#### Create `.github/instructions/investment-management.instructions.md`:

```markdown
---
applyTo: "**/*.portfolio,**/*.analysis,**/*.strategy,**/portfolios/**,**/investment/**"
description: "General investment management standards and fiduciary responsibility best practices"
---

# Investment Management Procedural Memory

## Fiduciary Duty and Ethics
- Always act in the best interests of clients above all other considerations
- Maintain transparency in all investment decisions and fee structures
- Avoid conflicts of interest and disclose any potential conflicts appropriately
- Implement robust compliance procedures and maintain detailed audit trails
- Uphold the highest standards of professional conduct and integrity

## Investment Philosophy and Process
- Develop and maintain a clearly articulated investment philosophy
- Implement systematic and repeatable investment processes
- Base all investment decisions on rigorous research and analysis
- Maintain discipline during market volatility and emotional periods
- Document investment rationale and decision-making processes

## Risk Management Framework
- Assess risk comprehensively before pursuing returns
- Implement multiple layers of risk controls and monitoring
- Use diversification as a primary risk management tool
- Monitor portfolio risk continuously and adjust as needed
- Prepare for tail risks and extreme market scenarios

## Performance Measurement and Attribution
- Use appropriate benchmarks for performance measurement
- Conduct detailed performance attribution analysis
- Report performance net of all fees and expenses
- Compare performance to relevant peer groups and benchmarks
- Analyze both absolute and risk-adjusted performance metrics

## Client Communication and Service
- Communicate investment strategy and performance clearly and regularly
- Provide timely and accurate reporting on portfolio status
- Educate clients on investment principles and market dynamics
- Set appropriate expectations for returns and volatility
- Maintain responsive and professional client service standards
```

#### Create `.github/instructions/portfolio-analysis.instructions.md`:

```markdown
---
applyTo: "**/*.portfolio,**/*.allocation,**/*.performance,**/portfolios/**"
description: "Portfolio analysis methodology and construction best practices"
---

# Portfolio Analysis Procedural Memory

## Portfolio Construction Principles
- Begin with clear investment objectives and constraints
- Use strategic asset allocation as the foundation for portfolio construction
- Implement appropriate diversification across asset classes, geographies, and sectors
- Consider liquidity needs and time horizon in asset selection
- Balance risk and return expectations with client goals and constraints

## Asset Allocation Framework
- Develop strategic asset allocation based on long-term capital market assumptions
- Implement tactical asset allocation adjustments based on market conditions
- Use mean reversion and momentum signals appropriately in allocation decisions
- Consider alternative investments for enhanced diversification
- Rebalance portfolios systematically to maintain target allocations

## Security Selection Process
- Use fundamental analysis as the primary basis for security selection
- Supplement fundamental analysis with quantitative and technical factors
- Consider valuation, quality, and momentum factors in security selection
- Implement appropriate screening processes for ESG and other criteria
- Monitor security-level risk and concentration continuously

## Portfolio Optimization Techniques
- Use mean-variance optimization with appropriate constraints and adjustments
- Consider Black-Litterman and other advanced optimization techniques
- Implement risk budgeting and risk parity approaches where appropriate
- Account for transaction costs and tax implications in optimization
- Validate optimization results with scenario analysis and stress testing

## Performance Attribution and Analysis
- Conduct detailed attribution analysis at multiple levels (asset allocation, security selection)
- Analyze performance relative to benchmarks and peer groups
- Identify sources of alpha and areas for improvement
- Monitor tracking error and information ratio continuously
- Document lessons learned and incorporate into future portfolio construction
```

#### Create `.github/instructions/risk-assessment.instructions.md`:

```markdown
---
applyTo: "**/*.risk,**/*.var,**/*.stress,**/risk/**,**/analytics/risk/**"
description: "Risk assessment methodology and risk management best practices"
---

# Risk Assessment Procedural Memory

## Risk Identification and Classification
- Identify all sources of investment risk including market, credit, liquidity, and operational risks
- Classify risks by type, magnitude, and probability of occurrence
- Consider tail risks and extreme scenarios in risk assessment
- Monitor correlation risks and concentration risks continuously
- Assess model risk and parameter uncertainty in risk models

## Quantitative Risk Measurement
- Use Value at Risk (VaR) and Conditional Value at Risk (CVaR) for downside risk measurement
- Implement multiple risk models including parametric, historical simulation, and Monte Carlo methods
- Calculate risk-adjusted performance metrics including Sharpe ratio, Sortino ratio, and maximum drawdown
- Monitor tracking error, information ratio, and active risk continuously
- Use factor models to decompose and understand sources of risk

## Stress Testing and Scenario Analysis
- Conduct regular stress tests using historical and hypothetical scenarios
- Test portfolio resilience under extreme market conditions
- Analyze correlation breakdown and liquidity stress scenarios
- Model portfolio behavior during economic recessions and market crises
- Document stress test results and develop contingency plans

## Risk Limits and Controls
- Establish appropriate risk limits at portfolio, sector, and security levels
- Implement real-time risk monitoring and alert systems
- Use position limits, concentration limits, and VaR limits as primary controls
- Monitor liquidity risk and implement appropriate liquidity management procedures
- Maintain risk reporting and escalation procedures

## Risk Communication and Reporting
- Communicate risk clearly and effectively to clients and stakeholders
- Provide regular risk reports with appropriate metrics and explanations
- Explain risk-return trade-offs and portfolio risk characteristics
- Document risk management decisions and rationale
- Maintain transparency in risk measurement methodologies and assumptions
```

#### Create `.github/instructions/financial-modeling.instructions.md`:

```markdown
---
applyTo: "**/*.model,**/*.valuation,**/*.backtest,**/models/**"
description: "Financial modeling standards and valuation methodology best practices"
---

# Financial Modeling Procedural Memory

## Model Development Standards
- Use clear and logical model structure with appropriate documentation
- Implement robust assumptions and sensitivity analysis
- Validate model inputs and outputs with independent data sources
- Use appropriate statistical methods and avoid overfitting
- Document model limitations and appropriate use cases

## Valuation Methodology
- Use multiple valuation approaches including DCF, relative valuation, and asset-based methods
- Apply appropriate discount rates based on risk and cost of capital
- Consider multiple scenarios in valuation analysis
- Use comparable company analysis and precedent transactions appropriately
- Validate valuation results with market prices and other benchmarks

## Backtesting and Model Validation
- Conduct comprehensive backtesting using out-of-sample data
- Test model performance across different market environments
- Analyze model stability and parameter sensitivity
- Document model performance statistics and limitations
- Implement ongoing model monitoring and validation procedures

## Quantitative Factor Models
- Use academically validated factors with strong theoretical foundations
- Test factor stability and predictive power over time
- Consider factor interactions and non-linear relationships
- Implement appropriate factor timing and combination strategies
- Monitor factor performance and adjust models as needed

## Monte Carlo Simulation and Scenario Modeling
- Use appropriate probability distributions and parameter estimates
- Validate simulation results with analytical solutions where possible
- Consider correlation structures and tail dependencies in simulation
- Implement variance reduction techniques for improved efficiency
- Document simulation assumptions and interpret results appropriately
```

#### Create `.github/instructions/market-research.instructions.md`:

```markdown
---
applyTo: "**/*.research,**/research/**,**/*market*,**/*sector*"
description: "Market research methodology and analysis standards"
---

# Market Research Procedural Memory

## Macroeconomic Analysis Framework
- Analyze key economic indicators including GDP, inflation, employment, and monetary policy
- Monitor central bank policies and their impact on financial markets
- Assess geopolitical risks and their potential market implications
- Consider demographic trends and their long-term economic impacts
- Use leading indicators to anticipate economic turning points

## Sector and Industry Analysis
- Conduct comprehensive industry structure analysis using Porter's Five Forces
- Analyze industry lifecycle stage and competitive dynamics
- Monitor regulatory changes and their impact on industry profitability
- Assess technological disruption and innovation within sectors
- Compare sector valuations and fundamentals across time and regions

## Market Cycle and Timing Analysis
- Identify market cycle stages and their investment implications
- Use technical analysis to supplement fundamental market research
- Monitor sentiment indicators and contrarian investment opportunities
- Analyze market breadth and momentum indicators
- Consider seasonal patterns and calendar effects in market analysis

## Global and Regional Market Analysis
- Assess relative attractiveness of different geographic markets
- Analyze currency trends and their impact on international investments
- Monitor global capital flows and their market implications
- Consider cultural and institutional factors in international market analysis
- Assess country-specific risks including political and regulatory risks

## Research Process and Documentation
- Use multiple independent sources to validate research conclusions
- Document research methodology and key assumptions clearly
- Update research regularly and communicate changes in outlook
- Maintain research archives for historical reference and backtesting
- Coordinate research efforts across different asset classes and regions
```

#### Create `.github/instructions/security-analysis.instructions.md`:

```markdown
---
applyTo: "**/*equity*,**/*bond*,**/*security*,**/research/security-analysis/**"
description: "Security analysis methodology and valuation standards"
---

# Security Analysis Procedural Memory

## Fundamental Equity Analysis
- Conduct comprehensive financial statement analysis including quality of earnings assessment
- Analyze business model, competitive positioning, and management quality
- Use multiple valuation methods including DCF, P/E, EV/EBITDA, and PEG ratios
- Assess company-specific risks including operational, financial, and strategic risks
- Monitor key performance indicators and business trends continuously

## Credit Analysis and Fixed Income
- Analyze credit quality using financial ratios and qualitative factors
- Assess default probability and recovery rates for credit securities
- Consider duration, convexity, and yield curve positioning in bond analysis
- Evaluate municipal bond credit quality and tax considerations
- Monitor credit spread movements and relative value opportunities

## Technical Analysis Integration
- Use chart patterns and technical indicators to supplement fundamental analysis
- Identify support and resistance levels for entry and exit timing
- Monitor volume patterns and momentum indicators
- Consider technical factors in position sizing and risk management
- Validate technical signals with fundamental analysis

## Quantitative Screening and Factor Analysis
- Use quantitative screens to identify investment opportunities
- Implement factor-based approaches including value, growth, quality, and momentum factors
- Analyze factor loadings and exposures in security selection
- Consider factor timing and rotation strategies
- Validate quantitative signals with fundamental research

## ESG and Sustainability Analysis
- Integrate environmental, social, and governance factors into security analysis
- Assess ESG risks and opportunities in investment decisions
- Use ESG ratings and scores appropriately with independent analysis
- Consider long-term sustainability and stakeholder capitalism trends
- Monitor ESG controversies and their potential impact on security values
```

### Step 5: Investment Management Episodic Memory Files

#### Create `.github/prompts/portfolio-construction.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Portfolio construction and optimization workflow"
---

# Portfolio Construction Episode Template

## Phase 1: Investment Objectives and Constraints Analysis
- Define clear investment objectives including return targets and risk tolerance
- Identify investment constraints including liquidity needs, time horizon, and regulatory requirements
- Assess client-specific factors including tax situation and ESG preferences
- Establish appropriate benchmark and performance measurement criteria
- Document investment policy statement with clear guidelines and restrictions

## Phase 2: Strategic Asset Allocation Development
- Develop long-term capital market assumptions for major asset classes
- Use mean-variance optimization and other techniques to determine optimal asset allocation
- Consider alternative investments and their role in portfolio diversification
- Test asset allocation robustness using scenario analysis and stress testing
- Establish rebalancing rules and tactical allocation ranges

## Phase 3: Security Selection and Implementation
- Implement systematic security selection process based on investment philosophy
- Use fundamental analysis, quantitative factors, and technical analysis appropriately
- Consider transaction costs, tax implications, and market impact in implementation
- Optimize portfolio construction using appropriate optimization techniques
- Establish position sizing and risk management rules

## Phase 4: Portfolio Monitoring and Optimization
- Implement ongoing portfolio monitoring and risk management procedures
- Conduct regular performance attribution and risk analysis
- Optimize portfolio based on changing market conditions and client needs
- Execute rebalancing and tactical adjustments systematically
- Document portfolio decisions and maintain detailed audit trail

Focus on client objectives and systematic implementation
```

#### Create `.github/prompts/investment-research.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Investment research and due diligence workflow"
---

# Investment Research Episode Template

## Phase 1: Research Planning and Scope Definition
- Define research objectives and specific questions to be answered
- Identify key information sources and data requirements
- Plan research methodology and analytical approach
- Establish timeline and resource allocation for research project
- Consider potential biases and limitations in research design

## Phase 2: Data Collection and Analysis
- Gather relevant financial data, market information, and industry research
- Conduct fundamental analysis using financial statements and key metrics
- Perform comparative analysis with peers and benchmarks
- Analyze quantitative factors and technical indicators
- Interview management teams and industry experts where appropriate

## Phase 3: Valuation and Risk Assessment
- Apply multiple valuation methodologies to determine fair value
- Conduct scenario analysis and sensitivity testing
- Assess investment risks including business, financial, and market risks
- Analyze ESG factors and their potential impact on investment returns
- Compare risk-adjusted returns with alternative investment opportunities

## Phase 4: Investment Recommendation and Documentation
- Synthesize research findings into clear investment recommendation
- Document investment thesis with supporting analysis and rationale
- Identify key risks and potential catalysts for investment performance
- Establish target prices, position sizing, and monitoring criteria
- Communicate research conclusions to investment committee and portfolio managers

Focus on rigorous analysis and evidence-based conclusions
```

#### Create `.github/prompts/risk-analysis.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Risk analysis and stress testing workflow"
---

# Risk Analysis Episode Template

## Phase 1: Risk Identification and Classification
- Identify all sources of portfolio risk including market, credit, liquidity, and operational risks
- Classify risks by type, magnitude, and probability of occurrence
- Assess correlation risks and concentration risks across portfolio
- Consider tail risks and extreme scenarios in risk assessment
- Map risks to potential impact on portfolio objectives and client goals

## Phase 2: Quantitative Risk Measurement
- Calculate Value at Risk (VaR) and Conditional Value at Risk (CVaR) using multiple methodologies
- Implement factor models to decompose and understand sources of risk
- Measure tracking error, active risk, and risk-adjusted performance metrics
- Analyze portfolio sensitivity to key risk factors and market movements
- Validate risk models using backtesting and out-of-sample analysis

## Phase 3: Stress Testing and Scenario Analysis
- Design stress tests using historical scenarios and hypothetical extreme events
- Test portfolio resilience under various market conditions and economic scenarios
- Analyze correlation breakdown and liquidity stress scenarios
- Model portfolio behavior during market crises and economic recessions
- Assess portfolio downside protection and tail risk characteristics

## Phase 4: Risk Management and Mitigation
- Develop risk management strategies based on risk analysis findings
- Implement appropriate risk controls and limits at portfolio and position levels
- Design contingency plans for extreme risk scenarios
- Monitor risk continuously and establish alert systems for limit breaches
- Communicate risk findings and recommendations to stakeholders and clients

Focus on comprehensive risk assessment and proactive management
```

#### Create `.github/prompts/market-analysis.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Market analysis and outlook development workflow"
---

# Market Analysis Episode Template

## Phase 1: Macroeconomic Environment Assessment
- Analyze current economic conditions including growth, inflation, and employment trends
- Monitor central bank policies and their implications for financial markets
- Assess geopolitical risks and their potential impact on market performance
- Consider structural economic changes and long-term demographic trends
- Evaluate policy responses and their effectiveness in current environment

## Phase 2: Market Valuation and Technical Analysis
- Assess current market valuations using multiple metrics and historical comparisons
- Analyze earnings trends, margin pressures, and corporate fundamentals
- Conduct technical analysis of major market indices and sectors
- Monitor sentiment indicators and positioning data for contrarian signals
- Compare valuations across regions, sectors, and asset classes

## Phase 3: Sector and Style Analysis
- Analyze relative performance and valuations across market sectors
- Assess factor performance including value, growth, quality, and momentum
- Monitor style rotation patterns and their underlying drivers
- Evaluate sector-specific fundamentals and competitive dynamics
- Consider thematic investment opportunities and secular trends

## Phase 4: Market Outlook and Investment Implications
- Synthesize analysis into coherent market outlook and investment thesis
- Identify key risks and opportunities for portfolio positioning
- Develop tactical asset allocation recommendations based on market analysis
- Communicate market views and their implications for investment strategy
- Establish monitoring criteria and potential triggers for strategy changes

Focus on objective analysis and actionable investment insights
```

#### Create `.github/prompts/strategy-development.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Investment strategy development and implementation workflow"
---

# Strategy Development Episode Template

## Phase 1: Strategy Foundation and Philosophy
- Define investment philosophy and core beliefs about market behavior
- Establish strategy objectives including return targets and risk parameters
- Identify target client base and appropriate market positioning
- Develop competitive advantages and differentiation factors
- Create theoretical framework supporting strategy approach

## Phase 2: Strategy Design and Backtesting
- Design systematic investment process and decision-making framework
- Develop quantitative models and screening criteria for strategy implementation
- Conduct comprehensive backtesting using historical data and multiple time periods
- Test strategy performance across different market environments and cycles
- Analyze strategy characteristics including volatility, drawdowns, and correlation

## Phase 3: Implementation Planning and Infrastructure
- Design operational infrastructure required for strategy implementation
- Establish technology requirements and data needs for strategy execution
- Develop risk management framework and compliance procedures
- Plan portfolio construction and trade execution processes
- Create performance measurement and attribution framework

## Phase 4: Strategy Launch and Monitoring
- Implement strategy with appropriate position sizing and risk controls
- Monitor strategy performance and characteristics continuously
- Conduct regular strategy reviews and make adjustments as needed
- Communicate strategy performance and positioning to stakeholders
- Document lessons learned and continuously improve strategy implementation

Focus on systematic approach and continuous improvement
```

### Step 6: Meta-Cognitive Files Integration

The learning.instructions.md, meta-cognition.instructions.md, consolidation.prompt.md, self-assessment.prompt.md, meta-learning.prompt.md, and cognitive-health.prompt.md files from previous setups apply to investment management as well, focusing on continuous improvement of investment management capabilities.

## 💰 Investment Management Setup Validation

After creating all files, verify investment management setup:

1. **Check investment management file structure**: Ensure all directories and investment-specific files exist
2. **Validate VS Code settings**: Confirm investment management instruction files are recognized
3. **Test investment management activation**: Try investment management "@" commands in Copilot chat
4. **Verify data security**: Check that confidential research patterns are properly excluded

## 🚀 Investment Management Quick Start Commands

After setup, test with these investment management-specific commands:

**Investment Management Tests**:
- `@workspace Help me construct an optimal portfolio` (Should activate portfolio-construction.prompt.md)
- `Analyze investment risks and stress test portfolio` (Should activate risk-analysis.prompt.md)
- `Conduct comprehensive market analysis` (Should activate market-analysis.prompt.md)

**Research and Analysis Tests**:
- `Perform security analysis and valuation` (Should activate investment-research.prompt.md)
- `Develop investment strategy framework` (Should activate strategy-development.prompt.md)
- `Create performance attribution analysis` (Should activate performance-review.prompt.md)

**Meta-Investment Management Tests**:
- `@workspace Assess your investment analysis quality` (Should activate self-assessment.prompt.md)
- `How can you improve portfolio construction support?` (Should activate meta-learning.prompt.md)
- `Monitor your investment management architecture health` (Should activate cognitive-health.prompt.md)

## ⚡ Investment Management Success Indicators

Your investment management cognitive architecture is working when:

- **Fiduciary Excellence**: All investment decisions prioritize client interests and maintain ethical standards
- **Risk-First Approach**: Comprehensive risk assessment precedes all investment opportunities
- **Evidence-Based Decisions**: All investment recommendations are supported by rigorous analysis
- **Systematic Process**: Investment process is repeatable, documented, and continuously improved
- **Performance Accountability**: Clear performance measurement and attribution analysis
- **Client Communication**: Transparent and effective communication of investment strategy and results
- **Meta-Cognitive Growth**: System continuously improves investment management capabilities and processes

---

**SETUP COMPLETE**: Your investment management cognitive architecture is now ready for comprehensive portfolio management, fiduciary responsibility, and evidence-based investment decision-making. The system maintains the highest ethical standards while providing sophisticated analysis and strategic guidance for all aspects of investment management.
