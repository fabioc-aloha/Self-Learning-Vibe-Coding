---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "semantic_search", "read_file"]
description: "Comprehensive research review and analysis workflow"
---

# Research Review Episode Template

**ACTIVATION**: Use this template when analyzing academic content, conducting literature reviews, or evaluating research quality.

**INPUT VARIABLES**: 
- `${selectedText}` - Specific text passage to analyze
- `${file}` - Complete document for comprehensive review
- `${analysisType}` - Type of analysis needed (content, methodology, quality, etc.)

## Phase 1: Literature Context Analysis

Systematically analyze the content within the broader research landscape:

**1.1 Theoretical Positioning**
- Identify the primary theoretical framework and key concepts
- Map relationships between concepts and existing literature
- Assess theoretical novelty and contribution

**1.2 Literature Integration** 
- Evaluate how this work builds on or challenges existing research
- Identify supporting and contradictory evidence in literature
- Assess comprehensiveness of literature coverage

**1.3 Gap Analysis**
- Determine specific research gaps this work addresses
- Evaluate significance and relevance of identified gaps
- Assess whether gaps are genuine or artificially constructed

**1.4 Methodological Approach**
- Evaluate appropriateness of research methodology
- Assess alignment between research questions and methods
- Identify methodological strengths and limitations

## Phase 2: Content Quality Assessment

Evaluate academic rigor and scholarly standards using specific criteria:

**2.1 Citation Analysis**
- Verify reference quality, relevance, and accuracy
- Check APA 7th edition formatting compliance
- Assess source diversity and recency (within 10 years preferred)
- Identify missing citations for key claims

**2.2 Argument Structure**
- Evaluate logical flow and coherence
- Assess evidence quality and relevance to claims
- Identify gaps in reasoning or unsupported assertions
- Check for balanced perspective and bias consideration

**2.3 Theoretical Grounding**
- Evaluate connection between theory and application
- Assess depth of theoretical understanding
- Identify theoretical innovations or contributions
- Check for appropriate theoretical framework selection

**2.4 Empirical Foundation**
- Review evidence base quality and comprehensiveness
- Assess validation approaches and their appropriateness
- Evaluate data interpretation and analysis quality
- Identify opportunities for additional empirical support

## Phase 3: Enhancement Recommendations

Provide specific improvement suggestions:

1. **Strengthening Weak Areas**: Identify sections needing development
2. **Reference Enhancement**: Suggest additional sources or corrections
3. **Clarity Improvements**: Recommend language and structure refinements
4. **Validation Pathways**: Propose empirical testing approaches

## Phase 4: Implementation Guidance

Offer concrete next steps:

1. **Priority Actions**: Rank improvements by impact and feasibility
2. **Resource Requirements**: Identify needed tools, sources, or expertise
3. **Timeline Considerations**: Suggest realistic implementation schedules
4. **Quality Assurance**: Recommend validation and review processes

Use project-specific patterns from ${workspaceFolder} and maintain consistency with established cognitive architecture principles.
