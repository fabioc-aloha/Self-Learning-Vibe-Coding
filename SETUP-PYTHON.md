# Python Cognitive Architecture Auto-Setup Guide

**INSTRUCTIONS FOR GITHUB COPILOT**: This file contains complete setup instructions for implementing the Self-Learning Vibe Coding cognitive memory architecture optimized for Python programming with .venv virtual environments. Follow these instructions to create all necessary directories, files, and configurations.

## 🐍 Python Automated Setup Protocol

**Execute these steps in order to establish a complete cognitive architecture system for Python development:**

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
  "files.associations": {
    "*.py": "python",
    "requirements*.txt": "pip-requirements",
    "Pipfile": "toml",
    "pyproject.toml": "toml"
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
│   │   ├── python.instructions.md
│   │   ├── testing.instructions.md
│   │   ├── documentation.instructions.md
│   │   ├── packaging.instructions.md
│   │   ├── data-science.instructions.md
│   │   ├── learning.instructions.md     # Meta-Cognitive Learning
│   │   └── meta-cognition.instructions.md  # Self-Monitoring
│   └── prompts/                         # Episodic Memory Store
│       ├── code-review.prompt.md
│       ├── debugging.prompt.md
│       ├── refactoring.prompt.md
│       ├── testing.prompt.md
│       ├── data-analysis.prompt.md
│       ├── package-development.prompt.md
│       ├── consolidation.prompt.md
│       ├── performance-optimization.prompt.md
│       ├── environment-setup.prompt.md
│       ├── self-assessment.prompt.md    # Meta-Cognitive Assessment
│       ├── meta-learning.prompt.md      # Learning Strategy Evolution
│       └── cognitive-health.prompt.md   # Architecture Maintenance
├── .venv/                               # Virtual Environment
├── src/                                 # Source Code
├── tests/                               # Test Files
├── requirements.txt                     # Dependencies
├── requirements-dev.txt                 # Development Dependencies
├── .env                                 # Environment Variables
├── .gitignore                          # Git Ignore
└── pyproject.toml                      # Project Configuration
```

### Step 3: Python Environment Setup

**Create virtual environment and basic project structure:**

```powershell
# Create virtual environment
python -m venv .venv

# Activate virtual environment (Windows PowerShell)
.venv\Scripts\Activate.ps1

# Upgrade pip
python -m pip install --upgrade pip

# Create basic project structure
New-Item -ItemType Directory -Force -Path "src", "tests"

# Create requirements files
@"
# Core dependencies
requests>=2.31.0
python-dotenv>=1.0.0
"@ | Out-File -FilePath "requirements.txt" -Encoding utf8

@"
# Development dependencies
pytest>=7.4.0
pytest-cov>=4.1.0
black>=23.0.0
flake8>=6.0.0
pylint>=2.17.0
mypy>=1.5.0
pre-commit>=3.4.0
jupyter>=1.0.0
"@ | Out-File -FilePath "requirements-dev.txt" -Encoding utf8

# Install development dependencies
pip install -r requirements-dev.txt

# Create .env file
@"
# Environment variables
PYTHONPATH=src
DEBUG=True
"@ | Out-File -FilePath ".env" -Encoding utf8

# Create .gitignore
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

# Jupyter
.ipynb_checkpoints/

# OS
.DS_Store
Thumbs.db
"@ | Out-File -FilePath ".gitignore" -Encoding utf8

# Create pyproject.toml
@"
[build-system]
requires = ["setuptools>=45", "wheel"]
build-backend = "setuptools.build_meta"

[project]
name = "python-project"
version = "0.1.0"
description = "Python project with cognitive architecture"
requires-python = ">=3.8"

[tool.black]
line-length = 88
target-version = ['py38']

[tool.pytest.ini_options]
testpaths = ["tests"]
python_files = ["test_*.py"]
python_classes = ["Test*"]
python_functions = ["test_*"]
addopts = "--cov=src --cov-report=html --cov-report=term"

[tool.mypy]
python_version = "3.8"
warn_return_any = true
warn_unused_configs = true
disallow_untyped_defs = true
"@ | Out-File -FilePath "pyproject.toml" -Encoding utf8
```

### Step 4: Global Python Declarative Memory Setup

**Create `.github/copilot-instructions.md`** with this exact content:

```markdown
# Self-Learning Vibe Coding - Python Cognitive Memory Architecture

IMPORTANT: This file serves as Global Python Declarative Memory. Keep minimal and efficient. Detailed execution resides in specialized memory files.

## 🧠 Python Cognitive Architecture Status

**Working Memory**: 4/4 rules (at optimal capacity for Python development)
**Consolidation**: Auto-trigger when exceeding capacity
**Memory Distribution**: Active across Python procedural (.instructions.md) and development episodic (.prompt.md) systems

## 🚀 Python Working Memory - Quick Reference (Limit: 4 Critical Rules)

| Priority | Rule | Load | Auto-Consolidate |
|----------|------|------|------------------|
| P1 | `@pythonic` - Follow Python PEP standards and Pythonic idioms | Low | Never |
| P2 | `@venv` - Always use .venv virtual environment for dependencies | Medium | >30 days unused |
| P3 | `@meditation` - Auto-consolidate when working memory capacity exceeded | High | When triggered |
| P4 | `@testing` - Write comprehensive tests with pytest and maintain coverage | Medium | When obsolete |

## 🎯 Python Cognitive Architecture Coordination

### Multi-Modal Python Memory Distribution

**Procedural Memory Activation** (Context-Dependent):
- `python.instructions.md` → Python standards and best practices for .py files, PEP compliance
- `testing.instructions.md` → Testing patterns for test_*.py files, pytest configurations
- `documentation.instructions.md` → Documentation standards for README, docstrings, API docs
- `packaging.instructions.md` → Package management for setup.py, requirements.txt, pyproject.toml
- `data-science.instructions.md` → Data science patterns for .ipynb, pandas, numpy workflows
- `learning.instructions.md` → Meta-cognitive learning and self-monitoring protocols
- `meta-cognition.instructions.md` → Self-awareness and cognitive monitoring patterns

**Episodic Memory Activation** (Problem-Solving):
- `code-review.prompt.md` → Systematic Python code review and quality assessment workflows
- `debugging.prompt.md` → Python debugging and troubleshooting procedures with pdb
- `refactoring.prompt.md` → Python code refactoring and optimization methodologies
- `testing.prompt.md` → Comprehensive testing workflows with pytest and coverage
- `data-analysis.prompt.md` → Data analysis and visualization workflows
- `package-development.prompt.md` → Python package creation and distribution
- `consolidation.prompt.md` → Memory consolidation and cognitive architecture optimization
- `performance-optimization.prompt.md` → Python performance analysis and optimization
- `environment-setup.prompt.md` → Virtual environment and dependency management
- `self-assessment.prompt.md` → Cognitive performance evaluation and improvement
- `meta-learning.prompt.md` → Learning strategy development and evolution
- `cognitive-health.prompt.md` → Architecture health monitoring and maintenance

### Auto-Consolidation Triggers

- Working memory > 4 rules → Execute consolidation.prompt.md
- Rule conflicts detected → Activate learning.instructions.md
- Performance degradation → Review and redistribute memory load
- User requests meditation → Full cognitive architecture optimization
- **Virtual environment issues → Execute environment-setup.prompt.md**
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
| python.instructions.md | Python Standards | *.py, PEP compliance | Auto-tracked |
| testing.instructions.md | Testing & QA | test_*.py, pytest | Auto-tracked |
| documentation.instructions.md | Documentation | *.md, docstrings | Auto-tracked |
| packaging.instructions.md | Package Management | setup.py, requirements.txt | Auto-tracked |
| data-science.instructions.md | Data Science | *.ipynb, pandas, numpy | Auto-tracked |
| learning.instructions.md | Meta-Learning | *instructions*, *learning* | Auto-tracked |
| meta-cognition.instructions.md | Self-Monitoring | *meta*, *monitor*, *assess* | Auto-tracked |

### Episodic Memory Store (.github/prompts/)
| File | Workflow Type | Complexity Level | Usage Frequency |
|------|---------------|------------------|-----------------|
| code-review.prompt.md | Python Code Review | High | Auto-tracked |
| debugging.prompt.md | Python Debugging | High | Auto-tracked |
| refactoring.prompt.md | Code Optimization | Medium | Auto-tracked |
| testing.prompt.md | Testing Workflows | High | Auto-tracked |
| data-analysis.prompt.md | Data Analysis | Medium | Auto-tracked |
| package-development.prompt.md | Package Creation | Medium | Auto-tracked |
| consolidation.prompt.md | Memory Optimization | High | Auto-tracked |
| performance-optimization.prompt.md | Performance Analysis | Medium | Auto-tracked |
| environment-setup.prompt.md | Environment Management | Medium | Auto-tracked |
| self-assessment.prompt.md | Self-Evaluation | High | Auto-tracked |
| meta-learning.prompt.md | Learning Evolution | High | Auto-tracked |
| cognitive-health.prompt.md | Health Monitoring | Medium | Auto-tracked |

### Memory Transfer Protocol Status
- **Active Files**: 19 specialized memory files (7 procedural + 12 episodic)
- **Last Consolidation**: Setup initialization with Python-specific meta-cognitive enhancements
- **Cognitive Load Status**: Optimized through distributed processing with Python-specific patterns
- **Index Synchronization**: Maintained automatically during consolidation
- **Meta-Cognitive Status**: Fully operational with self-assessment and learning evolution capabilities

---

*Global Declarative Memory Component - Coordinates distributed cognitive architecture while maintaining optimal working memory efficiency. Detailed execution protocols reside in specialized memory files.*
```

### Step 5: Procedural Memory Files

#### Create `.github/instructions/python.instructions.md`:

```markdown
---
applyTo: "**/*.py,**/setup.py,**/conftest.py"
description: "Python standards and development best practices"
---

# Python Standards Procedural Memory

## PEP Compliance and Code Style
- Follow PEP 8 style guidelines for code formatting
- Use PEP 257 conventions for docstrings
- Apply PEP 484 type hints for function parameters and return values
- Follow PEP 20 (Zen of Python) principles for code design
- Use Black formatter with 88-character line length

## Pythonic Programming Patterns
- Use list comprehensions and generator expressions appropriately
- Prefer context managers (with statements) for resource management
- Use enumerate() instead of manual indexing in loops
- Apply duck typing and EAFP (Easier to Ask for Forgiveness than Permission)
- Utilize built-in functions and standard library modules

## Code Organization and Structure
- Organize imports: standard library, third-party, local imports
- Use __init__.py files to create packages
- Follow single responsibility principle for functions and classes
- Use meaningful names that describe purpose and behavior
- Keep functions focused and limit to 20-30 lines when possible

## Error Handling and Debugging
- Use specific exception types rather than broad except clauses
- Implement proper logging with the logging module
- Use assert statements for debugging and testing assumptions
- Handle edge cases and validate input parameters
- Provide meaningful error messages and context

## Performance and Memory Optimization
- Use generators for large datasets to save memory
- Leverage itertools for efficient iteration patterns
- Profile code with cProfile or line_profiler
- Use slots for classes with fixed attributes
- Consider numpy arrays for numerical computations
```

#### Create `.github/instructions/testing.instructions.md`:

```markdown
---
applyTo: "**/test_*.py,**/tests/**,**/conftest.py"
description: "Python testing patterns and pytest best practices"
---

# Python Testing Procedural Memory

## Pytest Framework Standards
- Use pytest fixtures for test setup and teardown
- Organize tests with clear arrange-act-assert pattern
- Use parametrize decorator for testing multiple scenarios
- Implement conftest.py for shared fixtures and configuration
- Use meaningful test function names that describe what is tested

## Test Organization and Structure
- Group related tests in classes using TestClass naming
- Use descriptive test method names: test_should_do_something_when_condition
- Create separate test files for each module being tested
- Organize tests to mirror source code structure
- Use pytest marks to categorize and filter tests

## Coverage and Quality Standards
- Maintain minimum 80% code coverage for critical modules
- Test both happy path and error scenarios
- Include edge cases and boundary condition testing
- Use mock objects to isolate units under test
- Write integration tests for API endpoints and database operations

## Fixtures and Test Data Management
- Create reusable fixtures for common test data
- Use factory_boy or similar for generating test objects
- Implement database fixtures with proper cleanup
- Use temporary files and directories for file system tests
- Mock external services and APIs in tests

## Performance and CI Integration
- Keep individual tests fast (under 100ms when possible)
- Use pytest-xdist for parallel test execution
- Implement smoke tests for critical functionality
- Configure pytest in pyproject.toml for consistency
- Generate coverage reports in multiple formats (HTML, XML)
```

#### Create `.github/instructions/packaging.instructions.md`:

```markdown
---
applyTo: "**/setup.py,**/pyproject.toml,**/requirements*.txt,**/Pipfile"
description: "Python package management and distribution best practices"
---

# Python Packaging Procedural Memory

## Dependency Management
- Use requirements.txt for production dependencies
- Maintain requirements-dev.txt for development dependencies
- Pin exact versions for production: package==1.2.3
- Use version ranges for development: package>=1.2.0,<2.0.0
- Regularly update dependencies and test compatibility

## Virtual Environment Best Practices
- Always use .venv for virtual environments
- Include .venv/ in .gitignore
- Document Python version requirements clearly
- Use python -m venv instead of virtualenv for consistency
- Activate environment before installing dependencies

## Project Configuration
- Use pyproject.toml for modern Python project configuration
- Define build system requirements and backend
- Configure tool settings (black, pytest, mypy) in pyproject.toml
- Include project metadata: name, version, description, author
- Specify minimum Python version requirements

## Package Distribution
- Follow semantic versioning (MAJOR.MINOR.PATCH)
- Include comprehensive README.md with installation and usage
- Create CHANGELOG.md documenting version changes
- Use setup.py or pyproject.toml for package building
- Test package installation in clean environments

## Security and Maintenance
- Use pip-audit to check for security vulnerabilities
- Implement automated dependency updates with Dependabot
- Scan for outdated packages with pip-outdated
- Use safety package for security vulnerability checking
- Document security policies and vulnerability reporting
```

#### Create `.github/instructions/data-science.instructions.md`:

```markdown
---
applyTo: "**/*.ipynb,**/notebooks/**,**/data/**"
description: "Data science and machine learning patterns with Python"
---

# Data Science Procedural Memory

## Jupyter Notebook Best Practices
- Use meaningful cell organization with markdown headers
- Clear all outputs before committing to version control
- Include data source documentation and methodology
- Use consistent naming conventions for variables
- Add markdown cells explaining complex analysis steps

## Pandas and Data Manipulation
- Use vectorized operations instead of loops when possible
- Check data types and handle missing values explicitly
- Use meaningful column names and index labels
- Implement data validation and quality checks
- Document data transformation steps with comments

## NumPy and Scientific Computing
- Use numpy arrays for numerical computations
- Leverage broadcasting for efficient array operations
- Choose appropriate data types to optimize memory usage
- Use numpy's random module with fixed seeds for reproducibility
- Profile memory usage for large datasets

## Visualization and Reporting
- Use matplotlib/seaborn for static visualizations
- Create reusable plotting functions for consistency
- Include proper titles, labels, and legends
- Use appropriate color schemes and accessibility considerations
- Export plots in high-resolution formats for publications

## Machine Learning Workflows
- Implement proper train/validation/test splits
- Use cross-validation for model evaluation
- Document feature engineering and selection processes
- Track experiments with MLflow or similar tools
- Validate model performance with appropriate metrics
```

### Step 6: Episodic Memory Files

#### Create `.github/prompts/testing.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "run_in_terminal", "read_file", "get_errors"]
description: "Comprehensive Python testing workflow with pytest"
---

# Python Testing Episode Template

## Phase 1: Test Planning and Setup
- Analyze code structure and identify testable units
- Plan test cases covering happy path, edge cases, and error scenarios
- Set up pytest configuration in pyproject.toml
- Create necessary fixtures and test data in conftest.py

## Phase 2: Test Implementation
- Write unit tests following arrange-act-assert pattern
- Implement integration tests for complex workflows
- Use parametrize for testing multiple input scenarios
- Mock external dependencies and services appropriately

## Phase 3: Coverage and Quality Validation
- Run pytest with coverage reporting
- Analyze coverage reports to identify untested code
- Add missing tests to achieve target coverage
- Validate test reliability and fix flaky tests

## Phase 4: CI/CD Integration
- Configure pytest for continuous integration
- Set up automated test execution on code changes
- Implement test result reporting and notifications
- Monitor test performance and optimize slow tests

Use Python-specific patterns from ${workspaceFolder}/.venv
```

#### Create `.github/prompts/data-analysis.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "run_in_terminal", "read_file", "create_file"]
description: "Data analysis and visualization workflow"
---

# Data Analysis Episode Template

## Phase 1: Data Exploration and Understanding
- Load and inspect data structure, types, and quality
- Identify missing values, outliers, and data anomalies
- Generate descriptive statistics and initial visualizations
- Document data source and collection methodology

## Phase 2: Data Cleaning and Preprocessing
- Handle missing values with appropriate strategies
- Detect and address outliers based on domain knowledge
- Transform data types and normalize scales as needed
- Create derived features and engineered variables

## Phase 3: Analysis and Modeling
- Apply appropriate statistical or machine learning methods
- Validate assumptions and check model diagnostics
- Implement cross-validation and performance evaluation
- Document methodology and parameter choices

## Phase 4: Visualization and Reporting
- Create clear, informative visualizations
- Generate summary statistics and key findings
- Document insights and recommendations
- Prepare reproducible analysis scripts

Use Python data science libraries from ${workspaceFolder}/.venv
```

#### Create `.github/prompts/package-development.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "run_in_terminal", "create_file", "read_file"]
description: "Python package creation and distribution workflow"
---

# Package Development Episode Template

## Phase 1: Project Structure Setup
- Create proper package directory structure
- Configure pyproject.toml with build system and metadata
- Set up virtual environment and development dependencies
- Initialize version control and .gitignore

## Phase 2: Code Organization and Documentation
- Organize modules and packages logically
- Write comprehensive docstrings for all public APIs
- Create usage examples and API documentation
- Implement proper __init__.py files for packages

## Phase 3: Testing and Quality Assurance
- Develop comprehensive test suite with pytest
- Set up continuous integration for multiple Python versions
- Implement code quality checks (black, flake8, mypy)
- Achieve target code coverage and documentation standards

## Phase 4: Distribution and Maintenance
- Build and test package in clean environments
- Configure PyPI publishing with proper metadata
- Create release notes and version management
- Set up automated dependency updates and security scanning

Use Python packaging tools from ${workspaceFolder}/.venv
```

#### Create `.github/prompts/environment-setup.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "run_in_terminal", "read_file", "create_file"]
description: "Python virtual environment and dependency management workflow"
---

# Environment Setup Episode Template

## Phase 1: Virtual Environment Creation
- Create .venv virtual environment in project root
- Activate environment and upgrade pip to latest version
- Configure VS Code Python interpreter to use .venv
- Set up environment variables in .env file

## Phase 2: Dependency Management
- Create requirements.txt for production dependencies
- Set up requirements-dev.txt for development tools
- Install and configure development tools (pytest, black, flake8)
- Pin dependency versions for reproducible environments

## Phase 3: Configuration and Tools
- Configure pyproject.toml for tool settings
- Set up pre-commit hooks for code quality
- Configure IDE settings for Python development
- Create .gitignore with Python-specific patterns

## Phase 4: Validation and Documentation
- Test environment setup in clean state
- Document installation and setup procedures
- Validate all development tools work correctly
- Create troubleshooting guide for common issues

Use Python environment management from ${workspaceFolder}/.venv
```

#### Create additional episodic memory files by copying and adapting from the coding setup:

```markdown
# Copy and adapt these files from SETUP-CODING.md:
# - .github/prompts/code-review.prompt.md (adapt for Python-specific patterns)
# - .github/prompts/debugging.prompt.md (adapt for Python debugging with pdb)
# - .github/prompts/refactoring.prompt.md (adapt for Python refactoring patterns)
# - .github/prompts/consolidation.prompt.md (same meta-cognitive content)
# - .github/prompts/performance-optimization.prompt.md (adapt for Python performance)
# - .github/prompts/self-assessment.prompt.md (same meta-cognitive content)
# - .github/prompts/meta-learning.prompt.md (same meta-cognitive content)
# - .github/prompts/cognitive-health.prompt.md (same meta-cognitive content)
```

## 🎯 Setup Validation

After creating all files, verify setup:

1. **Check virtual environment**: Ensure `.venv` is created and activated
2. **Validate dependencies**: Confirm all packages in requirements-dev.txt are installed
3. **Test VS Code integration**: Verify Python interpreter points to `.venv/Scripts/python.exe`
4. **Check instruction files**: Ensure all `.github/instructions/` files exist
5. **Verify episodic templates**: Confirm all `.github/prompts/` files are created

## 🚀 Quick Start Commands

After setup, test with these commands in GitHub Copilot:

**Environment Tests**:
- `@workspace Set up my Python virtual environment` (Should activate environment-setup.prompt.md)
- `Help me install and configure development dependencies` (Should activate packaging.instructions.md)

**Development Tests**:
- `Create a Python class following best practices` (Should activate python.instructions.md)
- `Write comprehensive tests for this function` (Should activate testing.prompt.md)
- `Help me debug this Python error` (Should activate debugging.prompt.md)

**Data Science Tests**:
- `Analyze this dataset and create visualizations` (Should activate data-analysis.prompt.md)
- `Set up a Jupyter notebook for data exploration` (Should activate data-science.instructions.md)

**Meta-Cognition Tests**:
- `@workspace Please assess your Python development performance` (Should activate self-assessment.prompt.md)
- `How can you improve your Python learning strategies?` (Should activate meta-learning.prompt.md)
- `Check the health of your cognitive architecture` (Should activate cognitive-health.prompt.md)

## ⚡ Success Indicators

Your Python cognitive architecture is working when:
- Virtual environment is properly configured and isolated
- Python code follows PEP standards automatically
- Testing workflows are systematic and comprehensive
- Data analysis follows scientific methodology
- Package management is consistent and reproducible
- **Meta-cognitive capabilities**: The AI can assess its Python development performance
- **Self-monitoring**: The system tracks Python-specific patterns and optimizes
- **Learning evolution**: The AI improves its Python strategies over time
- **Environment awareness**: The system manages .venv dependencies automatically

## 🔄 Maintenance

- Update dependencies regularly with `pip install --upgrade -r requirements-dev.txt`
- Run `pip freeze > requirements.txt` after adding new dependencies
- Execute consolidation meditation when adding 5+ new Python patterns
- Monitor virtual environment health and recreate if corrupted
- **Execute self-assessment weekly to monitor Python development cognitive health**
- **Run meta-learning analysis monthly for Python strategy optimization**
- **Perform cognitive architecture health checks quarterly**
- **Update Python-specific capabilities based on performance data**

---

**PYTHON SETUP COMPLETE**: Your adaptive AI Python development partner is now ready with .venv virtual environment management, comprehensive testing workflows, data science capabilities, and meta-cognitive self-monitoring for Python programming excellence.
