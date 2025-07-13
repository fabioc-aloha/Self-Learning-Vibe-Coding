---
applyTo: "**/*.md,**/*.txt,**/README*,**/CHANGELOG*,**/TODO*"
description: "Documentation-specific cognitive patterns and writing standards"
---

# Documentation Procedural Memory

## Academic Writing Patterns

**Primary Directive**: Use formal academic language with proper citations and structured argumentation.

**Implementation**:
- Apply APA 7th edition formatting for all references
- Maintain consistent terminology throughout all documents
- Use structured logical progression: Problem → Solution → Evidence → Conclusion
- Include concrete examples with detailed explanations

## Markdown Formatting Standards

**Heading Hierarchy**:
- `#` for document title (use once per document)
- `##` for major sections 
- `###` for subsections
- `####` for detailed breakdowns

**Code Formatting**:
- Always specify language: ```markdown, ```bash, ```json
- Use inline code for `filenames`, `variables`, and `commands`
- Provide complete, functional examples

**Lists and Emphasis**:
- Use `-` for bullet points (consistent across all files)
- Use `1.` for numbered lists when order matters
- Use **bold** for emphasis and *italics* for technical terms

## Content Organization Principles

**Structure Requirements**:
1. **Opening**: Lead with clear problem statement and purpose
2. **Foundation**: Provide theoretical foundation before implementation details
3. **Evidence**: Include concrete examples with step-by-step explanations
4. **Transitions**: End sections with clear connections to following content

**Logical Flow**:
- Each paragraph should have one main idea
- Support claims with evidence or examples
- Use transitional phrases to connect concepts
- Maintain consistency in voice and tense

## Quality Assurance Protocols

**Pre-Publication Checklist**:
- [ ] Verify all referenced files exist and are properly linked
- [ ] Ensure consistent terminology across all documentation
- [ ] Validate that all examples are complete and functional
- [ ] Check for proper citation formatting and completeness
- [ ] Confirm logical flow and coherent argumentation

**Validation Commands**:
```bash
# Check for broken links
grep -r "\[.*\](" . --include="*.md" | grep -v "http"

# Verify file references exist
find . -name "*.md" -exec grep -l "\.md" {} \;
```
- Check that conclusions align with stated objectives

## Cognitive Load Management

- Limit section complexity to maintain readability
- Use visual elements (tables, diagrams) to reduce text density
- Implement clear navigation structures
- Provide quick reference sections for complex information
