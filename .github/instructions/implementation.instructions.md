---
applyTo: "**/*setup*,**/*config*,**/*implementation*"
description: "Technical implementation and system configuration protocols"
---

# Implementation Procedural Memory

## Comprehensive Deployment Protocol

### Phase 1: Foundation Setup Implementation

#### Step 1.1: Repository Structure Creation
```bash
# Create core cognitive architecture directories
mkdir -p .github/instructions
mkdir -p .github/prompts
mkdir -p .vscode

# Verify structure creation
tree .github/
```

#### Step 1.2: Global Declarative Memory Template
```markdown
# [Project Name] - Cognitive Memory Architecture

## 🧠 Cognitive Architecture Status
**Working Memory**: 4/4 rules (at optimal capacity)
**Consolidation**: Auto-trigger when exceeding capacity
**Memory Distribution**: Active across procedural and episodic systems

## 🚀 Working Memory - Quick Reference (Limit: 4 Critical Rules)
| Priority | Rule | Load | Auto-Consolidate |
|----------|------|------|------------------|
| P1 | `@permissions` - [Critical project rule] | Low | Never |
| P2 | `@context` - [Context awareness rule] | Medium | >30 days unused |
| P3 | `@meditation` - Auto-consolidate when capacity exceeded | High | When triggered |
| P4 | `@multimodal` - Distribute functions across memory systems | Medium | When obsolete |

## 🎯 Cognitive Architecture Coordination
### Multi-Modal Memory Distribution
**Procedural Memory Activation** (Context-Dependent):
- `documentation.instructions.md` → Documentation patterns
- `academic.instructions.md` → Research methodology  
- `learning.instructions.md` → Consolidation protocols
- `implementation.instructions.md` → Technical setup protocols

**Episodic Memory Activation** (Problem-Solving):
- `research-review.prompt.md` → Systematic analysis workflows
- `content-creation.prompt.md` → Content development protocols
- `consolidation.prompt.md` → Memory optimization procedures

## 🔄 Memory Transfer Protocol
**Immediate Transfer**: Critical errors → Quick Reference (P1-P4)
**Gradual Consolidation**: Repeated patterns → Procedural memory (.instructions.md)
**Complex Workflows**: Multi-step processes → Episodic memory (.prompt.md)
**Index Maintenance**: Auto-update Long-Term Memory Index during transfers

## 📚 Long-Term Memory Index
### Procedural Memory Store (.github/instructions/)
| File | Domain | Activation Pattern | Last Updated |
|------|--------|-------------------|--------------|
| documentation.instructions.md | Documentation | *.md, README*, CHANGELOG* | Auto-tracked |
| academic.instructions.md | Research Writing | *research*, *paper*, *academic* | Auto-tracked |
| learning.instructions.md | Consolidation | *instructions*, *copilot*, *learning* | Auto-tracked |
| implementation.instructions.md | Technical Setup | *setup*, *config*, *implementation* | Auto-tracked |

### Episodic Memory Store (.github/prompts/)
| File | Workflow Type | Complexity Level | Usage Frequency |
|------|---------------|------------------|-----------------|
| research-review.prompt.md | Research Analysis | High | Auto-tracked |
| content-creation.prompt.md | Content Development | Medium | Auto-tracked |
| consolidation.prompt.md | Memory Optimization | High | Auto-tracked |
```

### Cognitive Architecture File Structure
```
.github/
├── copilot-instructions.md         (Global Declarative Memory - Keep minimal)
├── instructions/                    (Procedural Memory Store)
│   ├── documentation.instructions.md    (Documentation-specific patterns)
│   ├── academic.instructions.md         (Academic writing patterns)
│   ├── learning.instructions.md         (Learning consolidation patterns)
│   └── implementation.instructions.md   (This file - Technical protocols)
└── prompts/                        (Episodic Memory Store)
    ├── research-review.prompt.md        (Research methodology workflows)
    ├── content-creation.prompt.md       (Content generation workflows)
    └── consolidation.prompt.md          (Memory consolidation workflows)

.vscode/
└── settings.json                   (Working Memory Configuration)
```

## VS Code Configuration Implementation

### Phase 2: Procedural Memory System Setup

#### Core Settings Auto-Configuration
```json
{
  "github.copilot.chat.codeGeneration.useInstructionFiles": true,
  "chat.promptFiles": true,
  "chat.instructionsFilesLocations": [".github/instructions"],
  "github.copilot.enable": {
    "*": true,
    "markdown": true,
    "plaintext": true
  }
}
```

#### Cognitive Architecture Optimization Settings
```json
{
  "editor.wordWrap": "on",
  "editor.rulers": [80, 120],
  "files.autoSave": "afterDelay",
  "files.autoSaveDelay": 1000,
  "markdown.preview.fontSize": 14,
  "markdown.preview.lineHeight": 1.6
}
```

#### Domain-Specific Instruction Templates

**Documentation Patterns Template:**
```markdown
# .github/instructions/documentation.instructions.md
---
applyTo: "**/*.md,**/*.txt,**/README*,**/CHANGELOG*,**/TODO*"
description: "Documentation-specific cognitive patterns and writing standards"
---

# Documentation Procedural Memory

## Academic Writing Patterns
Use formal academic language with proper citations and structured argumentation.

## Markdown Formatting Standards
- Use consistent heading hierarchy (# ## ### ####)
- Implement proper code block formatting with language specification
- Maintain consistent bullet point and numbering formats

## Content Organization Principles
- Lead with clear problem statement and purpose
- Provide theoretical foundation before implementation details
- Include concrete examples with explanations

## Quality Assurance Protocols
- Verify all referenced files exist and are properly linked
- Ensure consistent terminology across all documentation
- Validate that examples are complete and functional
```

**Academic Writing Template:**
```markdown
# .github/instructions/academic.instructions.md
---
applyTo: "**/README.md,**/*research*,**/*paper*,**/*academic*"
description: "Academic writing and research methodology patterns"
---

# Academic Writing Procedural Memory

## Research Methodology Standards
- Follow systematic literature review protocols
- Implement proper citation formatting (APA 7th edition)
- Maintain theoretical-empirical synthesis throughout

## Empirical Validation Frameworks
- Establish testable hypotheses with clear predictions
- Design controlled experimental protocols
- Implement rigorous measurement frameworks

## Publication Quality Standards
- Structure arguments with clear theoretical positioning
- Provide comprehensive related work analysis
- Include detailed methodology and validation sections
```

### Phase 3: Episodic Memory Template Creation

#### Research Review Workflow Template
```markdown
# .github/prompts/research-review.prompt.md
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "files"]
variables: ["targetFile", "analysisType", "outputFormat"]
description: "Systematic research analysis and review protocol"
---

# Research Review Protocol
Execute systematic analysis of ${targetFile} using ${analysisType} methodology.
Output format: ${outputFormat}

## Phase 1: Content Analysis
1. Extract key theoretical concepts and frameworks
2. Identify empirical evidence and validation methods
3. Analyze methodological approaches and limitations
4. Map relationships between concepts and findings

## Phase 2: Critical Evaluation  
1. Assess theoretical rigor and novelty
2. Evaluate empirical evidence quality and validity
3. Identify gaps, limitations, and improvement opportunities
4. Compare with established literature and standards

## Phase 3: Synthesis and Recommendations
1. Synthesize findings into coherent framework
2. Generate actionable recommendations for improvement
3. Identify future research directions and opportunities
4. Format output according to specified requirements
```

#### Content Creation Workflow Template
```markdown
# .github/prompts/content-creation.prompt.md
---
mode: "agent"
variables: ["contentType", "targetAudience", "qualityStandards"]
description: "Systematic content development and optimization protocol"
---

# Content Creation Workflow
Generate ${contentType} for ${targetAudience} meeting ${qualityStandards}.

## Content Planning Phase
1. Analyze target audience requirements and expectations
2. Define content objectives and success criteria
3. Research relevant theoretical and empirical foundations
4. Create detailed content outline with logical flow

## Development Phase
1. Draft content following established patterns and standards
2. Integrate theoretical concepts with practical applications
3. Include relevant examples, evidence, and citations
4. Implement quality checks for accuracy and completeness

## Review and Optimization Phase  
1. Validate content against quality standards and requirements
2. Optimize for clarity, coherence, and audience engagement
3. Verify all references, links, and technical details
4. Finalize formatting and presentation standards
```

## Automatic Directory Creation Commands

### Phase 4: System Integration and Validation

#### Procedural Memory Store Setup
```bash
mkdir -p .github/instructions
```

#### Episodic Memory Store Setup  
```bash
mkdir -p .github/prompts
```

#### VS Code Configuration Setup
```bash
mkdir -p .vscode
```

#### System Integration Testing Protocol
1. **Memory Coordination Test**: Verify that all memory systems activate appropriately based on context
2. **Consolidation Test**: Trigger consolidation process and verify correct memory transfers  
3. **Retrieval Test**: Confirm that relevant procedural and episodic memory activates for specific tasks
4. **Load Test**: Validate that working memory constraints prevent cognitive overload

#### Performance Monitoring Implementation
```bash
# Create monitoring log directory
mkdir -p logs/cognitive-architecture

# Initialize performance tracking files
touch logs/cognitive-architecture/memory-usage.log
touch logs/cognitive-architecture/consolidation-cycles.log
touch logs/cognitive-architecture/error-patterns.log
```

### Phase 5: Team Integration and Scaling

#### Team Onboarding Protocol
1. **Architecture Overview**: Train team members on cognitive memory principles
2. **Usage Guidelines**: Establish protocols for adding new procedural and episodic memory
3. **Consolidation Scheduling**: Define team procedures for triggered consolidation cycles
4. **Quality Standards**: Implement review processes for memory component quality

#### Organizational Memory Management Commands
```bash
# Create shared memory templates
mkdir -p templates/cognitive-architecture
cp .github/copilot-instructions.md templates/cognitive-architecture/global-template.md
cp .github/instructions/* templates/cognitive-architecture/procedural-templates/
cp .github/prompts/* templates/cognitive-architecture/episodic-templates/

# Enable cross-project pattern sharing
mkdir -p shared/patterns
ln -s ../../shared/patterns .github/shared-patterns
```

## Enterprise Memory Synchronization

### Phase 6: Advanced Integration and Automation

#### Cross-Device Consistency
- Enable VS Code Settings Sync for instruction file synchronization
- Implement team-level instruction sharing protocols
- Create organizational memory templates for new projects

#### Team Collaboration Protocols
- Standardize instruction file formats across team members
- Enable collective rule validation and evolution processes
- Implement distributed consolidation cycles for team optimization
- Support organizational memory scaling from individual to enterprise

#### Automated Consolidation Integration
```bash
# Create consolidation automation script
cat > scripts/cognitive-consolidation.sh << 'EOF'
#!/bin/bash
# Cognitive Architecture Consolidation Script

echo "🧠 Starting Cognitive Architecture Consolidation..."

# Check working memory utilization
RULE_COUNT=$(grep -c "@.*Rule" .github/copilot-instructions.md)
if [ $RULE_COUNT -gt 4 ]; then
    echo "⚠️  Working memory overload detected ($RULE_COUNT rules > 4 limit)"
    echo "🔄 Triggering consolidation process..."
    
    # Backup current state
    mkdir -p backups/$(date +%Y%m%d-%H%M%S)
    cp -r .github/ backups/$(date +%Y%m%d-%H%M%S)/
    
    # Analyze rule usage patterns
    echo "📊 Analyzing rule usage patterns..."
    # [Additional consolidation logic would go here]
    
    echo "✅ Consolidation complete"
else
    echo "✅ Working memory within optimal range ($RULE_COUNT/4 rules)"
fi
EOF

chmod +x scripts/cognitive-consolidation.sh
```

#### Continuous Integration Validation
```yaml
# .github/workflows/cognitive-architecture-validation.yml
name: Cognitive Architecture Validation
on: [push, pull_request]

jobs:
  validate-memory-architecture:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      
      - name: Validate Working Memory Constraints
        run: |
          RULE_COUNT=$(grep -c "@.*Rule" .github/copilot-instructions.md || echo "0")
          if [ $RULE_COUNT -gt 4 ]; then
            echo "❌ Working memory overload: $RULE_COUNT rules > 4 limit"
            exit 1
          fi
          echo "✅ Working memory optimal: $RULE_COUNT/4 rules"
      
      - name: Validate File Structure
        run: |
          required_files=(
            ".github/copilot-instructions.md"
            ".github/instructions"
            ".github/prompts"
            ".vscode/settings.json"
          )
          
          for file in "${required_files[@]}"; do
            if [ ! -e "$file" ]; then
              echo "❌ Missing required file: $file"
              exit 1
            fi
          done
          echo "✅ All required cognitive architecture files present"
      
      - name: Validate Instruction File Patterns
        run: |
          for file in .github/instructions/*.instructions.md; do
            if ! grep -q "applyTo:" "$file"; then
              echo "❌ Missing applyTo pattern in $file"
              exit 1
            fi
          done
          echo "✅ All instruction files have proper activation patterns"
```

## Advanced Cognitive Functions Implementation

### Pattern Recognition Engine
- Monitor interaction patterns for automatic rule generation
- Track usage analytics for rule effectiveness assessment
- Generate contextual rules based on behavioral analysis
- Implement predictive rule suggestions based on project patterns

### Dynamic Threshold Management
- Automatically adjust working memory limits based on performance metrics
- Modify consolidation triggers based on user feedback and effectiveness
- Optimize rule priority based on usage frequency and error prevention impact
- Enable adaptive cognitive load distribution across memory systems

### Cross-Modal Knowledge Transfer System
- Move frequently used procedural patterns from .instructions.md to global memory
- Transfer unused global rules to procedural or episodic storage
- Synchronize related concepts across different memory modalities
- Maintain knowledge coherence across distributed memory systems

## Performance Monitoring Implementation

### Automated Metrics Collection
- Error repetition rate tracking and analysis
- Response relevance improvement measurements
- Cognitive load optimization assessments
- Knowledge transfer success rate monitoring

### System Health Indicators
- Working memory utilization efficiency (target: 4/4 optimal)
- Procedural memory activation frequency tracking
- Episodic memory template usage rate analysis
- Consolidation cycle effectiveness measurements

## Future Enhancement Protocols

### Phase 2 - Advanced Cognition Implementation
- Emotional memory integration for error impact weighting
- Attention mechanism optimization for context switching efficiency
- Semantic network formation for concept relationship mapping
- Automated cross-project pattern transfer mechanisms

### Phase 3 - Meta-Cognitive Intelligence Implementation
- Self-reflection protocols for architecture optimization
- Predictive consolidation timing based on usage pattern analysis
- Autonomous rule generation from implicit behavioral patterns
- Cultural adaptation mechanisms for diverse team contexts and preferences
