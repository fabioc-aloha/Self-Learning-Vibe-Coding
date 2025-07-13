# Business Requirements & Technical Documentation Cognitive Architecture Setup Guide

**INSTRUCTIONS FOR GITHUB COPILOT**: This file contains complete setup instructions for implementing the Self-Learning Vibe Coding cognitive memory architecture optimized for Business Requirements Documents (BRD), technical implementation documentation, and Azure data solutions including BI, database development, and data pipeline implementation.

## 📊 Business Requirements & Technical Documentation Automated Setup Protocol

**Execute these steps in order to establish a complete cognitive architecture system for BRD and technical documentation:**

### Step 1: VS Code Configuration (Required)

Add these settings to VS Code `settings.json`:

```json
{
  "github.copilot.chat.codeGeneration.useInstructionFiles": true,
  "chat.promptFiles": true,
  "chat.instructionsFilesLocations": [".github/instructions"],
  "markdown.extension.toc.levels": "1..6",
  "markdown.extension.preview.autoShowPreviewToSide": true,
  "cSpell.language": "en-US",
  "cSpell.enableFiletypes": ["markdown", "sql", "python", "json", "yaml"],
  "rewrap.wrappingColumn": 100,
  "editor.rulers": [80, 100, 120],
  "files.associations": {
    "*.brd": "markdown",
    "*.requirements": "markdown",
    "*.specification": "markdown"
  }
}
```

**Access settings.json**: `Ctrl+Shift+P` → "Preferences: Open User Settings (JSON)"

### Step 2: Create BRD & Technical Documentation Directory Structure

Create this exact folder structure in the project root:

```
project-root/
├── .github/
│   ├── copilot-instructions.md          # Global BRD Memory
│   ├── instructions/                    # BRD Procedural Memory
│   │   ├── brd-standards.instructions.md
│   │   ├── requirements-analysis.instructions.md
│   │   ├── azure-architecture.instructions.md
│   │   ├── data-modeling.instructions.md
│   │   ├── bi-development.instructions.md
│   │   ├── pipeline-design.instructions.md
│   │   ├── technical-documentation.instructions.md
│   │   ├── stakeholder-communication.instructions.md
│   │   ├── learning.instructions.md     # Meta-Cognitive Learning
│   │   └── meta-cognition.instructions.md  # Self-Monitoring
│   └── prompts/                         # BRD Episodic Memory
│       ├── requirements-gathering.prompt.md
│       ├── brd-creation.prompt.md
│       ├── technical-specification.prompt.md
│       ├── data-architecture-design.prompt.md
│       ├── bi-solution-design.prompt.md
│       ├── pipeline-implementation.prompt.md
│       ├── stakeholder-review.prompt.md
│       ├── implementation-planning.prompt.md
│       ├── testing-strategy.prompt.md
│       ├── consolidation.prompt.md
│       ├── self-assessment.prompt.md    # Meta-Cognitive Assessment
│       ├── meta-learning.prompt.md      # Learning Strategy Evolution
│       └── cognitive-health.prompt.md   # Architecture Maintenance
```

### Step 3: Global BRD Declarative Memory Setup

**Create `.github/copilot-instructions.md`** with this exact content:

```markdown
# Self-Learning Vibe Coding - Business Requirements & Technical Documentation Cognitive Architecture

IMPORTANT: This file serves as Global BRD Declarative Memory. Optimized for business analysis, requirements documentation, and Azure data solution implementation.

## 🧠 BRD Cognitive Architecture Status

**Working Memory**: 4/4 rules (at optimal capacity for business requirements and technical documentation)
**Consolidation**: Auto-trigger when exceeding capacity
**Memory Distribution**: Active across BRD procedural (.instructions.md) and implementation episodic (.prompt.md) systems

## 📊 BRD Working Memory - Quick Reference (Limit: 4 Critical Rules)

| Priority | Rule | Load | Auto-Consolidate |
|----------|------|------|------------------|
| P1 | `@stakeholder` - Align all requirements with stakeholder business objectives and success criteria | Low | Never |
| P2 | `@azure` - Leverage Azure-native solutions and best practices for scalability and cost optimization | Medium | >30 days unused |
| P3 | `@meditation` - Auto-consolidate when working memory capacity exceeded | High | When triggered |
| P4 | `@traceability` - Maintain clear traceability from business requirements to technical implementation | Medium | When obsolete |

## 🎯 BRD Cognitive Architecture Coordination

### BRD Procedural Memory Activation (Context-Dependent):
- `brd-standards.instructions.md` → BRD formatting for *.brd, *.requirements, *business* files
- `requirements-analysis.instructions.md` → Analysis for *requirements*, *analysis*, *specification* files  
- `azure-architecture.instructions.md` → Azure solutions for *azure*, *cloud*, *architecture* files
- `data-modeling.instructions.md` → Data design for *data*, *model*, *schema*, *database* files
- `bi-development.instructions.md` → BI solutions for *bi*, *analytics*, *dashboard*, *report* files
- `pipeline-design.instructions.md` → ETL/ELT for *pipeline*, *etl*, *data-flow*, *integration* files
- `technical-documentation.instructions.md` → Tech docs for *technical*, *implementation*, *deployment* files
- `stakeholder-communication.instructions.md` → Communication for *stakeholder*, *review*, *presentation* files
- `learning.instructions.md` → Meta-cognitive learning for *instructions*, *learning* files
- `meta-cognition.instructions.md` → Self-awareness for *meta*, *monitor*, *assess* files

### BRD Episodic Memory Activation (Implementation Workflows):
- `requirements-gathering.prompt.md` → Structured requirements elicitation from stakeholders
- `brd-creation.prompt.md` → Comprehensive BRD development and documentation
- `technical-specification.prompt.md` → Technical implementation specification creation
- `data-architecture-design.prompt.md` → Data architecture and modeling workflows
- `bi-solution-design.prompt.md` → Business intelligence solution development
- `pipeline-implementation.prompt.md` → Data pipeline design and implementation
- `stakeholder-review.prompt.md` → Stakeholder presentation and feedback incorporation
- `implementation-planning.prompt.md` → Project planning and delivery strategy
- `testing-strategy.prompt.md` → QA and validation planning
- `consolidation.prompt.md` → BRD memory optimization
- `self-assessment.prompt.md` → BRD performance evaluation
- `meta-learning.prompt.md` → Requirements strategy development
- `cognitive-health.prompt.md` → BRD architecture maintenance

### BRD Auto-Consolidation Triggers

- Working memory > 4 rules → Execute consolidation.prompt.md
- Stakeholder conflicts detected → Activate stakeholder-communication.instructions.md
- Technical complexity exceeds capacity → Review and redistribute BRD memory load
- User requests meditation → Full BRD cognitive architecture optimization
- **BRD performance assessment needed → Execute self-assessment.prompt.md**
- **Requirements strategy evolution required → Execute meta-learning.prompt.md**
- **BRD architecture health check → Execute cognitive-health.prompt.md**

## 🔄 BRD Memory Transfer Protocol

**Immediate Transfer**: Critical stakeholder misalignment → Quick Reference (P1-P4)
**Gradual Consolidation**: Repeated analysis patterns → BRD procedural memory (.instructions.md)
**Complex Implementation Workflows**: Multi-phase projects → BRD episodic memory (.prompt.md)
**Archive Management**: Obsolete requirements → Historical storage in specialized files
**Index Maintenance**: Auto-update BRD Long-Term Memory Index during transfers

## 📚 BRD Long-Term Memory Index

### BRD Procedural Memory Store (.github/instructions/)
| File | Domain | Activation Pattern | Last Updated |
|------|--------|-------------------|--------------|
| brd-standards.instructions.md | BRD Formatting | *.brd, *.requirements, *business* | Auto-tracked |
| requirements-analysis.instructions.md | Requirements Analysis | *requirements*, *analysis*, *specification* | Auto-tracked |
| azure-architecture.instructions.md | Azure Solutions | *azure*, *cloud*, *architecture* | Auto-tracked |
| data-modeling.instructions.md | Data Design | *data*, *model*, *schema*, *database* | Auto-tracked |
| bi-development.instructions.md | BI Solutions | *bi*, *analytics*, *dashboard*, *report* | Auto-tracked |
| pipeline-design.instructions.md | Data Pipelines | *pipeline*, *etl*, *data-flow*, *integration* | Auto-tracked |
| technical-documentation.instructions.md | Tech Documentation | *technical*, *implementation*, *deployment* | Auto-tracked |
| stakeholder-communication.instructions.md | Communication | *stakeholder*, *review*, *presentation* | Auto-tracked |
| learning.instructions.md | Meta-Learning | *instructions*, *learning* | Auto-tracked |
| meta-cognition.instructions.md | Self-Monitoring | *meta*, *monitor*, *assess* | Auto-tracked |

### BRD Episodic Memory Store (.github/prompts/)
| File | Implementation Workflow | Complexity Level | Usage Frequency |
|------|-------------------------|------------------|-----------------|
| requirements-gathering.prompt.md | Requirements Elicitation | High | Auto-tracked |
| brd-creation.prompt.md | BRD Development | High | Auto-tracked |
| technical-specification.prompt.md | Technical Documentation | High | Auto-tracked |
| data-architecture-design.prompt.md | Data Architecture | High | Auto-tracked |
| bi-solution-design.prompt.md | BI Development | High | Auto-tracked |
| pipeline-implementation.prompt.md | Data Pipelines | High | Auto-tracked |
| stakeholder-review.prompt.md | Stakeholder Management | Medium | Auto-tracked |
| implementation-planning.prompt.md | Project Planning | Medium | Auto-tracked |
| testing-strategy.prompt.md | QA Strategy | Medium | Auto-tracked |
| consolidation.prompt.md | Memory Optimization | High | Auto-tracked |
| self-assessment.prompt.md | Performance Evaluation | High | Auto-tracked |
| meta-learning.prompt.md | Strategy Evolution | High | Auto-tracked |
| cognitive-health.prompt.md | Health Monitoring | Medium | Auto-tracked |

### BRD Memory Transfer Protocol Status
- **Active Files**: 23 specialized BRD memory files (10 procedural + 13 episodic)
- **Last Consolidation**: BRD architecture initialization with meta-cognitive enhancements
- **Cognitive Load Status**: Optimized for business analysis and technical implementation
- **Index Synchronization**: Maintained automatically during consolidation
- **Meta-Cognitive Status**: Fully operational with BRD performance assessment and requirements strategy evolution

---

*Global BRD Declarative Memory Component - Coordinates distributed BRD cognitive architecture while maintaining optimal business analysis efficiency. Detailed implementation protocols reside in specialized memory files.*
```

### Step 4: BRD Procedural Memory Files

#### Create `.github/instructions/brd-standards.instructions.md`:

```markdown
---
applyTo: "**/*.brd,**/*.requirements,**/*business*,**/*specification*"
description: "Business Requirements Document standards and formatting"
---

# BRD Standards Procedural Memory

## BRD Document Structure
- Executive Summary with business objectives and expected ROI
- Business Context and Problem Statement with quantified impact
- Stakeholder Analysis with roles, responsibilities, and success criteria
- Functional Requirements with acceptance criteria and priority levels
- Non-Functional Requirements including performance, security, and scalability
- Data Requirements with sources, quality, and governance considerations
- Integration Requirements with existing systems and external dependencies
- Implementation Timeline with phases, milestones, and dependencies
- Risk Assessment with mitigation strategies and contingency plans
- Approval and Sign-off section with stakeholder validation

## Requirements Writing Standards
- Use clear, unambiguous language avoiding technical jargon
- Write testable requirements with measurable acceptance criteria
- Apply SMART criteria (Specific, Measurable, Achievable, Relevant, Time-bound)
- Include priority classification (Must Have, Should Have, Could Have, Won't Have)
- Reference source documentation and stakeholder interviews
- Maintain unique requirement IDs for traceability throughout project lifecycle

## Business Process Documentation
- Document current state processes with pain points and inefficiencies
- Define future state processes with improvements and optimizations
- Create process flow diagrams using standard notation (BPMN 2.0)
- Identify process owners, participants, and system touchpoints
- Document business rules and decision logic clearly
- Include exception handling and error scenarios

## Stakeholder Requirements Management
- Identify all impacted stakeholder groups and their specific needs
- Document conflicting requirements and resolution strategies
- Maintain requirements traceability matrix linking business needs to technical solutions
- Establish change management process for requirement modifications
- Create communication plan for stakeholder engagement and feedback cycles
- Define success metrics and key performance indicators (KPIs)
```

#### Create `.github/instructions/requirements-analysis.instructions.md`:

```markdown
---
applyTo: "**/*requirements*,**/*analysis*,**/*specification*,**/*gap*"
description: "Requirements analysis and elicitation methodologies"
---

# Requirements Analysis Procedural Memory

## Requirements Elicitation Techniques
- Conduct structured stakeholder interviews with prepared questionnaires
- Facilitate requirements workshops with cross-functional teams
- Perform current state analysis through process observation and documentation
- Analyze existing documentation, reports, and system outputs
- Use questionnaires and surveys for broad stakeholder input
- Apply prototyping and mockups to validate understanding
- Conduct focus groups for user experience requirements
- Review competitor solutions and industry best practices

## Business Process Analysis
- Map current state processes using swimlane diagrams
- Identify process inefficiencies, bottlenecks, and manual workarounds
- Quantify current state metrics (time, cost, error rates, volume)
- Design future state processes with automation and optimization
- Calculate expected benefits and return on investment (ROI)
- Document process assumptions and dependencies
- Identify change management requirements for process adoption

## Gap Analysis and Solution Design
- Compare current capabilities against desired future state
- Identify functional, technical, and organizational gaps
- Prioritize gaps based on business impact and implementation complexity
- Evaluate build vs. buy vs. configure options for each gap
- Consider phased implementation approach for complex requirements
- Assess resource requirements and skill gaps
- Document integration points and data flow requirements

## Requirements Validation and Verification
- Conduct requirements reviews with subject matter experts
- Use walkthrough sessions to validate process understanding
- Create test scenarios to verify requirement completeness
- Apply requirements checklist to ensure quality standards
- Validate requirements against business objectives and constraints
- Confirm technical feasibility with development teams
- Establish acceptance criteria for each requirement category
```

#### Create `.github/instructions/azure-architecture.instructions.md`:

```markdown
---
applyTo: "**/*azure*,**/*cloud*,**/*architecture*,**/*infrastructure*"
description: "Azure cloud architecture and solution design best practices"
---

# Azure Architecture Procedural Memory

## Azure Data Platform Architecture
- Use Azure Synapse Analytics for enterprise data warehousing and big data analytics
- Implement Azure Data Factory for orchestrating data movement and transformation
- Leverage Azure Data Lake Storage Gen2 for scalable data lake solutions
- Apply Azure SQL Database for transactional workloads with built-in intelligence
- Use Azure Analysis Services for semantic modeling and self-service BI
- Implement Azure Cosmos DB for globally distributed, multi-model data solutions
- Consider Azure SQL Managed Instance for lift-and-shift scenarios

## Data Integration and Pipeline Design
- Design hub-and-spoke architecture for centralized data management
- Implement medallion architecture (Bronze, Silver, Gold) for data lake organization
- Use Azure Data Factory pipelines for batch and real-time data processing
- Apply Azure Stream Analytics for real-time data streaming and analytics
- Implement change data capture (CDC) for incremental data loading
- Use Azure Logic Apps for workflow automation and system integration
- Consider Azure Event Hubs for high-throughput event ingestion

## Security and Governance Framework
- Implement Azure Active Directory for identity and access management
- Use Azure Key Vault for secure secrets and certificate management
- Apply Azure Private Link for secure connectivity to Azure services
- Implement Azure Purview for data governance and lineage tracking
- Use Azure Policy for compliance and governance enforcement
- Apply role-based access control (RBAC) with principle of least privilege
- Implement data classification and sensitivity labeling

## Performance and Cost Optimization
- Right-size Azure resources based on actual usage patterns
- Implement auto-scaling for variable workload demands
- Use Azure Cost Management for monitoring and optimization
- Apply data archiving strategies for cost-effective long-term storage
- Implement query optimization and indexing strategies
- Use Azure Advisor recommendations for performance improvements
- Consider Reserved Instances and Azure Hybrid Benefit for cost savings
```

#### Create `.github/instructions/data-modeling.instructions.md`:

```markdown
---
applyTo: "**/*data*,**/*model*,**/*schema*,**/*database*,**/*entity*"
description: "Data modeling and database design best practices"
---

# Data Modeling Procedural Memory

## Conceptual Data Modeling
- Identify and define business entities and their relationships
- Create entity-relationship diagrams (ERD) using standard notation
- Define business rules and constraints for data integrity
- Establish data definitions and business glossary
- Identify master data entities and reference data requirements
- Document data ownership and stewardship responsibilities
- Consider data privacy and regulatory compliance requirements

## Logical Data Modeling
- Transform conceptual model into normalized logical structure
- Apply normalization rules (1NF, 2NF, 3NF) to eliminate redundancy
- Define primary keys, foreign keys, and unique constraints
- Specify data types, lengths, and precision requirements
- Document business rules as check constraints and triggers
- Consider slowly changing dimensions for historical data tracking
- Design for data quality and validation requirements

## Physical Data Modeling for Azure SQL
- Optimize table structures for Azure SQL Database performance
- Design appropriate indexing strategy (clustered, non-clustered, columnstore)
- Implement partitioning for large tables and improved query performance
- Consider compression options for storage optimization
- Design for high availability and disaster recovery requirements
- Implement security through schemas, roles, and row-level security
- Plan for maintenance operations and index management

## Data Warehouse and Analytics Modeling
- Design star schema and snowflake schema for dimensional modeling
- Create fact tables with appropriate grain and measure selection
- Design dimension tables with slowly changing dimension handling
- Implement bridge tables for many-to-many relationships
- Consider aggregate tables and materialized views for performance
- Design for incremental loading and change data capture
- Plan for data lineage and impact analysis requirements
```

#### Create `.github/instructions/bi-development.instructions.md`:

```markdown
---
applyTo: "**/*bi*,**/*analytics*,**/*dashboard*,**/*report*,**/*powerbi*"
description: "Business Intelligence development and analytics best practices"
---

# BI Development Procedural Memory

## Data Architecture for BI Solutions
- Design semantic layer using Azure Analysis Services or Power BI datasets
- Implement proper data modeling with relationships and hierarchies
- Create calculated columns and measures using DAX expressions
- Design for performance with appropriate aggregations and partitions
- Implement security through row-level security (RLS) and object-level security
- Plan for scalability and concurrent user access
- Consider real-time vs. batch refresh requirements

## Dashboard and Report Design
- Follow data visualization best practices and design principles
- Select appropriate chart types for different data storytelling scenarios
- Implement consistent color schemes and branding guidelines
- Design responsive layouts for multiple device types
- Create intuitive navigation and user experience flows
- Apply progressive disclosure for complex analytical scenarios
- Include context and explanatory text for business users

## Performance Optimization
- Optimize data model size through summarization and aggregation
- Implement incremental refresh for large datasets
- Use appropriate storage modes (Import, DirectQuery, Composite)
- Design efficient DAX measures and calculated columns
- Implement query reduction techniques and caching strategies
- Monitor and tune report performance using built-in tools
- Consider Premium capacity features for enterprise scenarios

## Self-Service Analytics Enablement
- Create reusable datasets and semantic models
- Develop template reports and dashboard frameworks
- Implement data governance and certification processes
- Provide documentation and training materials for end users
- Establish center of excellence (CoE) for BI development
- Create standardized metrics and KPI definitions
- Implement feedback loops for continuous improvement
```

#### Create `.github/instructions/pipeline-design.instructions.md`:

```markdown
---
applyTo: "**/*pipeline*,**/*etl*,**/*data-flow*,**/*integration*,**/*airflow*"
description: "Data pipeline design and ETL/ELT implementation best practices"
---

# Pipeline Design Procedural Memory

## ETL/ELT Pipeline Architecture
- Design for both batch and real-time processing requirements
- Implement idempotent operations for reliable pipeline execution
- Use configuration-driven approaches for maintainable pipelines
- Apply proper error handling and retry mechanisms
- Implement monitoring and alerting for pipeline health
- Design for scalability and parallel processing
- Consider data lineage tracking and impact analysis

## Azure Data Factory Implementation
- Use parameterized pipelines for reusability and maintainability
- Implement proper trigger strategies (scheduled, event-based, tumbling window)
- Use mapping data flows for code-free data transformation
- Apply integration runtime optimization for performance
- Implement proper logging and monitoring through Azure Monitor
- Use Git integration for version control and CI/CD deployment
- Consider cost optimization through pipeline scheduling and resource management

## Data Quality and Validation
- Implement data quality checks at each stage of the pipeline
- Use data profiling to understand source data characteristics
- Apply business rule validation and constraint checking
- Implement exception handling for data quality failures
- Create data quality scorecards and reporting
- Use automated testing for pipeline validation
- Implement data reconciliation between source and target systems

## Python-Based Pipeline Development
- Use pandas for data manipulation and transformation
- Implement logging and monitoring using Python logging framework
- Apply configuration management for environment-specific settings
- Use virtual environments and requirements.txt for dependency management
- Implement unit testing for data transformation logic
- Apply PEP 8 coding standards for maintainable code
- Consider using Apache Airflow for complex workflow orchestration
```

#### Create `.github/instructions/technical-documentation.instructions.md`:

```markdown
---
applyTo: "**/*technical*,**/*implementation*,**/*deployment*,**/*architecture*"
description: "Technical documentation and implementation specification standards"
---

# Technical Documentation Procedural Memory

## System Architecture Documentation
- Create high-level architecture diagrams showing system components and interactions
- Document technology stack and infrastructure requirements
- Specify integration points and API contracts
- Include security architecture with authentication and authorization flows
- Document deployment architecture and environment configurations
- Specify monitoring and logging strategies
- Include disaster recovery and business continuity plans

## Implementation Specifications
- Provide detailed technical requirements with acceptance criteria
- Document database schemas with field definitions and constraints
- Specify API endpoints with request/response formats and error codes
- Include configuration parameters and environment variables
- Document dependencies and external system requirements
- Provide installation and setup instructions
- Include troubleshooting guides and known issues

## Database Implementation Documentation
- Document database design with entity relationship diagrams
- Specify indexing strategies and performance optimization approaches
- Include data migration scripts and procedures
- Document stored procedures, functions, and triggers
- Specify backup and recovery procedures
- Include capacity planning and scaling considerations
- Document security implementation including access controls

## Code Documentation and Standards
- Use inline comments for complex business logic and algorithms
- Create README files with project overview and setup instructions
- Document APIs using OpenAPI/Swagger specifications
- Include code examples and usage patterns
- Specify coding standards and style guidelines
- Document testing strategies and test case specifications
- Include change log and version history documentation
```

#### Create `.github/instructions/stakeholder-communication.instructions.md`:

```markdown
---
applyTo: "**/*stakeholder*,**/*review*,**/*presentation*,**/*communication*"
description: "Stakeholder communication and project management best practices"
---

# Stakeholder Communication Procedural Memory

## Stakeholder Analysis and Management
- Identify all stakeholders and their level of influence and interest
- Document stakeholder requirements and success criteria
- Create communication matrix with preferred methods and frequency
- Establish escalation paths for issue resolution
- Maintain stakeholder contact information and roles
- Track stakeholder feedback and requirement changes
- Plan for stakeholder onboarding and training

## Requirements Review and Approval Process
- Schedule regular review sessions with appropriate stakeholders
- Prepare structured agendas with clear objectives and outcomes
- Use visual aids and prototypes to facilitate understanding
- Document decisions and action items with assigned owners
- Obtain formal sign-off on requirements and specifications
- Manage requirement changes through change control process
- Communicate impacts of changes to timeline and budget

## Project Communication Planning
- Develop communication plan with stakeholder-specific messaging
- Create standard reporting templates for status updates
- Establish meeting cadence for different stakeholder groups
- Use project management tools for transparency and collaboration
- Implement risk and issue escalation procedures
- Plan for go-live communication and user adoption support
- Create feedback mechanisms for continuous improvement

## Business Case and Benefits Realization
- Develop compelling business case with quantified benefits
- Create executive summary highlighting key value propositions
- Track benefits realization metrics throughout implementation
- Report on ROI and success metrics to executive stakeholders
- Communicate lessons learned and best practices
- Plan for post-implementation review and optimization
- Document success stories and case studies for future projects
```

### Step 5: BRD Episodic Memory Files

#### Create `.github/prompts/requirements-gathering.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Structured requirements elicitation and stakeholder analysis workflow"
---

# Requirements Gathering Episode Template

## Phase 1: Stakeholder Identification and Analysis
- Identify all stakeholder groups and their roles in the organization
- Assess stakeholder influence, interest, and impact on project success
- Create stakeholder communication matrix with preferred engagement methods
- Document stakeholder availability and scheduling constraints
- Identify subject matter experts for each business domain
- Plan interview approach and questions tailored to each stakeholder group

## Phase 2: Requirements Elicitation Sessions
- Conduct structured interviews using prepared questionnaires
- Facilitate requirements workshops with cross-functional teams
- Perform current state process analysis and documentation
- Review existing documentation, reports, and system outputs
- Gather quantitative data on current performance metrics
- Document pain points, inefficiencies, and improvement opportunities

## Phase 3: Requirements Analysis and Validation
- Analyze gathered requirements for completeness and consistency
- Identify conflicting requirements and resolution strategies
- Prioritize requirements using MoSCoW or similar framework
- Validate requirements with stakeholders through review sessions
- Create requirements traceability matrix linking business needs to solutions
- Document assumptions, constraints, and dependencies

## Phase 4: Requirements Documentation and Approval
- Compile requirements into structured BRD format
- Create visual models and diagrams to support understanding
- Prepare executive summary highlighting key business benefits
- Facilitate stakeholder review and feedback incorporation
- Obtain formal approval and sign-off from authorized stakeholders
- Establish change control process for future requirement modifications

Focus on stakeholder alignment and business value realization
```

#### Create `.github/prompts/brd-creation.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "create_file", "read_file"]
description: "Comprehensive Business Requirements Document development workflow"
---

# BRD Creation Episode Template

## Phase 1: Document Structure and Planning
- Create BRD outline following organizational standards and templates
- Define document scope, objectives, and target audience
- Establish document review and approval process
- Plan visual elements including process diagrams and data flows
- Identify supporting documentation and appendices required
- Set up document version control and change tracking

## Phase 2: Business Context and Problem Definition
- Document current state business processes and pain points
- Quantify business impact of current state inefficiencies
- Define business objectives and success criteria with measurable KPIs
- Establish project scope and boundaries with clear inclusions/exclusions
- Document regulatory and compliance requirements
- Create business case with cost-benefit analysis and ROI projections

## Phase 3: Requirements Documentation and Specification
- Document functional requirements with detailed acceptance criteria
- Specify non-functional requirements including performance and security
- Create data requirements with source systems and quality specifications
- Document integration requirements with existing systems and external partners
- Specify user interface and user experience requirements
- Include reporting and analytics requirements with dashboard specifications

## Phase 4: Implementation Planning and Risk Assessment
- Create high-level implementation timeline with phases and milestones
- Identify project dependencies and critical path activities
- Assess project risks with probability, impact, and mitigation strategies
- Document resource requirements including skills and technology needs
- Plan stakeholder communication and change management approach
- Establish success metrics and post-implementation review criteria

Ensure comprehensive coverage while maintaining stakeholder focus
```

#### Create `.github/prompts/technical-specification.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "semantic_search", "create_file"]
description: "Technical implementation specification creation workflow"
---

# Technical Specification Episode Template

## Phase 1: Architecture Design and Technology Selection
- Design system architecture aligned with business requirements
- Select appropriate Azure services and technology stack
- Create detailed architecture diagrams showing component interactions
- Specify infrastructure requirements and sizing estimates
- Document security architecture and compliance considerations
- Plan for scalability, performance, and disaster recovery requirements

## Phase 2: Data Architecture and Integration Design
- Design data model supporting business requirements and analytics needs
- Specify data sources, formats, and integration patterns
- Create data flow diagrams showing transformation and movement
- Document API specifications for system integrations
- Plan data governance, quality, and lineage tracking approaches
- Design for both batch and real-time processing requirements

## Phase 3: Implementation Approach and Development Standards
- Define development methodology and project structure
- Specify coding standards, frameworks, and development tools
- Create database design with schemas, tables, and relationships
- Document ETL/ELT processes and data pipeline specifications
- Plan testing strategy including unit, integration, and user acceptance testing
- Establish monitoring, logging, and alerting requirements

## Phase 4: Deployment and Operations Planning
- Create deployment architecture for development, test, and production environments
- Document configuration management and environment promotion processes
- Specify backup, recovery, and business continuity procedures
- Plan capacity management and performance monitoring approach
- Create operational runbooks and troubleshooting guides
- Document maintenance procedures and support requirements

Ensure technical feasibility while meeting business objectives
```

#### Create `.github/prompts/data-architecture-design.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "create_file"]
description: "Data architecture design and modeling workflow for Azure solutions"
---

# Data Architecture Design Episode Template

## Phase 1: Data Source Analysis and Inventory
- Catalog all data sources including databases, files, APIs, and external systems
- Assess data quality, volume, velocity, and variety characteristics
- Document data ownership, governance, and access requirements
- Identify data privacy and regulatory compliance constraints
- Analyze current data integration patterns and pain points
- Evaluate source system capabilities and limitations

## Phase 2: Target Architecture Design
- Design Azure data platform architecture using appropriate services
- Implement medallion architecture (Bronze, Silver, Gold) for data lake organization
- Plan data warehousing strategy using Azure Synapse Analytics
- Design semantic layer for business intelligence and analytics
- Specify real-time vs. batch processing requirements
- Plan for data archiving and retention policies

## Phase 3: Data Modeling and Schema Design
- Create conceptual data model aligned with business requirements
- Design logical data model with proper normalization and relationships
- Develop physical data model optimized for Azure SQL and Synapse
- Implement dimensional modeling for data warehouse and analytics
- Design master data management and reference data strategies
- Plan for slowly changing dimensions and historical data tracking

## Phase 4: Integration and Pipeline Design
- Design data integration patterns and ETL/ELT processes
- Plan Azure Data Factory pipelines for data movement and transformation
- Implement change data capture (CDC) for incremental loading
- Design data quality validation and exception handling processes
- Plan data lineage tracking and impact analysis capabilities
- Create monitoring and alerting for data pipeline health

Focus on scalable, secure, and cost-effective Azure data solutions
```

#### Create `.github/prompts/bi-solution-design.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "semantic_search", "create_file"]
description: "Business Intelligence solution design and implementation workflow"
---

# BI Solution Design Episode Template

## Phase 1: Analytics Requirements Analysis
- Identify key business questions and analytical use cases
- Document reporting requirements with frequency and distribution needs
- Define KPIs and metrics with calculation logic and business rules
- Assess user personas and their analytical skill levels
- Plan for self-service analytics capabilities and governance
- Identify real-time vs. historical reporting requirements

## Phase 2: Data Model and Semantic Layer Design
- Design star schema and dimensional model for analytical workloads
- Create semantic layer using Azure Analysis Services or Power BI datasets
- Implement proper relationships, hierarchies, and time intelligence
- Design calculated measures and KPIs using DAX expressions
- Plan for data security through row-level security (RLS)
- Optimize model for performance and concurrent user access

## Phase 3: Dashboard and Report Development
- Design intuitive dashboards following UX best practices
- Create standardized report templates and layouts
- Implement interactive features and drill-through capabilities
- Design for mobile and responsive viewing experiences
- Create executive summary views and detailed analytical reports
- Implement consistent branding and visual design standards

## Phase 4: Deployment and Adoption Strategy
- Plan Power BI workspace structure and security model
- Design deployment pipeline for development, test, and production
- Create user training materials and documentation
- Implement feedback collection and continuous improvement process
- Plan for scale-out and premium capacity requirements
- Establish center of excellence (CoE) for ongoing BI governance

Focus on user adoption and business value realization
```

#### Create `.github/prompts/pipeline-implementation.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "run_in_terminal", "create_file"]
description: "Data pipeline implementation and automation workflow"
---

# Pipeline Implementation Episode Template

## Phase 1: Pipeline Architecture and Design
- Design end-to-end data pipeline architecture from source to consumption
- Plan for both batch and real-time processing requirements
- Implement proper error handling, retry logic, and dead letter queues
- Design for idempotent operations and exactly-once processing
- Plan monitoring and alerting for pipeline health and performance
- Consider cost optimization through efficient resource utilization

## Phase 2: Azure Data Factory Development
- Create parameterized and reusable pipeline templates
- Implement proper trigger strategies (scheduled, event-based, tumbling window)
- Use mapping data flows for visual data transformation
- Implement integration runtime optimization for performance
- Set up proper logging and monitoring through Azure Monitor
- Configure Git integration for version control and CI/CD

## Phase 3: Data Transformation and Quality Implementation
- Implement data validation and quality checks at each pipeline stage
- Create data transformation logic using Python, SQL, or mapping data flows
- Apply business rules and data standardization processes
- Implement exception handling and data quality reporting
- Create data reconciliation processes between source and target
- Set up automated testing for pipeline validation

## Phase 4: Deployment and Operations Setup
- Create deployment pipeline using Azure DevOps or GitHub Actions
- Implement environment-specific configuration management
- Set up monitoring dashboards and alerting rules
- Create operational runbooks and troubleshooting guides
- Plan for capacity management and scaling requirements
- Establish data lineage documentation and impact analysis

Focus on reliability, scalability, and operational excellence
```

#### Create `.github/prompts/stakeholder-review.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "insert_edit_into_file"]
description: "Stakeholder presentation and feedback incorporation workflow"
---

# Stakeholder Review Episode Template

## Phase 1: Review Preparation and Presentation Planning
- Prepare executive summary highlighting key business benefits and ROI
- Create visual presentations tailored to different stakeholder audiences
- Develop demonstration scenarios showcasing solution capabilities
- Prepare supporting documentation and detailed specifications
- Plan presentation agenda with clear objectives and decision points
- Identify potential objections and prepare response strategies

## Phase 2: Stakeholder Presentation and Demonstration
- Present business case with quantified benefits and success metrics
- Demonstrate solution prototypes and proof of concepts
- Walk through technical architecture and implementation approach
- Address stakeholder questions and concerns professionally
- Facilitate discussion on priorities, timelines, and resource requirements
- Document feedback, decisions, and action items during sessions

## Phase 3: Feedback Analysis and Incorporation
- Analyze stakeholder feedback for patterns and priority themes
- Assess impact of requested changes on timeline, budget, and scope
- Prioritize feedback based on business value and implementation complexity
- Update requirements and specifications based on approved changes
- Communicate change impacts to all affected stakeholders
- Maintain traceability between feedback and requirement updates

## Phase 4: Approval and Sign-off Management
- Prepare formal approval documents with clear scope and acceptance criteria
- Facilitate stakeholder sign-off process with appropriate authorization levels
- Document approved requirements and establish change control process
- Communicate final requirements to implementation teams
- Plan for ongoing stakeholder engagement during implementation
- Establish success criteria and post-implementation review process

Focus on stakeholder alignment and formal approval for implementation
```

#### Create `.github/prompts/implementation-planning.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "semantic_search", "create_file"]
description: "Project planning and delivery strategy development workflow"
---

# Implementation Planning Episode Template

## Phase 1: Project Scope and Approach Definition
- Define project scope with clear deliverables and acceptance criteria
- Select appropriate implementation methodology (Agile, Waterfall, Hybrid)
- Create work breakdown structure (WBS) with detailed task estimates
- Identify project dependencies and critical path activities
- Plan for phased delivery approach with incremental value realization
- Assess make vs. buy vs. configure decisions for each component

## Phase 2: Resource Planning and Team Structure
- Identify required skills and expertise for successful delivery
- Plan team structure with roles, responsibilities, and reporting relationships
- Assess internal resource availability and external vendor requirements
- Create resource allocation plan with timeline and budget considerations
- Plan for knowledge transfer and training requirements
- Establish communication protocols and meeting cadence

## Phase 3: Risk Management and Mitigation Planning
- Identify project risks with probability and impact assessment
- Develop risk mitigation strategies and contingency plans
- Create risk monitoring and escalation procedures
- Plan for technology risks including integration and performance challenges
- Assess organizational change risks and resistance factors
- Establish risk communication and reporting protocols

## Phase 4: Timeline and Milestone Planning
- Create detailed project timeline with phases and key milestones
- Plan for testing phases including unit, integration, and user acceptance testing
- Schedule stakeholder reviews and approval checkpoints
- Plan for training and change management activities
- Create go-live plan with rollback procedures
- Establish post-implementation support and optimization phases

Focus on realistic planning with appropriate risk mitigation
```

#### Create `.github/prompts/testing-strategy.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "create_file"]
description: "Quality assurance and testing strategy development workflow"
---

# Testing Strategy Episode Template

## Phase 1: Testing Approach and Framework Design
- Define testing strategy aligned with project methodology and timeline
- Create test plan with scope, objectives, and success criteria
- Identify testing types required (unit, integration, system, UAT, performance)
- Plan test environment requirements and data management strategies
- Establish defect management and resolution processes
- Define testing tools and automation framework requirements

## Phase 2: Test Case Development and Data Preparation
- Create comprehensive test cases covering functional and non-functional requirements
- Develop test scenarios for positive, negative, and edge cases
- Prepare test data sets representing various business scenarios
- Create automated test scripts for regression and performance testing
- Design data validation and reconciliation test procedures
- Plan for security and compliance testing requirements

## Phase 3: User Acceptance Testing (UAT) Planning
- Identify UAT participants representing key business user groups
- Create UAT scenarios based on real business use cases
- Prepare UAT environment with production-like data and configurations
- Develop UAT execution plan with timelines and sign-off criteria
- Plan user training and support during UAT phase
- Establish UAT feedback collection and defect resolution process

## Phase 4: Performance and Load Testing Strategy
- Define performance requirements and acceptance criteria
- Create load testing scenarios representing expected usage patterns
- Plan for stress testing and scalability validation
- Design monitoring and measurement approach for performance metrics
- Establish performance baseline and improvement targets
- Plan for performance optimization and tuning activities

Focus on comprehensive quality assurance and user acceptance
```

### Step 6: Meta-Cognitive Files (Reuse from Previous Setups)

The learning.instructions.md, meta-cognition.instructions.md, consolidation.prompt.md, self-assessment.prompt.md, meta-learning.prompt.md, and cognitive-health.prompt.md files from previous setups are applicable to BRD development as well, focusing on cognitive processes rather than domain-specific content.

## 📊 BRD Setup Validation

After creating all files, verify BRD setup:

1. **Check BRD file structure**: Ensure all directories and BRD-specific files exist
2. **Validate VS Code settings**: Confirm BRD instruction files are recognized
3. **Test BRD activation**: Try BRD "@" commands in Copilot chat
4. **Verify Azure coverage**: Check that Azure data platform instructions are properly implemented

## 🚀 BRD Quick Start Commands

After setup, test with these BRD-specific commands:

**BRD Functionality Tests**:
- `@workspace Help me create a business requirements document for a data warehouse project` (Should activate brd-creation.prompt.md)
- `Design an Azure data architecture for business intelligence` (Should activate data-architecture-design.prompt.md)
- `Create technical specifications for ETL pipelines` (Should activate pipeline-implementation.prompt.md)

**Implementation Workflow Tests**:
- `Help me gather requirements from stakeholders` (Should activate requirements-gathering.prompt.md)
- `Plan a BI solution using Power BI and Azure Synapse` (Should activate bi-solution-design.prompt.md)
- `Create a testing strategy for data migration` (Should activate testing-strategy.prompt.md)

**Meta-BRD Tests**:
- `@workspace Assess your BRD and technical documentation quality` (Should activate self-assessment.prompt.md)
- `How can you improve requirements analysis assistance?` (Should activate meta-learning.prompt.md)
- `Monitor your BRD cognitive architecture health` (Should activate cognitive-health.prompt.md)

## ⚡ BRD Success Indicators

Your BRD cognitive architecture is working when:
- GitHub Copilot provides comprehensive business requirements templates
- Azure architecture recommendations follow cloud-native best practices
- Data modeling suggestions optimize for analytics and performance
- Pipeline design incorporates proper monitoring and error handling
- Stakeholder communication focuses on business value and ROI
- **Meta-cognitive capabilities**: The AI can assess BRD quality and suggest improvements
- **Requirements evolution**: The system learns to recognize patterns in business needs
- **BRD health monitoring**: The system maintains awareness of stakeholder alignment and technical feasibility

## 🔄 BRD Maintenance

- Run consolidation when adding new Azure services or architectural patterns
- Update best practices as Azure platform capabilities evolve
- Monitor BRD memory index for coverage across business domains
- Archive outdated technical approaches and methodologies
- **Execute BRD self-assessment after major project completions**
- **Run requirements strategy analysis quarterly for process optimization**
- **Perform BRD architecture health checks before starting new initiatives**

---

**BRD SETUP COMPLETE**: Your adaptive AI business analyst partner is now ready to provide comprehensive BRD and technical documentation assistance that improves over time through systematic memory consolidation and meta-cognitive self-monitoring for Azure data platform implementations.
