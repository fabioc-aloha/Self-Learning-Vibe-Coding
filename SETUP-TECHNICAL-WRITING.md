# Technical Writing Cognitive Architecture Setup Guide

**INSTRUCTIONS FOR GITHUB COPILOT**: This file contains complete setup instructions for implementing the Self-Learning Vibe Coding cognitive memory architecture optimized for technical writing, including documentation strategy, API documentation, user guides, knowledge management, and comprehensive content creation workflows.

## 📝 Technical Writing Automated Setup Protocol

**Execute these steps in order to establish a complete cognitive architecture system for technical writing:**

### Step 1: VS Code Configuration (Required)

Add these settings to VS Code `settings.json`:

```json
{
  "github.copilot.chat.codeGeneration.useInstructionFiles": true,
  "chat.promptFiles": true,
  "chat.instructionsFilesLocations": [".github/instructions"],
  "files.associations": {
    "*.docs": "markdown",
    "*.guide": "markdown",
    "*.manual": "markdown",
    "*.spec": "markdown",
    "*.reference": "markdown",
    "*.tutorial": "markdown",
    "*.changelog": "markdown",
    "*.glossary": "markdown",
    "*.template": "markdown",
    "*.style": "markdown"
  },
  "search.exclude": {
    "**/drafts/**": false,
    "**/reviews/**": false,
    "**/archived/**": true
  },
  "files.watcherExclude": {
    "**/archived/**": true,
    "**/legacy-docs/**": true
  },
  "editor.rulers": [80, 120],
  "editor.wordWrap": "wordWrapColumn",
  "editor.wordWrapColumn": 80,
  "markdown.extension.toc.levels": "2..6",
  "markdown.extension.completion.enabled": true,
  "markdown.extension.list.indentationSize": "adaptive",
  "markdown.extension.orderedList.marker": "ordered",
  "markdown.extension.orderedList.autoRenumber": true,
  "markdown.extension.tableFormatter.enabled": true,
  "markdown.extension.print.absoluteImgPath": false,
  "markdown.extension.syntax.decorations": true,
  "markdown.extension.math.enabled": true,
  "grammarly.files.include": ["**/*.md", "**/*.txt", "**/*.docs"],
  "grammarly.overrides": [
    {
      "files": ["**/*.md"],
      "config": {
        "audience": "knowledgeable",
        "domain": "technical",
        "emotions": [],
        "goals": ["inform", "describe"]
      }
    }
  ]
}
```

**Access settings.json**: `Ctrl+Shift+P` → "Preferences: Open User Settings (JSON)"

### Step 2: Create Technical Writing Directory Structure

Create this exact folder structure in the project root:

```
project-root/
├── .github/
│   ├── copilot-instructions.md          # Global Technical Writing Memory
│   ├── instructions/                    # Technical Writing Procedural Memory
│   │   ├── technical-writing.instructions.md
│   │   ├── documentation-strategy.instructions.md
│   │   ├── api-documentation.instructions.md
│   │   ├── user-guides.instructions.md
│   │   ├── content-architecture.instructions.md
│   │   ├── style-guide.instructions.md
│   │   ├── information-design.instructions.md
│   │   ├── content-review.instructions.md
│   │   ├── version-control.instructions.md
│   │   ├── collaboration.instructions.md
│   │   ├── accessibility.instructions.md
│   │   ├── localization.instructions.md
│   │   ├── content-management.instructions.md
│   │   ├── analytics.instructions.md
│   │   ├── tools-integration.instructions.md
│   │   ├── maintenance.instructions.md
│   │   ├── learning.instructions.md     # Meta-Cognitive Learning
│   │   └── meta-cognition.instructions.md  # Self-Monitoring
│   └── prompts/                         # Technical Writing Episodic Memory
│       ├── documentation-planning.prompt.md
│       ├── content-creation.prompt.md
│       ├── api-reference.prompt.md
│       ├── tutorial-development.prompt.md
│       ├── user-story-documentation.prompt.md
│       ├── technical-specification.prompt.md
│       ├── content-audit.prompt.md
│       ├── style-consistency.prompt.md
│       ├── information-architecture.prompt.md
│       ├── content-migration.prompt.md
│       ├── review-process.prompt.md
│       ├── content-optimization.prompt.md
│       ├── knowledge-transfer.prompt.md
│       ├── publication-workflow.prompt.md
│       ├── consolidation.prompt.md
│       ├── self-assessment.prompt.md    # Meta-Cognitive Assessment
│       ├── meta-learning.prompt.md      # Learning Strategy Evolution
│       └── cognitive-health.prompt.md   # Architecture Maintenance
├── docs/
│   ├── user-guides/                     # User documentation
│   │   ├── getting-started/
│   │   │   ├── installation/
│   │   │   ├── quickstart/
│   │   │   ├── first-steps/
│   │   │   └── troubleshooting/
│   │   ├── tutorials/
│   │   │   ├── beginner/
│   │   │   ├── intermediate/
│   │   │   ├── advanced/
│   │   │   └── use-cases/
│   │   ├── how-to-guides/
│   │   │   ├── common-tasks/
│   │   │   ├── workflows/
│   │   │   ├── integrations/
│   │   │   └── customization/
│   │   └── faq/
│   │       ├── general/
│   │       ├── technical/
│   │       ├── billing/
│   │       └── support/
│   ├── api-reference/                   # API documentation
│   │   ├── overview/
│   │   ├── authentication/
│   │   ├── endpoints/
│   │   │   ├── rest-api/
│   │   │   ├── graphql/
│   │   │   ├── webhooks/
│   │   │   └── websockets/
│   │   ├── sdks/
│   │   │   ├── javascript/
│   │   │   ├── python/
│   │   │   ├── java/
│   │   │   ├── csharp/
│   │   │   └── mobile/
│   │   ├── examples/
│   │   │   ├── code-samples/
│   │   │   ├── use-cases/
│   │   │   ├── integrations/
│   │   │   └── testing/
│   │   └── reference/
│   │       ├── schemas/
│   │       ├── error-codes/
│   │       ├── rate-limits/
│   │       └── versioning/
│   ├── developer-guides/                # Developer documentation
│   │   ├── architecture/
│   │   │   ├── system-design/
│   │   │   ├── data-flow/
│   │   │   ├── security/
│   │   │   └── performance/
│   │   ├── setup/
│   │   │   ├── environment/
│   │   │   ├── dependencies/
│   │   │   ├── configuration/
│   │   │   └── deployment/
│   │   ├── contributing/
│   │   │   ├── guidelines/
│   │   │   ├── code-style/
│   │   │   ├── testing/
│   │   │   └── documentation/
│   │   └── advanced/
│   │       ├── customization/
│   │       ├── extensions/
│   │       ├── plugins/
│   │       └── integrations/
│   ├── technical-specs/                 # Technical specifications
│   │   ├── requirements/
│   │   │   ├── functional/
│   │   │   ├── non-functional/
│   │   │   ├── user-stories/
│   │   │   └── acceptance-criteria/
│   │   ├── design/
│   │   │   ├── system-design/
│   │   │   ├── database-design/
│   │   │   ├── api-design/
│   │   │   └── ui-design/
│   │   ├── protocols/
│   │   │   ├── communication/
│   │   │   ├── data-formats/
│   │   │   ├── security/
│   │   │   └── standards/
│   │   └── decisions/
│   │       ├── architecture/
│   │       ├── technology/
│   │       ├── process/
│   │       └── rationale/
│   └── release-notes/                   # Release documentation
│       ├── versions/
│       │   ├── major-releases/
│       │   ├── minor-releases/
│       │   ├── patches/
│       │   └── previews/
│       ├── changelogs/
│       │   ├── features/
│       │   ├── improvements/
│       │   ├── bug-fixes/
│       │   └── breaking-changes/
│       ├── migration-guides/
│       │   ├── version-upgrades/
│       │   ├── breaking-changes/
│       │   ├── deprecated-features/
│       │   └── compatibility/
│       └── announcements/
│           ├── new-features/
│           ├── deprecations/
│           ├── security-updates/
│           └── maintenance/
├── content/
│   ├── drafts/                          # Content in development
│   │   ├── articles/
│   │   ├── guides/
│   │   ├── tutorials/
│   │   └── specifications/
│   ├── reviews/                         # Content under review
│   │   ├── pending/
│   │   ├── in-progress/
│   │   ├── approved/
│   │   └── rejected/
│   ├── published/                       # Published content
│   │   ├── current/
│   │   ├── archived/
│   │   └── deprecated/
│   ├── templates/                       # Content templates
│   │   ├── documentation/
│   │   ├── tutorials/
│   │   ├── api-docs/
│   │   ├── user-guides/
│   │   └── specifications/
│   └── assets/                          # Content assets
│       ├── images/
│       │   ├── screenshots/
│       │   ├── diagrams/
│       │   ├── icons/
│       │   └── illustrations/
│       ├── videos/
│       │   ├── tutorials/
│       │   ├── demos/
│       │   ├── webinars/
│       │   └── presentations/
│       ├── downloads/
│       │   ├── samples/
│       │   ├── tools/
│       │   ├── templates/
│       │   └── resources/
│       └── interactive/
│           ├── demos/
│           ├── examples/
│           ├── simulations/
│           └── calculators/
├── style-guide/
│   ├── writing/                         # Writing guidelines
│   │   ├── tone-voice/
│   │   ├── grammar-style/
│   │   ├── terminology/
│   │   ├── formatting/
│   │   └── examples/
│   ├── visual/                          # Visual guidelines
│   │   ├── branding/
│   │   ├── typography/
│   │   ├── colors/
│   │   ├── imagery/
│   │   └── layouts/
│   ├── technical/                       # Technical guidelines
│   │   ├── code-examples/
│   │   ├── api-documentation/
│   │   ├── diagrams/
│   │   ├── screenshots/
│   │   └── version-control/
│   └── accessibility/                   # Accessibility guidelines
│       ├── content/
│       ├── images/
│       ├── navigation/
│       ├── multimedia/
│       └── testing/
├── workflows/
│   ├── content-creation/                # Content creation workflows
│   │   ├── planning/
│   │   ├── research/
│   │   ├── writing/
│   │   ├── editing/
│   │   └── publishing/
│   ├── review-process/                  # Review workflows
│   │   ├── technical-review/
│   │   ├── editorial-review/
│   │   ├── legal-review/
│   │   ├── accessibility-review/
│   │   └── final-approval/
│   ├── maintenance/                     # Maintenance workflows
│   │   ├── content-audit/
│   │   ├── updates/
│   │   ├── archiving/
│   │   ├── migration/
│   │   └── cleanup/
│   └── collaboration/                   # Collaboration workflows
│       ├── team-coordination/
│       ├── stakeholder-engagement/
│       ├── feedback-collection/
│       ├── knowledge-sharing/
│       └── training/
├── tools/
│   ├── authoring/                       # Authoring tools
│   │   ├── markdown-editors/
│   │   ├── documentation-generators/
│   │   ├── content-management/
│   │   ├── collaboration-platforms/
│   │   └── version-control/
│   ├── quality-assurance/               # QA tools
│   │   ├── grammar-checkers/
│   │   ├── style-validators/
│   │   ├── link-checkers/
│   │   ├── accessibility-validators/
│   │   └── content-auditors/
│   ├── automation/                      # Automation tools
│   │   ├── content-generation/
│   │   ├── publication-pipelines/
│   │   ├── update-notifications/
│   │   ├── backup-systems/
│   │   └── monitoring/
│   ├── analytics/                       # Analytics tools
│   │   ├── content-performance/
│   │   ├── user-behavior/
│   │   ├── search-analytics/
│   │   ├── feedback-analysis/
│   │   └── roi-measurement/
│   └── integration/                     # Integration tools
│       ├── cms-connectors/
│       ├── api-integrations/
│       ├── development-tools/
│       ├── design-tools/
│       └── project-management/
├── analytics/
│   ├── content-metrics/                 # Content performance
│   │   ├── readability-scores/
│   │   ├── engagement-metrics/
│   │   ├── completion-rates/
│   │   ├── user-satisfaction/
│   │   └── effectiveness-measures/
│   ├── user-behavior/                   # User analytics
│   │   ├── navigation-patterns/
│   │   ├── search-queries/
│   │   ├── help-requests/
│   │   ├── feedback-analysis/
│   │   └── conversion-tracking/
│   ├── content-health/                  # Content quality
│   │   ├── accuracy-checks/
│   │   ├── currency-monitoring/
│   │   ├── completeness-assessment/
│   │   ├── consistency-validation/
│   │   └── accessibility-compliance/
│   └── business-impact/                 # Business metrics
│       ├── support-reduction/
│       ├── user-adoption/
│       ├── time-to-value/
│       ├── cost-savings/
│       └── revenue-impact/
└── governance/
    ├── policies/                        # Content policies
    │   ├── editorial-standards/
    │   ├── publication-guidelines/
    │   ├── review-requirements/
    │   ├── retention-policies/
    │   └── compliance-standards/
    ├── roles-responsibilities/          # Team structure
    │   ├── content-owners/
    │   ├── subject-matter-experts/
    │   ├── editors/
    │   ├── reviewers/
    │   └── approvers/
    ├── processes/                       # Standard processes
    │   ├── content-lifecycle/
    │   ├── quality-assurance/
    │   ├── change-management/
    │   ├── escalation-procedures/
    │   └── training-programs/
    └── compliance/                      # Compliance management
        ├── legal-requirements/
        ├── industry-standards/
        ├── accessibility-compliance/
        ├── data-protection/
        └── audit-trails/
```

### Step 3: Global Technical Writing Declarative Memory Setup

**Create `.github/copilot-instructions.md`** with this exact content:

```markdown
# Self-Learning Vibe Coding - Technical Writing Cognitive Architecture

IMPORTANT: This file serves as Global Technical Writing Declarative Memory. Optimized for documentation strategy, API documentation, user guides, knowledge management, and comprehensive content creation workflows.

## 🧠 Technical Writing Cognitive Architecture Status

**Working Memory**: 4/4 rules (at optimal capacity for technical writing)
**Consolidation**: Auto-trigger when exceeding capacity
**Memory Distribution**: Active across technical writing procedural (.instructions.md) and content creation episodic (.prompt.md) systems

## 📝 Technical Writing Working Memory - Quick Reference (Limit: 4 Critical Rules)

| Priority | Rule | Load | Auto-Consolidate |
|----------|------|------|------------------|
| P1 | `@user-first` - Design all content prioritizing user needs, context, and task completion | Low | Never |
| P2 | `@clarity-precision` - Use clear, concise language with precise technical accuracy | Medium | >30 days unused |
| P3 | `@meditation` - Auto-consolidate when working memory capacity exceeded | High | When triggered |
| P4 | `@iterative-improvement` - Continuously improve content based on user feedback and analytics | Medium | When obsolete |

## 🎯 Technical Writing Cognitive Architecture Coordination

### Technical Writing Procedural Memory Activation (Context-Dependent):
- `technical-writing.instructions.md` → General tech writing for .docs, .guide, .manual, .spec files
- `documentation-strategy.instructions.md` → Doc strategy for *strategy*, *planning*, *architecture* files
- `api-documentation.instructions.md` → API docs for *api*, *endpoint*, *sdk*, *reference* files
- `user-guides.instructions.md` → User guides for *user*, *guide*, *tutorial*, *how-to* files
- `content-architecture.instructions.md` → Content architecture for *information*, *structure*, *taxonomy* files
- `style-guide.instructions.md` → Style guide for *style*, *tone*, *voice*, *grammar* files
- `information-design.instructions.md` → Info design for *design*, *layout*, *visual*, *ux* files
- `content-review.instructions.md` → Content review for *review*, *edit*, *feedback*, *quality* files
- `version-control.instructions.md` → Version control for *version*, *git*, *branch*, *merge* files
- `collaboration.instructions.md` → Collaboration for *team*, *workflow*, *process*, *stakeholder* files
- `accessibility.instructions.md` → Accessibility for *accessibility*, *a11y*, *inclusive*, *wcag* files
- `localization.instructions.md` → Localization for *localization*, *i18n*, *translation*, *cultural* files
- `content-management.instructions.md` → Content management for *cms*, *publishing*, *workflow*, *lifecycle* files
- `analytics.instructions.md` → Analytics for *analytics*, *metrics*, *performance*, *tracking* files
- `tools-integration.instructions.md` → Tools for *tools*, *automation*, *integration*, *pipeline* files
- `maintenance.instructions.md` → Maintenance for *maintenance*, *update*, *audit*, *archive* files
- `learning.instructions.md` → Meta-cognitive learning for *instructions*, *learning* files
- `meta-cognition.instructions.md` → Self-awareness for *meta*, *monitor*, *assess* files

### Technical Writing Episodic Memory Activation (Content Creation Workflows):
- `documentation-planning.prompt.md` → Documentation planning and strategy development
- `content-creation.prompt.md` → Content creation and writing workflows
- `api-reference.prompt.md` → API reference documentation creation
- `tutorial-development.prompt.md` → Tutorial and how-to guide development
- `user-story-documentation.prompt.md` → User story and requirement documentation
- `technical-specification.prompt.md` → Technical specification writing
- `content-audit.prompt.md` → Content audit and quality assessment
- `style-consistency.prompt.md` → Style and consistency review processes
- `information-architecture.prompt.md` → Information architecture design
- `content-migration.prompt.md` → Content migration and restructuring
- `review-process.prompt.md` → Content review and approval workflows
- `content-optimization.prompt.md` → Content optimization and improvement
- `knowledge-transfer.prompt.md` → Knowledge transfer and documentation
- `publication-workflow.prompt.md` → Publication and distribution workflows
- `consolidation.prompt.md` → Technical writing memory optimization
- `self-assessment.prompt.md` → Technical writing performance evaluation
- `meta-learning.prompt.md` → Technical writing strategy evolution
- `cognitive-health.prompt.md` → Technical writing architecture maintenance

### Technical Writing Auto-Consolidation Triggers

- Working memory > 4 rules → Execute consolidation.prompt.md
- User feedback conflicts detected → Activate user-first design protocols
- Content quality issues detected → Review and redistribute content creation memory load
- User requests meditation → Full technical writing cognitive architecture optimization
- **Technical writing performance assessment needed → Execute self-assessment.prompt.md**
- **Technical writing strategy evolution required → Execute meta-learning.prompt.md**
- **Technical writing architecture health check → Execute cognitive-health.prompt.md**

## 🔄 Technical Writing Memory Transfer Protocol

**Immediate Transfer**: Critical user experience issues → Quick Reference (P1-P4)
**Gradual Consolidation**: Repeated writing patterns → Technical writing procedural memory (.instructions.md)
**Complex Content Workflows**: Multi-stakeholder projects → Content creation episodic memory (.prompt.md)
**Archive Management**: Obsolete technical writing patterns → Historical storage in specialized files
**Index Maintenance**: Auto-update Technical Writing Long-Term Memory Index during transfers

## 📚 Technical Writing Long-Term Memory Index

### Technical Writing Procedural Memory Store (.github/instructions/)
| File | Domain | Activation Pattern | Last Updated |
|------|--------|-------------------|--------------|
| technical-writing.instructions.md | General Technical Writing | *.docs, *.guide, *.manual, *.spec | Auto-tracked |
| documentation-strategy.instructions.md | Documentation Strategy | *strategy*, *planning*, *architecture* | Auto-tracked |
| api-documentation.instructions.md | API Documentation | *api*, *endpoint*, *sdk*, *reference* | Auto-tracked |
| user-guides.instructions.md | User Guides | *user*, *guide*, *tutorial*, *how-to* | Auto-tracked |
| content-architecture.instructions.md | Content Architecture | *information*, *structure*, *taxonomy* | Auto-tracked |
| style-guide.instructions.md | Style Guide | *style*, *tone*, *voice*, *grammar* | Auto-tracked |
| information-design.instructions.md | Information Design | *design*, *layout*, *visual*, *ux* | Auto-tracked |
| content-review.instructions.md | Content Review | *review*, *edit*, *feedback*, *quality* | Auto-tracked |
| version-control.instructions.md | Version Control | *version*, *git*, *branch*, *merge* | Auto-tracked |
| collaboration.instructions.md | Collaboration | *team*, *workflow*, *process*, *stakeholder* | Auto-tracked |
| accessibility.instructions.md | Accessibility | *accessibility*, *a11y*, *inclusive*, *wcag* | Auto-tracked |
| localization.instructions.md | Localization | *localization*, *i18n*, *translation*, *cultural* | Auto-tracked |
| content-management.instructions.md | Content Management | *cms*, *publishing*, *workflow*, *lifecycle* | Auto-tracked |
| analytics.instructions.md | Analytics | *analytics*, *metrics*, *performance*, *tracking* | Auto-tracked |
| tools-integration.instructions.md | Tools Integration | *tools*, *automation*, *integration*, *pipeline* | Auto-tracked |
| maintenance.instructions.md | Maintenance | *maintenance*, *update*, *audit*, *archive* | Auto-tracked |
| learning.instructions.md | Meta-Learning | *instructions*, *learning* | Auto-tracked |
| meta-cognition.instructions.md | Self-Monitoring | *meta*, *monitor*, *assess* | Auto-tracked |

### Technical Writing Episodic Memory Store (.github/prompts/)
| File | Technical Writing Workflow | Complexity Level | Usage Frequency |
|------|----------------------------|------------------|-----------------|
| documentation-planning.prompt.md | Documentation Planning | High | Auto-tracked |
| content-creation.prompt.md | Content Creation | Medium | Auto-tracked |
| api-reference.prompt.md | API Reference Creation | High | Auto-tracked |
| tutorial-development.prompt.md | Tutorial Development | Medium | Auto-tracked |
| user-story-documentation.prompt.md | User Story Documentation | Medium | Auto-tracked |
| technical-specification.prompt.md | Technical Specification | High | Auto-tracked |
| content-audit.prompt.md | Content Audit | Medium | Auto-tracked |
| style-consistency.prompt.md | Style Consistency | Medium | Auto-tracked |
| information-architecture.prompt.md | Information Architecture | High | Auto-tracked |
| content-migration.prompt.md | Content Migration | High | Auto-tracked |
| review-process.prompt.md | Review Process | Medium | Auto-tracked |
| content-optimization.prompt.md | Content Optimization | Medium | Auto-tracked |
| knowledge-transfer.prompt.md | Knowledge Transfer | Medium | Auto-tracked |
| publication-workflow.prompt.md | Publication Workflow | Medium | Auto-tracked |
| consolidation.prompt.md | Memory Optimization | High | Auto-tracked |
| self-assessment.prompt.md | Performance Evaluation | High | Auto-tracked |
| meta-learning.prompt.md | Strategy Evolution | High | Auto-tracked |
| cognitive-health.prompt.md | Health Monitoring | Medium | Auto-tracked |

### Technical Writing Memory Transfer Protocol Status
- **Active Files**: 36 specialized technical writing memory files (18 procedural + 18 episodic)
- **Last Consolidation**: Technical writing architecture initialization with meta-cognitive enhancements
- **Cognitive Load Status**: Optimized for user-centered content creation and systematic documentation
- **Index Synchronization**: Maintained automatically during consolidation
- **Meta-Cognitive Status**: Fully operational with technical writing performance assessment and strategy evolution

---

*Global Technical Writing Declarative Memory Component - Coordinates distributed technical writing cognitive architecture while maintaining optimal content creation efficiency. Detailed technical writing protocols reside in specialized memory files.*
```

### Step 4: Technical Writing Procedural Memory Files

#### Create `.github/instructions/technical-writing.instructions.md`:

```markdown
---
applyTo: "**/*.docs,**/*.guide,**/*.manual,**/*.spec,**/docs/**,**/documentation/**"
description: "General technical writing standards and user-centered content creation best practices"
---

# Technical Writing Procedural Memory

## User-Centered Writing Principles
- Prioritize user needs, goals, and context in all content decisions
- Design content structure around user tasks and mental models
- Use plain language principles while maintaining technical accuracy
- Provide clear, actionable information that enables task completion
- Test content usability with representative users throughout development

## Information Architecture and Organization
- Structure content hierarchically with logical topic progression
- Use consistent navigation patterns and information organization
- Implement progressive disclosure for complex technical information
- Create clear content relationships through cross-references and linking
- Design content for multiple access patterns (sequential reading, reference lookup, search)

## Writing Style and Clarity Standards
- Use active voice and clear, direct language
- Write concise sentences and paragraphs focused on single concepts
- Define technical terms consistently and provide glossaries when needed
- Use parallel structure in lists, headings, and procedural steps
- Maintain consistent tone and voice throughout all content types

## Content Quality and Accuracy
- Verify technical accuracy through subject matter expert review
- Test all procedures, code examples, and instructions before publication
- Maintain version control and change tracking for all content
- Implement regular content audits and accuracy reviews
- Document content sources and maintain attribution standards

## Accessibility and Inclusive Design
- Follow WCAG guidelines for content accessibility
- Use descriptive headings, alt text, and semantic markup
- Design content for diverse reading levels and cognitive abilities
- Consider cultural context and inclusive language in all content
- Test content accessibility with assistive technologies and diverse users
```

#### Create `.github/instructions/documentation-strategy.instructions.md`:

```markdown
---
applyTo: "**/*strategy*,**/*planning*,**/*architecture*,**/docs/strategy/**"
description: "Documentation strategy development and content planning best practices"
---

# Documentation Strategy Procedural Memory

## Strategic Content Planning
- Align documentation strategy with business objectives and user needs
- Conduct comprehensive content audits to identify gaps and opportunities
- Develop content roadmaps that support product development cycles
- Establish content governance frameworks and ownership models
- Create measurement frameworks for documentation effectiveness and ROI

## Audience Analysis and Segmentation
- Identify distinct user personas and their information needs
- Map user journeys and content touchpoints throughout product lifecycle
- Analyze user behavior data to optimize content strategy decisions
- Segment content strategy by user expertise levels and use cases
- Design personalization strategies for different audience segments

## Content Architecture and Taxonomy
- Design scalable information architectures that support growth
- Develop consistent taxonomy and tagging systems for content organization
- Create content templates and standardized structures for efficiency
- Plan content relationships and cross-referencing strategies
- Design search and navigation systems that support user mental models

## Cross-Functional Collaboration
- Establish workflows for subject matter expert collaboration
- Create review and approval processes that ensure quality without bottlenecks
- Design stakeholder engagement strategies for content planning and feedback
- Coordinate documentation efforts with product, engineering, and design teams
- Implement change management processes for documentation updates

## Technology and Tool Strategy
- Evaluate and select documentation tools that support strategic objectives
- Plan integration strategies between documentation tools and development workflows
- Design automation strategies for content creation, maintenance, and publication
- Implement analytics and measurement tools for content performance tracking
- Plan scalability and maintenance requirements for documentation infrastructure
```

#### Create `.github/instructions/api-documentation.instructions.md`:

```markdown
---
applyTo: "**/*api*,**/*endpoint*,**/*sdk*,**/*reference*,**/api-reference/**"
description: "API documentation standards and developer-focused content creation"
---

# API Documentation Procedural Memory

## API Reference Documentation Standards
- Provide complete, accurate descriptions of all endpoints, parameters, and responses
- Include comprehensive example requests and responses with realistic data
- Document authentication requirements, rate limits, and error handling
- Maintain synchronization between API implementation and documentation
- Use consistent formatting and structure across all API reference content

## Developer Experience Optimization
- Design documentation that supports both learning and reference use cases
- Provide interactive examples and testing capabilities where possible
- Include code samples in multiple programming languages and frameworks
- Create clear getting-started guides that enable rapid API adoption
- Design error messages and troubleshooting guides that accelerate problem resolution

## Code Example Best Practices
- Use realistic, working code examples that demonstrate practical use cases
- Test all code examples for accuracy and completeness
- Provide examples at multiple complexity levels (basic, intermediate, advanced)
- Include error handling and edge case examples in code samples
- Maintain code examples across different SDK versions and programming languages

## SDK and Integration Documentation
- Document SDK installation, configuration, and basic usage patterns
- Provide comprehensive guides for common integration scenarios
- Include troubleshooting guides for common SDK and integration issues
- Document version compatibility and migration guides for SDK updates
- Create sample applications and tutorials that demonstrate real-world usage

## API Lifecycle Documentation
- Document API versioning strategies and backward compatibility policies
- Provide migration guides for API version updates and deprecations
- Maintain changelog documentation with clear impact assessment
- Document API roadmap and upcoming changes for developer planning
- Create deprecation timelines and communication strategies for API changes
```

#### Create `.github/instructions/user-guides.instructions.md`:

```markdown
---
applyTo: "**/*user*,**/*guide*,**/*tutorial*,**/*how-to*,**/user-guides/**"
description: "User guide development and task-oriented documentation standards"
---

# User Guides Procedural Memory

## Task-Oriented Content Design
- Structure content around user goals and specific tasks rather than system features
- Use action-oriented headings and clear step-by-step procedures
- Provide context for when and why users would perform specific tasks
- Include prerequisites, assumptions, and expected outcomes for all procedures
- Design content that supports both sequential reading and random access patterns

## Tutorial and Getting Started Guide Development
- Create progressive learning experiences that build user confidence and competence
- Start with simple, essential tasks and gradually introduce more complex concepts
- Provide multiple pathways for users with different experience levels and goals
- Include checkpoint assessments and validation steps throughout tutorials
- Design tutorials that align with real-world use cases and user workflows

## Procedural Documentation Standards
- Use imperative mood and active voice for all procedural steps
- Number sequential steps and use parallel structure for all instructions
- Include screenshots, diagrams, and visual aids that support written instructions
- Provide alternative approaches for different user preferences and contexts
- Test all procedures with representative users to validate usability

## Troubleshooting and Support Content
- Anticipate common user problems and provide proactive troubleshooting guidance
- Create systematic problem-solving frameworks that users can apply independently
- Include diagnostic questions and decision trees for complex troubleshooting scenarios
- Provide clear escalation paths when self-service solutions are insufficient
- Document known issues, workarounds, and resolution timelines

## User Feedback Integration
- Design feedback collection mechanisms that capture specific usability issues
- Implement systematic processes for incorporating user feedback into content updates
- Track content performance metrics and user satisfaction scores
- Create user testing protocols for validating content effectiveness
- Establish regular content review cycles based on user behavior and feedback data
```

#### Create `.github/instructions/content-architecture.instructions.md`:

```markdown
---
applyTo: "**/*information*,**/*structure*,**/*taxonomy*,**/*architecture*"
description: "Information architecture and content structure design standards"
---

# Content Architecture Procedural Memory

## Information Architecture Principles
- Design content structures that match user mental models and task flows
- Create hierarchical organization that supports both browsing and searching
- Implement consistent labeling and categorization systems across all content
- Design flexible architectures that can accommodate growth and change
- Use card sorting and tree testing methodologies to validate information structures

## Content Taxonomy and Classification
- Develop comprehensive tagging systems that enable content discovery and reuse
- Create standardized vocabulary and terminology across all content types
- Implement content types and templates that ensure structural consistency
- Design metadata schemas that support content management and automation
- Establish content relationship models that enable intelligent cross-referencing

## Navigation and Wayfinding Design
- Create clear, predictable navigation patterns that support user orientation
- Design breadcrumb systems and contextual navigation aids
- Implement search functionality that aligns with user search behavior patterns
- Create landing pages and content hubs that orient users to available information
- Design responsive navigation systems that work across different devices and contexts

## Content Lifecycle Architecture
- Design content creation workflows that ensure quality and consistency
- Implement version control and content approval processes
- Create content archival and sunsetting procedures that maintain link integrity
- Design content migration strategies that preserve user experience
- Establish content governance models that scale with organizational growth

## Scalability and Maintenance Planning
- Design modular content architectures that support reuse and repurposing
- Create automated content checking and validation systems
- Implement content performance monitoring and optimization processes
- Plan for internationalization and localization requirements in content architecture
- Design backup and disaster recovery procedures for content preservation
```

### Step 5: Technical Writing Episodic Memory Files

#### Create `.github/prompts/documentation-planning.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Documentation planning and strategy development workflow"
---

# Documentation Planning Episode Template

## Phase 1: User Research and Needs Analysis
- Conduct comprehensive user research to identify documentation needs and pain points
- Analyze user personas, journey maps, and task flows to understand information requirements
- Assess current content gaps and opportunities through user feedback and support data
- Evaluate competitor documentation strategies and industry best practices
- Define success metrics and measurement frameworks for documentation effectiveness

## Phase 2: Content Strategy and Architecture Design
- Develop comprehensive content strategy aligned with business objectives and user needs
- Design information architecture that supports multiple user access patterns
- Create content taxonomy and classification systems for scalable organization
- Plan content creation workflows and governance processes
- Establish content quality standards and review procedures

## Phase 3: Resource Planning and Timeline Development
- Assess required resources including writing, design, development, and review capabilities
- Create realistic project timelines that account for content creation, review, and iteration cycles
- Plan stakeholder engagement and subject matter expert collaboration workflows
- Design risk mitigation strategies for common documentation project challenges
- Establish change management processes for documentation updates and maintenance

## Phase 4: Implementation and Measurement Framework
- Create detailed implementation plans with clear milestones and deliverables
- Establish content performance monitoring and analytics frameworks
- Design user feedback collection and incorporation processes
- Plan regular content audits and optimization cycles
- Document lessons learned and best practices for future documentation projects

Focus on user-centered planning and measurable outcomes
```

#### Create `.github/prompts/content-creation.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "create_file", "read_file"]
description: "Content creation and writing workflow for technical documentation"
---

# Content Creation Episode Template

## Phase 1: Content Planning and Research
- Define specific content objectives and target audience for the content piece
- Conduct thorough research including subject matter expert interviews and technical validation
- Create content outline that aligns with user mental models and task flows
- Identify content dependencies, prerequisites, and integration points
- Plan visual elements, examples, and interactive components needed

## Phase 2: Content Development and Writing
- Write content using user-centered language and clear, actionable information
- Develop comprehensive examples, code samples, and visual aids
- Create logical content flow that supports both sequential reading and reference use
- Implement consistent style, tone, and formatting throughout content
- Include accessibility considerations and inclusive design principles

## Phase 3: Content Review and Validation
- Conduct technical accuracy review with subject matter experts
- Perform usability testing with representative users to validate content effectiveness
- Review content for consistency with style guide and brand standards
- Validate all examples, procedures, and code samples for accuracy
- Implement feedback and iterate on content based on review findings

## Phase 4: Content Publication and Optimization
- Prepare content for publication including final formatting and metadata
- Implement SEO optimization and discoverability enhancements
- Create content promotion and distribution strategies
- Establish monitoring and analytics tracking for content performance
- Plan regular content review and update cycles based on user feedback and analytics

Focus on user validation and iterative improvement
```

#### Create `.github/prompts/api-reference.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "API reference documentation creation workflow"
---

# API Reference Creation Episode Template

## Phase 1: API Analysis and Documentation Planning
- Conduct comprehensive analysis of API endpoints, parameters, and response structures
- Identify developer personas and primary use cases for API consumption
- Plan documentation structure that supports both learning and reference scenarios
- Assess authentication, rate limiting, and error handling requirements
- Create comprehensive content inventory and organization strategy

## Phase 2: Reference Documentation Development
- Document all endpoints with complete parameter descriptions and constraints
- Create comprehensive request and response examples with realistic data
- Develop code samples in multiple programming languages and frameworks
- Document authentication flows, error codes, and troubleshooting guidance
- Create interactive examples and testing capabilities where possible

## Phase 3: Developer Experience Enhancement
- Design getting-started guides that enable rapid API adoption
- Create comprehensive SDK documentation and integration guides
- Develop sample applications and real-world use case examples
- Implement search and navigation systems optimized for developer workflows
- Create troubleshooting guides and FAQ sections based on common developer issues

## Phase 4: Testing and Developer Validation
- Test all documentation examples and code samples for accuracy and completeness
- Conduct usability testing with representative developers to validate documentation effectiveness
- Implement feedback collection mechanisms for continuous improvement
- Establish synchronization processes between API changes and documentation updates
- Create maintenance workflows for keeping documentation current with API evolution

Focus on developer productivity and accurate technical implementation
```

#### Create `.github/prompts/tutorial-development.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Tutorial and how-to guide development workflow"
---

# Tutorial Development Episode Template

## Phase 1: Learning Objective Definition and User Analysis
- Define clear, measurable learning objectives for the tutorial
- Analyze target audience skills, knowledge level, and context of use
- Identify prerequisite knowledge and skills required for tutorial success
- Map tutorial content to specific user tasks and real-world scenarios
- Plan progressive learning structure that builds confidence and competence

## Phase 2: Tutorial Structure and Content Development
- Create logical learning progression from simple to complex concepts
- Develop hands-on exercises and practical examples that reinforce learning
- Include checkpoint assessments and validation steps throughout tutorial
- Create clear, action-oriented instructions with visual support
- Design alternative pathways for different learning styles and preferences

## Phase 3: Interactive Elements and Engagement Design
- Incorporate interactive examples, simulations, or live demonstrations
- Create practice exercises that allow learners to apply concepts immediately
- Design feedback mechanisms that help learners self-assess progress
- Include troubleshooting guidance for common learning obstacles
- Plan multimedia elements that enhance learning without creating cognitive overload

## Phase 4: Testing and Learning Effectiveness Validation
- Conduct usability testing with representative learners to validate tutorial effectiveness
- Measure learning outcomes and completion rates through assessment and analytics
- Gather feedback on tutorial clarity, pacing, and usefulness
- Iterate on tutorial content based on learner performance and feedback
- Establish maintenance processes for keeping tutorial content current and accurate

Focus on progressive learning and practical skill development
```

#### Create `.github/prompts/content-audit.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Content audit and quality assessment workflow"
---

# Content Audit Episode Template

## Phase 1: Audit Scope Definition and Baseline Assessment
- Define audit objectives including quality standards, user experience goals, and business alignment
- Establish comprehensive content inventory with metadata and classification
- Assess current content performance using analytics, user feedback, and support data
- Identify audit criteria including accuracy, usability, accessibility, and strategic alignment
- Plan audit methodology and resource allocation for comprehensive assessment

## Phase 2: Content Quality and Accuracy Assessment
- Evaluate technical accuracy through subject matter expert review and verification
- Assess content currency and relevance for current product versions and user needs
- Review content completeness and identify gaps in coverage or information
- Evaluate content consistency across style, tone, formatting, and structural standards
- Assess accessibility compliance and inclusive design implementation

## Phase 3: User Experience and Effectiveness Evaluation
- Analyze content usability through user testing and behavior analytics
- Evaluate information architecture and navigation effectiveness
- Assess content discoverability through search behavior and success metrics
- Review content task completion rates and user satisfaction scores
- Evaluate content performance across different devices and access methods

## Phase 4: Optimization Recommendations and Implementation Planning
- Prioritize content improvements based on user impact and business value
- Create detailed improvement recommendations with implementation guidance
- Develop content optimization roadmap with realistic timelines and resource requirements
- Plan content archival, consolidation, or migration strategies for underperforming content
- Establish ongoing content quality monitoring and review processes

Focus on data-driven improvement and user impact maximization
```

### Step 6: Meta-Cognitive Files Integration

The learning.instructions.md, meta-cognition.instructions.md, consolidation.prompt.md, self-assessment.prompt.md, meta-learning.prompt.md, and cognitive-health.prompt.md files from previous setups apply to technical writing as well, focusing on continuous improvement of technical writing capabilities.

## 📝 Technical Writing Setup Validation

After creating all files, verify technical writing setup:

1. **Check technical writing file structure**: Ensure all directories and writing-specific files exist
2. **Validate VS Code settings**: Confirm technical writing instruction files are recognized
3. **Test technical writing activation**: Try technical writing "@" commands in Copilot chat
4. **Verify content organization**: Check that content workflows and governance are properly structured

## 🚀 Technical Writing Quick Start Commands

After setup, test with these technical writing-specific commands:

**Technical Writing Tests**:
- `@workspace Help me plan comprehensive API documentation` (Should activate documentation-planning.prompt.md)
- `Create user-centered tutorial content` (Should activate tutorial-development.prompt.md)
- `Develop technical specification document` (Should activate content-creation.prompt.md)

**Content Strategy Tests**:
- `Design information architecture for documentation` (Should activate information-architecture.prompt.md)
- `Conduct comprehensive content audit` (Should activate content-audit.prompt.md)
- `Optimize content for user experience` (Should activate content-optimization.prompt.md)

**Meta-Technical Writing Tests**:
- `@workspace Assess your technical writing assistance quality` (Should activate self-assessment.prompt.md)
- `How can you improve documentation strategy support?` (Should activate meta-learning.prompt.md)
- `Monitor your technical writing architecture health` (Should activate cognitive-health.prompt.md)

## ⚡ Technical Writing Success Indicators

Your technical writing cognitive architecture is working when:

- **User-Centered Design**: All content prioritizes user needs and task completion
- **Clarity and Precision**: Content is clear, accurate, and actionable
- **Systematic Improvement**: Content continuously improves based on user feedback and analytics
- **Quality Consistency**: All content meets established style and quality standards
- **Accessibility Compliance**: Content is accessible to users with diverse abilities and contexts
- **Strategic Alignment**: Documentation strategy aligns with business objectives and user outcomes
- **Meta-Cognitive Growth**: System continuously improves technical writing capabilities and processes

---

**SETUP COMPLETE**: Your technical writing cognitive architecture is now ready for comprehensive documentation strategy, user-centered content creation, and systematic quality improvement. The system maintains focus on user needs while providing sophisticated writing support and strategic guidance for all aspects of technical communication.
