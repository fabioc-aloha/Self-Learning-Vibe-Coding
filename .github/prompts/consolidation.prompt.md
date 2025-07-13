---
mode: "agent"
model: "gpt-4"
tools: ["workspace"]
description: "Memory consolidation and cognitive architecture optimization workflow"
---

# Memory Consolidation Episode Template

**ACTIVATION**: Use this template when working memory exceeds 4 rules, conflicts are detected, or user requests cognitive architecture optimization.

**EXECUTION MODE**: Systematic meditation protocol with automated file creation and memory optimization.

## Phase 1: Cognitive Load Assessment

**Primary Objective**: Evaluate current memory system state and identify optimization opportunities.

**1.1 Working Memory Analysis**
- Count current rules in quick reference (optimal limit: 4)
- Identify which rules exceed capacity limit
- Assess rule clarity and actionability
- Document usage frequency patterns

**1.2 Rule Effectiveness Assessment**
- Measure usage patterns over recent sessions
- Evaluate error prevention impact and success rates
- Identify highly effective rules for promotion
- Document rules that provide minimal value

**1.3 Conflict Detection Protocol**
- Search for contradictory instructions across memory systems
- Identify redundant or overlapping rules
- Flag ambiguous instructions requiring clarification
- Document resolution priorities based on impact

**1.4 Performance Metrics Review**
- Analyze response time and relevance indicators
- Review user satisfaction and system effectiveness
- Identify areas of cognitive overload or inefficiency
- Document patterns indicating need for consolidation

## Phase 2: Knowledge Categorization

Organize information for optimal retrieval:

1. **Priority Classification**: Rank rules by frequency and impact
2. **Context Grouping**: Cluster related concepts and procedures
3. **Temporal Relevance**: Identify obsolete or outdated patterns
4. **Transfer Candidates**: Select rules for procedural or episodic memory

## Phase 3: Architecture Restructuring with Automatic File Creation

Implement systematic reorganization with automated memory file generation:

### 3.1 Working Memory Optimization
- **Promote critical rules** to quick reference (maintain 4-rule limit)
- **Archive excess rules** to appropriate memory systems
- **Resolve conflicts** through priority hierarchy

### 3.2 Procedural Memory Distribution (Auto-Create .instructions.md files)

**Automatically create specialized instruction files** when consolidating task-specific patterns:

```bash
# Auto-create directories if needed
mkdir -p .github/instructions
```

**Pattern-Based File Creation**:
- **Documentation patterns** → Create `documentation.instructions.md`
- **Academic writing patterns** → Create `academic.instructions.md`  
- **Learning/consolidation patterns** → Create `learning.instructions.md`
- **Technical implementation patterns** → Create `implementation.instructions.md`
- **Security/API patterns** → Create `security.instructions.md`
- **Testing patterns** → Create `testing.instructions.md`

**File Template for New .instructions.md**:
```markdown
---
applyTo: "**/{pattern-specific-glob}"
description: "{Context-specific cognitive patterns}"
---

# {Domain} Procedural Memory

## {Consolidated patterns from working memory}
{Move specific rules and procedures here}

## {Context-specific protocols}
{Domain-specific implementation details}
```

### 3.3 Episodic Template Creation (Auto-Create .prompt.md files)

**Automatically create workflow templates** when consolidating complex multi-step processes:

```bash
# Auto-create directories if needed
mkdir -p .github/prompts
```

**Workflow-Based Template Creation**:
- **Research analysis workflows** → Create `research-analysis.prompt.md`
- **Content creation workflows** → Create `content-creation.prompt.md`
- **Code review workflows** → Create `code-review.prompt.md`
- **Debugging workflows** → Create `debugging.prompt.md`
- **Refactoring workflows** → Create `refactoring.prompt.md`

**File Template for New .prompt.md**:
```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "relevant-tools"]
description: "{Workflow-specific description}"
---

# {Workflow} Episode Template

## Phase 1: {Initial Assessment}
{Consolidated workflow steps}

## Phase 2: {Process Execution}
{Systematic procedures}

## Phase 3: {Validation and Output}
{Quality assurance and results}

Use project-specific patterns from ${workspaceFolder}
```

### 3.4 Automatic File Creation and Index Update Protocol

**When consolidating, automatically execute**:

1. **Assess rule categories** and identify file creation needs
2. **Create directories** if they don't exist:
   ```bash
   mkdir -p .github/instructions
   mkdir -p .github/prompts
   ```
3. **Generate appropriate files** based on consolidated patterns
4. **Transfer rules** from working memory to new files
5. **Update global copilot-instructions.md** with long-term memory index

### 3.5 Long-Term Memory Index Management

**Automatically update the main cognitive file** with an index of distributed memory files:

**Add/Update this section in `.github/copilot-instructions.md`**:

```markdown
## 📚 Long-Term Memory Index

### Procedural Memory Store (.github/instructions/)
| File | Domain | Activation Pattern | Last Updated |
|------|--------|-------------------|--------------|
| documentation.instructions.md | Documentation | *.md, README*, CHANGELOG* | {auto-date} |
| academic.instructions.md | Research Writing | *research*, *paper*, *academic* | {auto-date} |
| learning.instructions.md | Consolidation | *instructions*, *copilot*, *learning* | {auto-date} |
| implementation.instructions.md | Technical Setup | *setup*, *config*, *implementation* | {auto-date} |
| security.instructions.md | Security Patterns | auth/**, api/**, security/** | {auto-date} |
| testing.instructions.md | Testing Protocols | tests/**, spec/**, *.test.* | {auto-date} |

### Episodic Memory Store (.github/prompts/)
| File | Workflow Type | Complexity Level | Usage Frequency |
|------|---------------|------------------|-----------------|
| research-review.prompt.md | Research Analysis | High | {usage-count} |
| content-creation.prompt.md | Content Development | Medium | {usage-count} |
| consolidation.prompt.md | Memory Optimization | High | {usage-count} |
| code-review.prompt.md | Code Analysis | Medium | {usage-count} |
| debugging.prompt.md | Problem Solving | High | {usage-count} |

### Memory Transfer Log
- **Last Consolidation**: {timestamp}
- **Rules Transferred**: {count} from working memory
- **Files Created**: {new-file-list}
- **Cognitive Load Reduction**: {percentage}%
```

**Index Update Algorithm**:

1. **Scan existing files** in `.github/instructions/` and `.github/prompts/`
2. **Extract metadata** from each file's frontmatter (applyTo, description)
3. **Track usage patterns** and last modification dates
4. **Generate table entries** with current information
5. **Update the Long-Term Memory Index section** in main cognitive file
6. **Maintain transfer logs** for consolidation history

## Phase 4: Validation and Index Verification

Ensure consolidated architecture effectiveness and index accuracy:

1. **Performance Testing**: Verify improved response relevance and speed
2. **Cognitive Load Verification**: Confirm optimal information density
3. **Knowledge Transfer**: Test cross-modal information accessibility
4. **File Integration**: Validate new .instructions.md and .prompt.md files function correctly
5. **Index Accuracy**: Verify long-term memory index reflects actual file structure
6. **Cross-Reference Validation**: Ensure all indexed files exist and are properly formatted
7. **Usage Tracking**: Initialize monitoring for new files in the index
8. **Adaptation Mechanisms**: Enable continuous learning and adjustment

## Consolidation Triggers

Automatically initiate this protocol when:
- Working memory exceeds 4 concurrent rules
- Rule conflicts detected
- Performance degradation observed
- Usage patterns indicate decay (>30 days unused)
- User explicitly requests meditation/reorganization

## Memory File Creation Examples

### Example: Security Pattern Consolidation
When security-related rules accumulate in working memory:

**Auto-create** `security.instructions.md`:
```markdown
---
applyTo: "**/auth/**,**/api/**,**/security/**"
description: "Security-focused cognitive patterns"
---

# Security Procedural Memory
- Validate all inputs using joi or zod schemas
- Implement rate limiting on API endpoints  
- Use bcrypt with minimum 12 rounds for password hashing
```

### Example: Research Workflow Consolidation
When complex research procedures are identified:

**Auto-create** `research-methodology.prompt.md`:
```markdown
---
mode: "agent"
description: "Systematic research analysis workflow"
---

# Research Methodology Episode Template
Phase 1: Literature Context Analysis
Phase 2: Theoretical Positioning Assessment
Phase 3: Gap Analysis and Contribution Identification
```

Apply memory consolidation principles from cognitive psychology research and maintain alignment with established learning frameworks in ${workspaceFolder}. **Automatically create necessary .instructions.md and .prompt.md files** during consolidation to ensure optimal memory distribution and cognitive load management.
