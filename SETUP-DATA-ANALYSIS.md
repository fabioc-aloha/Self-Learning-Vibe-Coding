# Data Analysis Cognitive Architecture Auto-Setup Guide

**INSTRUCTIONS FOR GITHUB COPILOT**: This file contains complete setup instructions for implementing the Self-Learning Vibe Coding cognitive memory architecture optimized for sophisticated statistical data analysis using Python, Jupyter notebooks, and SPSS .sav file processing. Follow these instructions to create all necessary directories, files, and configurations.

## 📊 Data Analysis Automated Setup Protocol

**Execute these steps in order to establish a complete cognitive architecture system for advanced statistical data analysis:**

### Step 1: VS Code Configuration (Required)

Add these settings to VS Code `settings.json`:

```json
{
  "github.copilot.chat.codeGeneration.useInstructionFiles": true,
  "chat.promptFiles": true,
  "chat.instructionsFilesLocations": [".github/instructions"],
  "python.defaultInterpreterPath": ".venv/Scripts/python.exe",
  "python.envFile": "${workspaceFolder}/.env",
  "python.linting.enabled": true,
  "python.linting.pylintEnabled": true,
  "python.linting.flake8Enabled": true,
  "python.formatting.provider": "black",
  "python.testing.pytestEnabled": true,
  "python.testing.pytestArgs": ["tests/"],
  "jupyter.askForKernelRestart": false,
  "jupyter.alwaysTrustNotebooks": true,
  "jupyter.showCellInputCode": true,
  "jupyter.interactiveWindow.textEditor.executeSelection": true,
  "files.associations": {
    "*.py": "python",
    "*.ipynb": "jupyter-notebook",
    "*.sav": "spss",
    "requirements*.txt": "pip-requirements",
    "pyproject.toml": "toml"
  },
  "notebook.cellToolbarLocation": {
    "default": "right",
    "jupyter-notebook": "left"
  }
}
```

**Access settings.json**: `Ctrl+Shift+P` → "Preferences: Open User Settings (JSON)"

### Step 2: Create Directory Structure

Create this exact folder structure in the project root:

```
project-root/
├── .github/
│   ├── copilot-instructions.md          # Global Declarative Memory
│   ├── instructions/                    # Procedural Memory Store
│   │   ├── data-analysis.instructions.md
│   │   ├── statistical-modeling.instructions.md
│   │   ├── visualization.instructions.md
│   │   ├── spss-processing.instructions.md
│   │   ├── jupyter.instructions.md
│   │   ├── documentation.instructions.md
│   │   ├── learning.instructions.md     # Meta-Cognitive Learning
│   │   └── meta-cognition.instructions.md  # Self-Monitoring
│   └── prompts/                         # Episodic Memory Store
│       ├── exploratory-analysis.prompt.md
│       ├── descriptive-statistics.prompt.md
│       ├── inferential-statistics.prompt.md
│       ├── multivariate-analysis.prompt.md
│       ├── time-series-analysis.prompt.md
│       ├── machine-learning.prompt.md
│       ├── data-cleaning.prompt.md
│       ├── visualization-creation.prompt.md
│       ├── report-generation.prompt.md
│       ├── spss-migration.prompt.md
│       ├── consolidation.prompt.md
│       ├── self-assessment.prompt.md    # Meta-Cognitive Assessment
│       ├── meta-learning.prompt.md      # Learning Strategy Evolution
│       └── cognitive-health.prompt.md   # Architecture Maintenance
├── .venv/                               # Virtual Environment
├── notebooks/                           # Jupyter Notebooks
│   ├── exploratory/                     # Exploratory Analysis
│   ├── modeling/                        # Statistical Modeling
│   ├── visualization/                   # Data Visualization
│   └── reports/                         # Final Reports
├── data/
│   ├── raw/                            # Raw SPSS files
│   ├── processed/                      # Cleaned data
│   └── output/                         # Analysis results
├── src/                                # Source Code
│   ├── utils/                          # Utility functions
│   ├── models/                         # Statistical models
│   └── visualization/                  # Custom plots
├── tests/                              # Test Files
├── requirements.txt                    # Core Dependencies
├── requirements-analysis.txt           # Analysis-specific Dependencies
├── requirements-dev.txt                # Development Dependencies
├── .env                                # Environment Variables
├── .gitignore                         # Git Ignore
└── pyproject.toml                     # Project Configuration
```

### Step 3: Advanced Analytics Environment Setup

**Create virtual environment and install comprehensive analytics stack:**

```powershell
# Create virtual environment
python -m venv .venv

# Activate virtual environment (Windows PowerShell)
.venv\Scripts\Activate.ps1

# Upgrade pip and install build tools
python -m pip install --upgrade pip setuptools wheel

# Create project directories
New-Item -ItemType Directory -Force -Path "notebooks/exploratory", "notebooks/modeling", "notebooks/visualization", "notebooks/reports"
New-Item -ItemType Directory -Force -Path "data/raw", "data/processed", "data/output"
New-Item -ItemType Directory -Force -Path "src/utils", "src/models", "src/visualization", "tests"

# Create comprehensive requirements files
@"
# Core Data Analysis Libraries
pandas>=2.1.0
numpy>=1.24.0
scipy>=1.11.0

# SPSS Data Processing
pyreadstat>=1.2.0
savReaderWriter>=4.0.0

# Statistical Analysis
statsmodels>=0.14.0
pingouin>=0.5.3
scikit-learn>=1.3.0
lifelines>=0.27.0

# Advanced Analytics
factor-analyzer>=0.4.1
prince>=0.7.1
imbalanced-learn>=0.11.0
optuna>=3.3.0

# Visualization
matplotlib>=3.7.0
seaborn>=0.12.0
plotly>=5.15.0
bokeh>=3.2.0
altair>=5.0.0

# Data Processing
openpyxl>=3.1.0
xlsxwriter>=3.1.0
python-dotenv>=1.0.0
tqdm>=4.65.0
"@ | Out-File -FilePath "requirements.txt" -Encoding utf8

@"
# Advanced Statistical Libraries
rpy2>=3.5.13
pymc>=5.7.0
arviz>=0.16.0
bambi>=0.12.0
xarray>=2023.7.0

# Machine Learning Extensions
xgboost>=1.7.0
lightgbm>=4.0.0
catboost>=1.2.0
tensorflow>=2.13.0
torch>=2.0.0
transformers>=4.33.0

# Time Series Analysis
prophet>=1.1.4
sktime>=0.21.0
darts>=0.25.0
neuralprophet>=0.5.4

# Network Analysis
networkx>=3.1.0
pyvis>=0.3.2

# Text Analytics
nltk>=3.8.0
spacy>=3.6.0
textblob>=0.17.0
wordcloud>=1.9.0

# Geospatial Analysis
geopandas>=0.13.0
folium>=0.14.0
contextily>=1.3.0

# Dimensionality Reduction
umap-learn>=0.5.3
hdbscan>=0.8.29
"@ | Out-File -FilePath "requirements-analysis.txt" -Encoding utf8

@"
# Development and Testing
jupyter>=1.0.0
jupyterlab>=4.0.0
notebook>=7.0.0
ipywidgets>=8.1.0
jupytext>=1.15.0

# Code Quality
pytest>=7.4.0
pytest-cov>=4.1.0
black>=23.0.0
flake8>=6.0.0
pylint>=2.17.0
mypy>=1.5.0
isort>=5.12.0

# Documentation
sphinx>=7.1.0
sphinx-rtd-theme>=1.3.0
nbsphinx>=0.9.0
jupyter-book>=0.15.0

# Performance Profiling
memory-profiler>=0.61.0
line-profiler>=4.1.0
py-spy>=0.3.14

# Data Validation
great-expectations>=0.17.0
pandera>=0.15.0
cerberus>=1.3.4
"@ | Out-File -FilePath "requirements-dev.txt" -Encoding utf8

# Install all dependencies
Write-Host "Installing core dependencies..." -ForegroundColor Green
pip install -r requirements.txt

Write-Host "Installing analysis-specific dependencies..." -ForegroundColor Green
pip install -r requirements-analysis.txt

Write-Host "Installing development dependencies..." -ForegroundColor Green
pip install -r requirements-dev.txt

# Create environment configuration
@"
# Environment Variables for Data Analysis
PYTHONPATH=src
DEBUG=True
JUPYTER_ENABLE_LAB=yes

# Data Paths
DATA_RAW_PATH=data/raw
DATA_PROCESSED_PATH=data/processed
DATA_OUTPUT_PATH=data/output

# Analysis Configuration
DEFAULT_SIGNIFICANCE_LEVEL=0.05
DEFAULT_CONFIDENCE_INTERVAL=0.95
MAX_MISSING_THRESHOLD=0.1

# Visualization Settings
MATPLOTLIB_BACKEND=Qt5Agg
PLOTLY_RENDERER=browser
DEFAULT_DPI=300
DEFAULT_FIGURE_SIZE=12,8

# Memory Management
PANDAS_MAX_COLUMNS=None
PANDAS_MAX_ROWS=None
NUMPY_RANDOM_SEED=42
"@ | Out-File -FilePath ".env" -Encoding utf8

# Create comprehensive .gitignore
@"
# Python
__pycache__/
*.py[cod]
*$py.class
*.so
.Python
build/
develop-eggs/
dist/
downloads/
eggs/
.eggs/
lib/
lib64/
parts/
sdist/
var/
wheels/
*.egg-info/
.installed.cfg
*.egg

# Virtual Environment
.venv/
venv/
ENV/

# Jupyter Notebooks
.ipynb_checkpoints/
*/.ipynb_checkpoints/*

# Data Files (adjust based on your needs)
data/raw/*.sav
data/raw/*.xlsx
data/raw/*.csv
data/processed/*.parquet
data/output/*.pdf
data/output/*.png
data/output/*.html

# IDE
.vscode/
.idea/
*.swp
*.swo
*~

# Environment
.env
.env.local
.env.*.local

# Testing
.coverage
.pytest_cache/
htmlcov/

# Documentation
docs/_build/
site/

# OS
.DS_Store
Thumbs.db

# R (if using rpy2)
.Rhistory
.RData
.Ruserdata

# Temporary files
*.tmp
*.temp
*.log
"@ | Out-File -FilePath ".gitignore" -Encoding utf8

# Create pyproject.toml with data analysis configuration
@"
[build-system]
requires = ["setuptools>=45", "wheel"]
build-backend = "setuptools.build_meta"

[project]
name = "data-analysis-project"
version = "0.1.0"
description = "Advanced statistical data analysis project with SPSS support"
requires-python = ">=3.9"

[tool.black]
line-length = 88
target-version = ['py39']
include = '\.pyi?$'
extend-exclude = '''
/(
  \.eggs
  | \.git
  | \.venv
  | build
  | dist
)/
'''

[tool.isort]
profile = "black"
multi_line_output = 3
include_trailing_comma = true
force_grid_wrap = 0
use_parentheses = true
ensure_newline_before_comments = true
line_length = 88

[tool.pytest.ini_options]
testpaths = ["tests"]
python_files = ["test_*.py"]
python_classes = ["Test*"]
python_functions = ["test_*"]
addopts = "--cov=src --cov-report=html --cov-report=term --cov-report=xml"

[tool.mypy]
python_version = "3.9"
warn_return_any = true
warn_unused_configs = true
disallow_untyped_defs = true
ignore_missing_imports = true

[tool.pylint.messages_control]
disable = ["C0330", "C0326", "R0903", "R0913"]

[tool.coverage.run]
source = ["src"]
omit = ["*/tests/*", "*/test_*"]

[tool.coverage.report]
exclude_lines = [
    "pragma: no cover",
    "def __repr__",
    "raise AssertionError",
    "raise NotImplementedError"
]
"@ | Out-File -FilePath "pyproject.toml" -Encoding utf8

Write-Host "Environment setup complete!" -ForegroundColor Green
Write-Host "Jupyter Lab can be started with: jupyter lab" -ForegroundColor Yellow
```

### Step 4: Global Data Analysis Declarative Memory Setup

**Create `.github/copilot-instructions.md`** with this exact content:

```markdown
# Self-Learning Vibe Coding - Data Analysis Cognitive Memory Architecture

IMPORTANT: This file serves as Global Data Analysis Declarative Memory. Keep minimal and efficient. Detailed execution resides in specialized memory files.

## 🧠 Data Analysis Cognitive Architecture Status

**Working Memory**: 4/4 rules (at optimal capacity for statistical data analysis)
**Consolidation**: Auto-trigger when exceeding capacity
**Memory Distribution**: Active across data analysis procedural (.instructions.md) and statistical episodic (.prompt.md) systems

## 🚀 Data Analysis Working Memory - Quick Reference (Limit: 4 Critical Rules)

| Priority | Rule | Load | Auto-Consolidate |
|----------|------|------|------------------|
| P1 | `@statistical` - Apply appropriate statistical methods based on data type and research questions | Low | Never |
| P2 | `@reproducible` - Ensure all analyses are reproducible with proper documentation and version control | Medium | >30 days unused |
| P3 | `@meditation` - Auto-consolidate when working memory capacity exceeded | High | When triggered |
| P4 | `@validation` - Validate assumptions, check data quality, and interpret results appropriately | Medium | When obsolete |

## 🎯 Data Analysis Cognitive Architecture Coordination

### Multi-Modal Data Analysis Memory Distribution

**Procedural Memory Activation** (Context-Dependent):
- `data-analysis.instructions.md` → General data analysis patterns for .py, .ipynb files
- `statistical-modeling.instructions.md` → Statistical methods for hypothesis testing, regression, ANOVA
- `visualization.instructions.md` → Data visualization best practices for matplotlib, seaborn, plotly
- `spss-processing.instructions.md` → SPSS .sav file processing with pyreadstat and savReaderWriter
- `jupyter.instructions.md` → Jupyter notebook organization and documentation standards
- `documentation.instructions.md` → Research documentation and report generation standards
- `learning.instructions.md` → Meta-cognitive learning and self-monitoring protocols
- `meta-cognition.instructions.md` → Self-awareness and cognitive monitoring patterns

**Episodic Memory Activation** (Problem-Solving):
- `exploratory-analysis.prompt.md` → Systematic exploratory data analysis workflows
- `descriptive-statistics.prompt.md` → Comprehensive descriptive statistics procedures
- `inferential-statistics.prompt.md` → Hypothesis testing and confidence interval workflows
- `multivariate-analysis.prompt.md` → Factor analysis, PCA, clustering, and classification
- `time-series-analysis.prompt.md` → Time series decomposition, forecasting, and analysis
- `machine-learning.prompt.md` → Predictive modeling and machine learning workflows
- `data-cleaning.prompt.md` → Data preprocessing and quality assessment procedures
- `visualization-creation.prompt.md` → Advanced visualization design and creation workflows
- `report-generation.prompt.md` → Statistical report writing and publication workflows
- `spss-migration.prompt.md` → SPSS to Python analysis migration procedures
- `consolidation.prompt.md` → Memory consolidation and cognitive architecture optimization
- `self-assessment.prompt.md` → Cognitive performance evaluation and improvement
- `meta-learning.prompt.md` → Learning strategy development and evolution
- `cognitive-health.prompt.md` → Architecture health monitoring and maintenance

### Auto-Consolidation Triggers

- Working memory > 4 rules → Execute consolidation.prompt.md
- Rule conflicts detected → Activate learning.instructions.md
- Performance degradation → Review and redistribute memory load
- User requests meditation → Full cognitive architecture optimization
- **Statistical assumption violations → Execute appropriate analysis workflow**
- **Meta-cognitive assessment needed → Execute self-assessment.prompt.md**
- **Learning strategy evolution required → Execute meta-learning.prompt.md**
- **Cognitive architecture health check → Execute cognitive-health.prompt.md**

## 🔄 Memory Transfer Protocol

**Immediate Transfer**: Critical errors → Quick Reference (P1-P4)
**Gradual Consolidation**: Repeated patterns → Procedural memory (.instructions.md)
**Complex Workflows**: Multi-step processes → Episodic memory (.prompt.md)
**Archive Management**: Obsolete rules → Historical storage in specialized files
**Index Maintenance**: Auto-update Long-Term Memory Index during all transfers

## 📚 Long-Term Memory Index

### Procedural Memory Store (.github/instructions/)
| File | Domain | Activation Pattern | Last Updated |
|------|--------|-------------------|--------------|
| data-analysis.instructions.md | General Analysis | *.py, *.ipynb, data analysis | Auto-tracked |
| statistical-modeling.instructions.md | Statistics | regression, ANOVA, hypothesis testing | Auto-tracked |
| visualization.instructions.md | Data Visualization | matplotlib, seaborn, plotly | Auto-tracked |
| spss-processing.instructions.md | SPSS Integration | *.sav, pyreadstat, SPSS migration | Auto-tracked |
| jupyter.instructions.md | Notebook Standards | *.ipynb, Jupyter workflows | Auto-tracked |
| documentation.instructions.md | Research Documentation | reports, documentation | Auto-tracked |
| learning.instructions.md | Meta-Learning | *instructions*, *learning* | Auto-tracked |
| meta-cognition.instructions.md | Self-Monitoring | *meta*, *monitor*, *assess* | Auto-tracked |

### Episodic Memory Store (.github/prompts/)
| File | Workflow Type | Complexity Level | Usage Frequency |
|------|---------------|------------------|-----------------|
| exploratory-analysis.prompt.md | EDA Workflows | Medium | Auto-tracked |
| descriptive-statistics.prompt.md | Descriptive Analysis | Low | Auto-tracked |
| inferential-statistics.prompt.md | Hypothesis Testing | High | Auto-tracked |
| multivariate-analysis.prompt.md | Multivariate Methods | High | Auto-tracked |
| time-series-analysis.prompt.md | Time Series | High | Auto-tracked |
| machine-learning.prompt.md | Predictive Modeling | High | Auto-tracked |
| data-cleaning.prompt.md | Data Preprocessing | Medium | Auto-tracked |
| visualization-creation.prompt.md | Advanced Visualization | Medium | Auto-tracked |
| report-generation.prompt.md | Report Writing | High | Auto-tracked |
| spss-migration.prompt.md | SPSS Migration | Medium | Auto-tracked |
| consolidation.prompt.md | Memory Optimization | High | Auto-tracked |
| self-assessment.prompt.md | Self-Evaluation | High | Auto-tracked |
| meta-learning.prompt.md | Learning Evolution | High | Auto-tracked |
| cognitive-health.prompt.md | Health Monitoring | Medium | Auto-tracked |

### Memory Transfer Protocol Status
- **Active Files**: 22 specialized memory files (8 procedural + 14 episodic)
- **Last Consolidation**: Setup initialization with data analysis meta-cognitive enhancements
- **Cognitive Load Status**: Optimized through distributed processing with statistical analysis patterns
- **Index Synchronization**: Maintained automatically during consolidation
- **Meta-Cognitive Status**: Fully operational with self-assessment and learning evolution capabilities

---

*Global Declarative Memory Component - Coordinates distributed cognitive architecture while maintaining optimal working memory efficiency. Detailed execution protocols reside in specialized memory files.*
```

### Step 5: Procedural Memory Files

#### Create `.github/instructions/data-analysis.instructions.md`:

```markdown
---
applyTo: "**/*.py,**/*.ipynb,**/data/**,**/notebooks/**"
description: "General data analysis patterns and best practices"
---

# Data Analysis Procedural Memory

## Data Loading and Initial Inspection
- Use pandas.read_spss() or pyreadstat.read_sav() for SPSS files
- Perform initial data inspection with .info(), .describe(), .head()
- Check for missing values, duplicates, and data type consistency
- Document data source, collection method, and variable definitions
- Create data dictionaries for complex datasets

## Data Quality Assessment
- Identify and handle missing data patterns (MCAR, MAR, MNAR)
- Detect and address outliers using statistical methods
- Validate data ranges and logical consistency
- Check for multicollinearity in predictive variables
- Assess sample size adequacy for planned analyses

## Reproducible Analysis Workflow
- Use consistent naming conventions for variables and files
- Set random seeds for reproducible results
- Version control data processing scripts
- Document all analysis decisions and assumptions
- Create automated data processing pipelines

## Statistical Best Practices
- Choose appropriate statistical tests based on data type and distribution
- Check statistical assumptions before applying tests
- Use appropriate effect size measures alongside p-values
- Apply multiple comparison corrections when necessary
- Report confidence intervals and practical significance

## Code Organization and Documentation
- Structure notebooks with clear markdown sections
- Use functions for repeated analysis tasks
- Create reusable utility modules for common operations
- Include detailed comments explaining analysis rationale
- Generate automated reports with results and interpretations
```

#### Create `.github/instructions/statistical-modeling.instructions.md`:

```markdown
---
applyTo: "**/*model*,**/*stat*,**/*test*,**/*regression*"
description: "Statistical modeling and hypothesis testing best practices"
---

# Statistical Modeling Procedural Memory

## Hypothesis Testing Framework
- Clearly state null and alternative hypotheses
- Choose appropriate significance level (typically α = 0.05)
- Select tests based on data type and distribution assumptions
- Check power analysis and sample size requirements
- Interpret results in context of practical significance

## Descriptive Statistics
- Report appropriate measures of central tendency and variability
- Use robust statistics for non-normal distributions
- Include confidence intervals for point estimates
- Provide effect size measures (Cohen's d, eta-squared, etc.)
- Create comprehensive summary tables

## Regression Analysis
- Check linearity, independence, homoscedasticity, and normality assumptions
- Assess multicollinearity using VIF or correlation matrices
- Use appropriate model selection techniques (AIC, BIC, cross-validation)
- Validate models using train/test splits or cross-validation
- Interpret coefficients in context of the research question

## Multivariate Analysis
- Apply appropriate dimensionality reduction techniques (PCA, FA)
- Use clustering methods suitable for data structure
- Validate cluster solutions using multiple criteria
- Interpret factor loadings and component meanings
- Report model fit statistics and validation metrics

## Advanced Statistical Methods
- Implement Bayesian analysis for complex modeling scenarios
- Use survival analysis for time-to-event data
- Apply mixed-effects models for hierarchical data
- Conduct meta-analysis for systematic reviews
- Implement propensity score matching for causal inference
```

#### Create `.github/instructions/spss-processing.instructions.md`:

```markdown
---
applyTo: "**/*.sav,**/*spss*,**/*pyreadstat*"
description: "SPSS data file processing and migration patterns"
---

# SPSS Processing Procedural Memory

## SPSS File Reading
- Use pyreadstat.read_sav() for comprehensive metadata preservation
- Extract variable labels, value labels, and missing value definitions
- Preserve SPSS data types and measurement levels
- Handle SPSS system missing values appropriately
- Document original SPSS variable names and transformations

## Data Type Conversion
- Convert SPSS string variables to appropriate pandas dtypes
- Transform SPSS date/time variables to pandas datetime
- Handle SPSS categorical variables with proper encoding
- Preserve ordinal variable ordering from SPSS
- Convert SPSS missing value codes to pandas NaN

## Variable Management
- Create comprehensive variable dictionaries
- Map SPSS variable labels to descriptive column names
- Preserve value labels for categorical variables
- Document any variable transformations or recodings
- Maintain backward compatibility with original SPSS syntax

## Analysis Migration
- Translate common SPSS procedures to Python equivalents
- Implement SPSS syntax patterns using pandas and scipy
- Reproduce SPSS output formats for comparison
- Validate migrated analyses against original SPSS results
- Document differences in calculation methods or assumptions

## Metadata Preservation
- Export enhanced datasets with full documentation
- Create SPSS-compatible output for collaboration
- Generate syntax files for reproducible SPSS workflows
- Maintain audit trails for data modifications
- Provide clear migration documentation for stakeholders
```

#### Create `.github/instructions/visualization.instructions.md`:

```markdown
---
applyTo: "**/*plot*,**/*chart*,**/*visual*,**/*graph*"
description: "Data visualization design and implementation best practices"
---

# Visualization Procedural Memory

## Chart Selection and Design
- Choose appropriate chart types based on data structure and message
- Follow principles of visual hierarchy and cognitive load reduction
- Use consistent color schemes and typography throughout projects
- Ensure accessibility with colorblind-friendly palettes
- Apply appropriate aspect ratios and scaling

## Statistical Visualization
- Include error bars, confidence intervals, and uncertainty measures
- Use appropriate binning and smoothing for distributions
- Show individual data points when sample sizes are small
- Apply statistical overlays (regression lines, confidence bands)
- Annotate significant differences and effect sizes

## Interactive and Dynamic Plots
- Implement interactive features that enhance understanding
- Use tooltips and hover information effectively
- Create linked plots for multi-dimensional exploration
- Design responsive layouts for different screen sizes
- Optimize performance for large datasets

## Publication-Quality Graphics
- Use vector formats (SVG, PDF) for scalable graphics
- Apply consistent styling with custom themes
- Include comprehensive titles, labels, and captions
- Follow journal-specific formatting requirements
- Create automated figure generation pipelines

## Dashboard and Report Integration
- Design cohesive visual narratives across multiple charts
- Implement effective layout and spacing principles
- Use consistent data-ink ratios and minimize chartjunk
- Create executive summary visualizations
- Enable easy updating with new data
```

#### Create `.github/instructions/jupyter.instructions.md`:

```markdown
---
applyTo: "**/*.ipynb,**/notebooks/**"
description: "Jupyter notebook organization and documentation standards"
---

# Jupyter Notebook Procedural Memory

## Notebook Structure and Organization
- Start with clear title, author, and date information
- Include table of contents for longer notebooks
- Use hierarchical markdown headers for logical sections
- Separate exploration, analysis, and reporting sections
- End with summary and conclusions

## Code Cell Best Practices
- Keep cells focused on single tasks or concepts
- Use descriptive variable names and consistent styling
- Include inline comments for complex operations
- Clear outputs before committing to version control
- Use markdown cells to explain analysis rationale

## Data and Results Documentation
- Document data sources, collection methods, and limitations
- Explain statistical methods and assumption checking
- Interpret results in context of research questions
- Include methodology references and citations
- Provide clear conclusions and recommendations

## Reproducibility and Version Control
- Set random seeds for stochastic processes
- Pin package versions in requirements files
- Use relative paths for data and output files
- Create automated notebook execution pipelines
- Generate static reports for sharing and archiving

## Interactive Elements and Widgets
- Use ipywidgets for parameter exploration
- Implement interactive plotting with plotly or bokeh
- Create dynamic filtering and selection interfaces
- Design user-friendly parameter adjustment tools
- Enable real-time visualization updates
```

### Step 6: Episodic Memory Files

#### Create `.github/prompts/exploratory-analysis.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "run_in_terminal", "read_file", "create_file"]
description: "Systematic exploratory data analysis workflow"
---

# Exploratory Data Analysis Episode Template

## Phase 1: Data Import and Initial Assessment
- Load SPSS .sav files using pyreadstat with metadata preservation
- Examine dataset structure, dimensions, and variable types
- Review variable labels, value labels, and missing value patterns
- Create comprehensive data dictionary and codebook
- Document data source and collection methodology

## Phase 2: Univariate Analysis
- Generate descriptive statistics for all variables
- Create appropriate visualizations (histograms, box plots, bar charts)
- Assess distributions and identify potential transformations
- Detect outliers using statistical methods (IQR, z-scores)
- Document unusual patterns or data quality issues

## Phase 3: Bivariate and Multivariate Exploration
- Create correlation matrices and heatmaps
- Generate cross-tabulations for categorical variables
- Explore relationships using scatter plots and regression lines
- Identify potential confounding variables
- Assess patterns of missing data across variables

## Phase 4: Hypothesis Generation and Analysis Planning
- Formulate research questions based on data exploration
- Identify appropriate statistical tests and modeling approaches
- Plan additional data collection or transformation needs
- Document assumptions and limitations
- Create analysis roadmap for subsequent investigations

Use sophisticated analytics tools from ${workspaceFolder}/.venv
```

#### Create `.github/prompts/multivariate-analysis.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "run_in_terminal", "read_file", "create_file"]
description: "Comprehensive multivariate statistical analysis workflow"
---

# Multivariate Analysis Episode Template

## Phase 1: Data Preparation and Assumption Checking
- Assess multivariate normality using Mardia's test
- Check for multicollinearity using VIF and correlation matrices
- Handle missing data using appropriate imputation methods
- Standardize variables when necessary for analysis
- Verify sample size adequacy using power analysis

## Phase 2: Dimensionality Reduction
- Apply Principal Component Analysis (PCA) with scree plots
- Implement Factor Analysis with appropriate rotation methods
- Use parallel analysis to determine optimal number of factors
- Interpret factor loadings and component meanings
- Validate factor structure using confirmatory methods

## Phase 3: Clustering and Classification
- Apply hierarchical clustering with dendrogram analysis
- Implement k-means clustering with optimal cluster determination
- Use DBSCAN for density-based clustering when appropriate
- Validate cluster solutions using silhouette analysis
- Profile clusters using discriminant analysis

## Phase 4: Advanced Multivariate Methods
- Conduct MANOVA for multiple dependent variables
- Apply canonical correlation analysis for relationship exploration
- Implement structural equation modeling when appropriate
- Use machine learning methods for prediction and classification
- Validate models using cross-validation and holdout samples

Use advanced statistical libraries from ${workspaceFolder}/.venv
```

#### Create `.github/prompts/spss-migration.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "run_in_terminal", "read_file", "create_file"]
description: "SPSS to Python analysis migration workflow"
---

# SPSS Migration Episode Template

## Phase 1: SPSS File Analysis and Import
- Load .sav files using pyreadstat with complete metadata
- Extract and document variable labels, value labels, and formats
- Identify SPSS system missing values and user-defined missing values
- Preserve measurement levels (nominal, ordinal, scale)
- Create comprehensive variable mapping documentation

## Phase 2: Syntax Translation and Validation
- Translate SPSS FREQUENCIES to pandas value_counts and crosstabs
- Convert SPSS DESCRIPTIVES to pandas describe and scipy stats
- Migrate SPSS T-TEST to scipy.stats t-tests and effect sizes
- Transform SPSS ANOVA to statsmodels ANOVA and post-hoc tests
- Reproduce SPSS REGRESSION using statsmodels OLS and diagnostics

## Phase 3: Output Comparison and Validation
- Generate side-by-side comparisons of SPSS and Python results
- Validate statistical test results within acceptable tolerance
- Document any differences in calculation methods or assumptions
- Create equivalent visualization outputs using matplotlib/seaborn
- Ensure p-values, test statistics, and effect sizes match

## Phase 4: Enhanced Python Implementation
- Extend analyses with additional diagnostics not available in SPSS
- Implement advanced visualization capabilities
- Add robust statistical methods and bootstrap confidence intervals
- Create interactive dashboards for ongoing analysis
- Document advantages and enhanced capabilities of Python implementation

Use SPSS processing tools from ${workspaceFolder}/.venv
```

#### Create additional episodic memory files:

```markdown
# Additional episodic memory files to create:
# - .github/prompts/descriptive-statistics.prompt.md
# - .github/prompts/inferential-statistics.prompt.md
# - .github/prompts/time-series-analysis.prompt.md
# - .github/prompts/machine-learning.prompt.md
# - .github/prompts/data-cleaning.prompt.md
# - .github/prompts/visualization-creation.prompt.md
# - .github/prompts/report-generation.prompt.md
# - .github/prompts/consolidation.prompt.md (same as other setups)
# - .github/prompts/self-assessment.prompt.md (same as other setups)
# - .github/prompts/meta-learning.prompt.md (same as other setups)
# - .github/prompts/cognitive-health.prompt.md (same as other setups)
```

## 🎯 Setup Validation

After creating all files, verify setup:

1. **Check virtual environment**: Ensure `.venv` is created with all analytics packages
2. **Test SPSS file reading**: Verify pyreadstat can read .sav files
3. **Validate Jupyter setup**: Confirm Jupyter Lab/Notebook can access .venv kernel
4. **Check statistical libraries**: Test imports for statsmodels, scipy, sklearn
5. **Verify visualization tools**: Confirm matplotlib, seaborn, plotly work correctly

## 🚀 Quick Start Commands

After setup, test with these commands in GitHub Copilot:

**SPSS Integration Tests**:
- `@workspace Load and analyze this .sav file` (Should activate spss-processing.instructions.md)
- `Help me migrate this SPSS analysis to Python` (Should activate spss-migration.prompt.md)

**Statistical Analysis Tests**:
- `Perform comprehensive exploratory data analysis` (Should activate exploratory-analysis.prompt.md)
- `Conduct multivariate statistical analysis` (Should activate multivariate-analysis.prompt.md)
- `Create publication-quality visualizations` (Should activate visualization-creation.prompt.md)

**Advanced Analytics Tests**:
- `Build predictive models for this dataset` (Should activate machine-learning.prompt.md)
- `Analyze time series patterns and trends` (Should activate time-series-analysis.prompt.md)

**Meta-Cognition Tests**:
- `@workspace Assess your statistical analysis performance` (Should activate self-assessment.prompt.md)
- `How can you improve your data analysis strategies?` (Should activate meta-learning.prompt.md)

## ⚡ Success Indicators

Your data analysis cognitive architecture is working when:
- SPSS .sav files load seamlessly with preserved metadata
- Statistical analyses follow appropriate methodological standards
- Visualizations are publication-quality and follow best practices
- Jupyter notebooks are well-organized and reproducible
- All analyses include proper assumption checking and validation
- **Meta-cognitive capabilities**: The AI can assess its statistical analysis performance
- **Self-monitoring**: The system tracks analysis patterns and suggests improvements
- **Learning evolution**: The AI improves its statistical methodology over time
- **Methodological awareness**: The system validates assumptions and suggests appropriate tests

## 🔄 Maintenance

- Update statistical packages regularly with careful version testing
- Review and update statistical methodology based on latest research
- Execute consolidation meditation when adding 5+ new analysis patterns
- Monitor computational performance with large datasets
- **Execute self-assessment weekly to monitor analysis quality**
- **Run meta-learning analysis monthly for methodology optimization**
- **Perform cognitive architecture health checks quarterly**
- **Update statistical capabilities based on new research and methods**

## 📖 Recommended Learning Resources

- **Statistical Methods**: "An Introduction to Statistical Learning" by James et al.
- **Python for Data Science**: "Python Data Science Handbook" by VanderPlas
- **Advanced Statistics**: "The Elements of Statistical Learning" by Hastie et al.
- **SPSS Migration**: Official SPSS Python integration documentation
- **Visualization**: "Fundamentals of Data Visualization" by Wilke

---

**DATA ANALYSIS SETUP COMPLETE**: Your adaptive AI statistical analysis partner is now ready with comprehensive SPSS .sav file processing, sophisticated analytical tools, publication-quality visualizations, and meta-cognitive self-monitoring for advanced data science workflows.
