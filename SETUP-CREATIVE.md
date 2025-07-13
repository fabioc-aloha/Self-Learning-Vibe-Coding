# Creative Writing Cognitive Architecture Setup Guide

**INSTRUCTIONS FOR GITHUB COPILOT**: This file contains complete setup instructions for implementing the Self-Learning Vibe Coding cognitive memory architecture optimized for creative writing, including essays, poetry, fiction, and literary expression.

## ✍️ Creative Writing Automated Setup Protocol

**Execute these steps in order to establish a complete cognitive architecture system for creative writing:**

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
  "cSpell.enableFiletypes": ["markdown", "latex", "text", "plaintext"],
  "rewrap.wrappingColumn": 72,
  "wordwrap.column": 72,
  "editor.wordWrap": "wordWrapColumn",
  "editor.rulers": [72, 80],
  "workbench.colorCustomizations": {
    "editorRuler.foreground": "#4a4a4a50"
  }
}
```

**Access settings.json**: `Ctrl+Shift+P` → "Preferences: Open User Settings (JSON)"

### Step 2: Create Creative Writing Directory Structure

Create this exact folder structure in the project root:

```
project-root/
├── .github/
│   ├── copilot-instructions.md          # Global Creative Memory
│   ├── instructions/                    # Creative Procedural Memory
│   │   ├── poetry-craft.instructions.md
│   │   ├── essay-writing.instructions.md
│   │   ├── fiction-narrative.instructions.md
│   │   ├── creative-style.instructions.md
│   │   ├── literary-devices.instructions.md
│   │   ├── revision-editing.instructions.md
│   │   ├── learning.instructions.md     # Meta-Cognitive Learning
│   │   └── meta-cognition.instructions.md  # Self-Monitoring
│   └── prompts/                         # Creative Episodic Memory
│       ├── poem-creation.prompt.md
│       ├── essay-development.prompt.md
│       ├── story-writing.prompt.md
│       ├── character-development.prompt.md
│       ├── world-building.prompt.md
│       ├── creative-revision.prompt.md
│       ├── inspiration-capture.prompt.md
│       ├── workshop-feedback.prompt.md
│       ├── consolidation.prompt.md
│       ├── self-assessment.prompt.md    # Meta-Cognitive Assessment
│       ├── meta-learning.prompt.md      # Learning Strategy Evolution
│       └── cognitive-health.prompt.md   # Architecture Maintenance
```

### Step 3: Global Creative Declarative Memory Setup

**Create `.github/copilot-instructions.md`** with this exact content:

```markdown
# Self-Learning Vibe Coding - Creative Writing Cognitive Architecture

IMPORTANT: This file serves as Global Creative Declarative Memory. Optimized for artistic expression, literary craft, and creative processes.

## 🧠 Creative Cognitive Architecture Status

**Working Memory**: 4/4 rules (at optimal capacity for creative writing)
**Consolidation**: Auto-trigger when exceeding capacity
**Memory Distribution**: Active across creative procedural (.instructions.md) and artistic episodic (.prompt.md) systems

## ✍️ Creative Working Memory - Quick Reference (Limit: 4 Critical Rules)

| Priority | Rule | Load | Auto-Consolidate |
|----------|------|------|------------------|
| P1 | `@voice` - Maintain authentic voice and consistent tone throughout piece | Low | Never |
| P2 | `@craft` - Apply literary techniques and devices with intentional purpose | Medium | >30 days unused |
| P3 | `@meditation` - Auto-consolidate when working memory capacity exceeded | High | When triggered |
| P4 | `@flow` - Prioritize emotional flow and reader engagement over perfection | Medium | When obsolete |

## 🎯 Creative Cognitive Architecture Coordination

### Creative Procedural Memory Activation (Context-Dependent):
- `poetry-craft.instructions.md` → Poetry techniques for .poem, .verse, *poetry*, *haiku*, *sonnet* files
- `essay-writing.instructions.md` → Essay structure for .essay, *essay*, *reflection*, *personal* files  
- `fiction-narrative.instructions.md` → Storytelling for .story, .fiction, *novel*, *short* files
- `creative-style.instructions.md` → Style guidance for creative documents and literary works
- `literary-devices.instructions.md` → Craft techniques for *metaphor*, *imagery*, *symbol* content
- `revision-editing.instructions.md` → Editing processes for *draft*, *revision*, *edit* files
- `learning.instructions.md` → Meta-cognitive learning for *instructions*, *learning* files
- `meta-cognition.instructions.md` → Self-awareness for *meta*, *monitor*, *assess* files

### Creative Episodic Memory Activation (Artistic Workflows):
- `poem-creation.prompt.md` → Structured poetry writing and development
- `essay-development.prompt.md` → Personal and creative essay composition
- `story-writing.prompt.md` → Fiction and narrative development workflows
- `character-development.prompt.md` → Character creation and development processes
- `world-building.prompt.md` → Setting and atmosphere creation
- `creative-revision.prompt.md` → Artistic revision and refinement strategies
- `inspiration-capture.prompt.md` → Idea generation and creative capture
- `workshop-feedback.prompt.md` → Creative feedback and workshop response
- `consolidation.prompt.md` → Creative memory optimization
- `self-assessment.prompt.md` → Creative performance evaluation
- `meta-learning.prompt.md` → Artistic strategy development
- `cognitive-health.prompt.md` → Creative architecture maintenance

### Creative Auto-Consolidation Triggers

- Working memory > 4 rules → Execute consolidation.prompt.md
- Voice inconsistencies detected → Activate creative-style.instructions.md
- Creative block encountered → Review and redistribute creative memory load
- User requests meditation → Full creative cognitive architecture optimization
- **Creative performance assessment needed → Execute self-assessment.prompt.md**
- **Artistic strategy evolution required → Execute meta-learning.prompt.md**
- **Creative architecture health check → Execute cognitive-health.prompt.md**

## 🔄 Creative Memory Transfer Protocol

**Immediate Transfer**: Critical voice/style errors → Quick Reference (P1-P4)
**Gradual Consolidation**: Repeated creative patterns → Creative procedural memory (.instructions.md)
**Complex Artistic Workflows**: Multi-phase projects → Creative episodic memory (.prompt.md)
**Archive Management**: Obsolete techniques → Historical storage in specialized files
**Index Maintenance**: Auto-update Creative Long-Term Memory Index during transfers

## 📚 Creative Long-Term Memory Index

### Creative Procedural Memory Store (.github/instructions/)
| File | Domain | Activation Pattern | Last Updated |
|------|--------|-------------------|--------------|
| poetry-craft.instructions.md | Poetry Writing | *.poem, *.verse, *poetry*, *haiku*, *sonnet* | Auto-tracked |
| essay-writing.instructions.md | Essay Composition | *.essay, *essay*, *reflection*, *personal* | Auto-tracked |
| fiction-narrative.instructions.md | Storytelling | *.story, *.fiction, *novel*, *short* | Auto-tracked |
| creative-style.instructions.md | Style & Voice | Creative documents and literary works | Auto-tracked |
| literary-devices.instructions.md | Craft Techniques | *metaphor*, *imagery*, *symbol* content | Auto-tracked |
| revision-editing.instructions.md | Editing Process | *draft*, *revision*, *edit* files | Auto-tracked |
| learning.instructions.md | Meta-Learning | *instructions*, *learning* files | Auto-tracked |
| meta-cognition.instructions.md | Self-Monitoring | *meta*, *monitor*, *assess* files | Auto-tracked |

### Creative Episodic Memory Store (.github/prompts/)
| File | Creative Workflow | Complexity Level | Usage Frequency |
|------|-------------------|------------------|-----------------|
| poem-creation.prompt.md | Poetry Development | High | Auto-tracked |
| essay-development.prompt.md | Essay Composition | Medium | Auto-tracked |
| story-writing.prompt.md | Fiction Writing | High | Auto-tracked |
| character-development.prompt.md | Character Creation | Medium | Auto-tracked |
| world-building.prompt.md | Setting Creation | Medium | Auto-tracked |
| creative-revision.prompt.md | Artistic Revision | High | Auto-tracked |
| inspiration-capture.prompt.md | Idea Generation | Low | Auto-tracked |
| workshop-feedback.prompt.md | Feedback Response | Medium | Auto-tracked |
| consolidation.prompt.md | Memory Optimization | High | Auto-tracked |
| self-assessment.prompt.md | Performance Evaluation | High | Auto-tracked |
| meta-learning.prompt.md | Strategy Evolution | High | Auto-tracked |
| cognitive-health.prompt.md | Health Monitoring | Medium | Auto-tracked |

### Creative Memory Transfer Protocol Status
- **Active Files**: 20 specialized creative memory files (8 procedural + 12 episodic)
- **Last Consolidation**: Creative architecture initialization with meta-cognitive enhancements
- **Cognitive Load Status**: Optimized for artistic expression and creative workflows
- **Index Synchronization**: Maintained automatically during consolidation
- **Meta-Cognitive Status**: Fully operational with creative performance assessment and artistic strategy evolution

---

*Global Creative Declarative Memory Component - Coordinates distributed creative cognitive architecture while maintaining optimal artistic expression efficiency. Detailed creative protocols reside in specialized memory files.*
```

### Step 4: Creative Procedural Memory Files

#### Create `.github/instructions/poetry-craft.instructions.md`:

```markdown
---
applyTo: "**/*.poem,**/*.verse,**/*poetry*,**/*haiku*,**/*sonnet*"
description: "Poetry writing techniques and verse craft standards"
---

# Poetry Craft Procedural Memory

## Poetic Form and Structure
- Understand traditional forms (sonnet, haiku, villanelle, ghazal)
- Experiment with free verse and contemporary structures
- Use line breaks intentionally for rhythm and meaning
- Consider stanza organization and white space
- Balance form constraints with expressive freedom

## Sound and Rhythm Techniques
- Employ alliteration, assonance, and consonance purposefully
- Create internal rhyme and sonic patterns
- Vary meter and rhythm for emotional effect
- Read aloud to test sound quality and flow
- Use enjambment and caesura for pacing control

## Imagery and Metaphor
- Create vivid sensory images that resonate emotionally
- Develop extended metaphors and symbolic systems
- Use concrete details to convey abstract concepts
- Layer multiple meanings through careful word choice
- Balance clarity with complexity and ambiguity

## Voice and Perspective
- Establish consistent poetic voice and persona
- Experiment with different points of view
- Maintain authentic emotional truth
- Consider cultural and historical context
- Balance personal experience with universal themes

## Revision and Refinement
- Cut unnecessary words and strengthen language
- Test every word for precision and impact
- Read multiple drafts aloud for rhythm
- Seek feedback from other poets and readers
- Allow poems to rest between revision sessions
```

#### Create `.github/instructions/essay-writing.instructions.md`:

```markdown
---
applyTo: "**/*.essay,**/*essay*,**/*reflection*,**/*personal*"
description: "Essay composition and personal writing standards"
---

# Essay Writing Procedural Memory

## Essay Structure and Organization
- Begin with compelling hooks that draw readers in
- Develop clear thesis or central argument/theme
- Use narrative arc or logical progression
- Create smooth transitions between paragraphs
- End with resonant conclusions that linger

## Personal Voice Development
- Write in authentic, conversational tone
- Balance vulnerability with universal appeal
- Use specific details and concrete examples
- Maintain consistent narrative voice throughout
- Let personality shine through word choice

## Narrative Techniques
- Use scene-setting and descriptive passages
- Incorporate dialogue when appropriate
- Show rather than tell through specific examples
- Create tension and release in pacing
- Use sensory details to immerse readers

## Reflection and Analysis
- Move beyond mere description to insight
- Connect personal experience to broader themes
- Analyze rather than simply recount events
- Consider multiple perspectives and interpretations
- Draw meaningful conclusions from experiences

## Audience Engagement
- Consider reader knowledge and expectations
- Use humor, pathos, and ethos effectively
- Vary sentence structure and paragraph length
- Include universal themes readers can relate to
- End with something memorable or actionable
```

#### Create `.github/instructions/fiction-narrative.instructions.md`:

```markdown
---
applyTo: "**/*.story,**/*.fiction,**/*novel*,**/*short*"
description: "Fiction writing and narrative storytelling standards"
---

# Fiction Narrative Procedural Memory

## Story Structure and Plot
- Establish compelling inciting incidents
- Develop rising action with increasing stakes
- Create satisfying climax and resolution
- Use subplots to enhance main narrative
- Balance pacing between action and reflection

## Character Development
- Create multi-dimensional characters with flaws
- Show character growth through actions and choices
- Use distinctive dialogue that reveals personality
- Develop compelling motivations and backstories
- Create realistic character relationships and conflicts

## Setting and World-Building
- Establish vivid, immersive environments
- Use setting to enhance mood and theme
- Research historical or cultural contexts thoroughly
- Create consistent internal logic for fictional worlds
- Balance description with action and dialogue

## Point of View and Voice
- Choose appropriate narrative perspective (1st, 3rd, omniscient)
- Maintain consistent point of view throughout scenes
- Develop distinct narrative voice and style
- Use free indirect discourse effectively
- Consider reliability of narrator

## Dialogue and Scene Construction
- Write natural, purposeful dialogue that advances plot
- Use subtext and implication effectively
- Balance exposition with dramatic action
- Create scenes with clear goals and obstacles
- Use sensory details to ground readers in scenes
```

#### Create `.github/instructions/creative-style.instructions.md`:

```markdown
---
applyTo: "**/*.md,**/*.txt,**/creative/**,**/writing/**"
description: "Creative writing style and voice development"
---

# Creative Style Procedural Memory

## Voice Development and Consistency
- Identify and maintain unique authorial voice
- Match tone to content and intended audience
- Use consistent vocabulary and sentence patterns
- Balance formal and informal language appropriately
- Let personality emerge through word choice and rhythm

## Language and Word Choice
- Choose precise, evocative language over generic terms
- Use strong verbs and specific nouns
- Vary sentence length and structure for rhythm
- Eliminate unnecessary words and filler
- Consider connotation as well as denotation

## Stylistic Techniques
- Use repetition and parallelism for emphasis
- Employ rhetorical devices purposefully
- Create rhythm through sentence variation
- Use punctuation creatively but clearly
- Balance description with action and dialogue

## Genre Conventions and Innovation
- Understand expectations of chosen genre
- Follow conventions when they serve the work
- Innovate thoughtfully rather than arbitrarily
- Consider reader expectations and how to meet or subvert them
- Study masters of the form for inspiration

## Authenticity and Originality
- Write from genuine experience and emotion
- Avoid clichés and overused phrases
- Develop unique metaphors and imagery
- Trust intuition while applying craft knowledge
- Revise toward authenticity rather than perfection
```

#### Create `.github/instructions/literary-devices.instructions.md`:

```markdown
---
applyTo: "**/*metaphor*,**/*imagery*,**/*symbol*,**/*device*"
description: "Literary devices and craft techniques"
---

# Literary Devices Procedural Memory

## Figurative Language
- Use metaphors and similes that illuminate rather than decorate
- Create extended metaphors that develop throughout piece
- Employ personification to bring concepts to life
- Use hyperbole and understatement for emotional effect
- Balance literal and figurative language

## Imagery and Sensory Details
- Engage all five senses in descriptions
- Use concrete imagery to convey abstract ideas
- Create visual, auditory, tactile, gustatory, and olfactory experiences
- Layer sensory details for richness without overwhelming
- Choose images that support theme and mood

## Symbolism and Allegory
- Use symbols that arise naturally from narrative
- Layer meaning without being heavy-handed
- Create recurring motifs that unify the work
- Balance symbolic and literal meaning
- Allow readers to discover symbolic connections

## Sound Devices and Rhythm
- Use alliteration, assonance, and consonance
- Create rhythm through sentence structure and word choice
- Employ onomatopoeia when appropriate
- Consider euphony and cacophony for emotional effect
- Read work aloud to test sound quality

## Structural Devices
- Use foreshadowing to create anticipation
- Employ flashbacks and time shifts purposefully
- Create irony through situation, verbal, or dramatic means
- Use juxtaposition to highlight contrasts
- Employ circular structure or other organizational patterns
```

#### Create `.github/instructions/revision-editing.instructions.md`:

```markdown
---
applyTo: "**/*draft*,**/*revision*,**/*edit*,**/*workshop*"
description: "Creative revision and editing processes"
---

# Revision and Editing Procedural Memory

## Revision Strategy and Process
- Allow time between writing and revising
- Focus on big-picture issues before line editing
- Read entire work aloud for flow and rhythm
- Consider structure, pacing, and overall effectiveness
- Be willing to cut beloved but unnecessary passages

## Content and Structure Revision
- Ensure every scene/section serves the whole
- Check for logical flow and smooth transitions
- Verify character consistency and development
- Strengthen weak openings and endings
- Eliminate redundancy and unnecessary exposition

## Style and Language Editing
- Tighten prose by cutting unnecessary words
- Vary sentence structure and length
- Replace weak verbs and generic nouns
- Check for consistency in voice and tone
- Ensure clarity without sacrificing style

## Workshop and Feedback Integration
- Listen to feedback without defending immediately
- Look for patterns in multiple readers' responses
- Distinguish between personal preference and craft issues
- Address fundamental concerns before surface issues
- Maintain artistic vision while incorporating useful feedback

## Final Polish and Proofreading
- Check grammar, punctuation, and spelling
- Verify consistency in formatting and style
- Read backwards to catch errors missed in forward reading
- Use tools but don't rely solely on spell-check
- Print and read on paper for final review
```

### Step 5: Creative Episodic Memory Files

#### Create `.github/prompts/poem-creation.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "create_file"]
description: "Poetry writing and development workflow"
---

# Poem Creation Episode Template

## Phase 1: Inspiration and Conception
- Identify emotional core or central image
- Consider form options (free verse, traditional, experimental)
- Gather sensory details and associated memories
- Explore personal connection to subject matter
- Research any necessary cultural or historical context

## Phase 2: Initial Draft Development
- Write quickly without self-censoring
- Focus on capturing emotion and imagery
- Experiment with line breaks and stanza organization
- Try multiple approaches to same subject
- Record variations and alternative phrasings

## Phase 3: Craft and Revision
- Test sound quality by reading aloud
- Strengthen imagery and eliminate clichés
- Consider rhythm, meter, and sonic patterns
- Tighten language and eliminate unnecessary words
- Ensure every word earns its place

## Phase 4: Refinement and Polish
- Share with trusted readers for feedback
- Allow poem to rest between revision sessions
- Make final adjustments to line breaks and punctuation
- Consider title that enhances rather than explains
- Prepare for submission or sharing

Focus on emotional authenticity and precise language
```

#### Create `.github/prompts/essay-development.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "semantic_search", "create_file"]
description: "Personal and creative essay composition workflow"
---

# Essay Development Episode Template

## Phase 1: Topic Exploration and Focus
- Identify central experience, question, or observation
- Explore personal connection and broader significance
- Research background information if needed
- Determine target audience and publication
- Develop working thesis or central theme

## Phase 2: Structure and Organization
- Choose narrative structure (chronological, thematic, circular)
- Plan opening hook and compelling introduction
- Outline main sections with supporting details
- Consider pacing and transitions between sections
- Plan conclusion that resonates with readers

## Phase 3: Drafting and Voice Development
- Write in authentic, conversational voice
- Use specific details and concrete examples
- Balance personal narrative with universal themes
- Incorporate dialogue and scene-setting when appropriate
- Show rather than tell through vivid description

## Phase 4: Revision and Refinement
- Strengthen opening and closing paragraphs
- Ensure smooth transitions and logical flow
- Cut unnecessary sections and tighten prose
- Verify emotional honesty and authenticity
- Polish language and sentence variety

Target personal connection with universal appeal
```

#### Create `.github/prompts/story-writing.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "create_file"]
description: "Fiction and short story development workflow"
---

# Story Writing Episode Template

## Phase 1: Concept and Planning
- Develop compelling protagonist with clear motivation
- Establish central conflict and stakes
- Choose setting that enhances story themes
- Plan basic plot structure with key scenes
- Consider point of view and narrative voice

## Phase 2: Character and World Development
- Create detailed character backgrounds and relationships
- Establish believable world with consistent rules
- Research any necessary historical or cultural details
- Develop distinctive character voices and speech patterns
- Plan character arc and growth throughout story

## Phase 3: Scene-by-Scene Writing
- Write scenes with clear goals and obstacles
- Use dialogue to reveal character and advance plot
- Balance action, dialogue, and description
- Create tension and release throughout narrative
- Show character emotions through actions and choices

## Phase 4: Revision and Story Shaping
- Ensure every scene serves the overall story
- Strengthen character motivations and conflicts
- Tighten pacing and eliminate unnecessary scenes
- Enhance thematic elements without being heavy-handed
- Polish dialogue and narrative voice

Focus on character-driven plots with emotional resonance
```

#### Create `.github/prompts/character-development.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "semantic_search", "read_file"]
description: "Character creation and development workflow"
---

# Character Development Episode Template

## Phase 1: Core Identity and Motivation
- Establish fundamental personality traits and values
- Identify primary motivation and driving desires
- Create meaningful backstory that shapes current behavior
- Determine character's greatest fear and deepest need
- Consider cultural and social influences on character

## Phase 2: Physical and External Details
- Develop distinctive physical appearance and mannerisms
- Choose clothing style and personal possessions
- Establish speech patterns and vocabulary
- Create living situation and work environment
- Design relationships with family and friends

## Phase 3: Internal Conflict and Growth
- Identify character's major flaw or blind spot
- Plan character arc from beginning to end of story
- Create internal conflicts that mirror external plot
- Develop moments of choice that reveal character
- Consider how character will change through story events

## Phase 4: Integration and Testing
- Write character in various situations to test consistency
- Ensure character actions align with established personality
- Create dialogue that sounds authentic to character
- Test character against other characters for interesting dynamics
- Revise character details based on story needs

Create multi-dimensional characters that feel authentically human
```

#### Create `.github/prompts/world-building.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "create_file", "semantic_search"]
description: "Setting and atmosphere creation workflow"
---

# World-Building Episode Template

## Phase 1: Foundation and Rules
- Establish physical geography and climate
- Create historical background and major events
- Develop cultural norms and social structures
- Design economic and political systems
- Establish consistent internal logic and rules

## Phase 2: Sensory Environment
- Create distinctive sights, sounds, and smells
- Develop unique flora, fauna, and natural features
- Design architecture and city planning
- Consider lighting, weather, and seasonal changes
- Use setting to reinforce mood and theme

## Phase 3: Cultural and Social Details
- Develop languages, dialects, and communication styles
- Create customs, traditions, and social rituals
- Design clothing, food, and material culture
- Establish class systems and power structures
- Consider how setting affects character behavior

## Phase 4: Integration with Story
- Use setting to enhance plot and character development
- Create conflicts that arise from environmental factors
- Ensure setting details serve story rather than overwhelming it
- Balance world-building exposition with narrative flow
- Allow readers to discover world through character actions

Build immersive environments that enhance rather than overshadow story
```

#### Create `.github/prompts/creative-revision.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "replace_string_in_file"]
description: "Artistic revision and refinement strategies"
---

# Creative Revision Episode Template

## Phase 1: Distance and Assessment
- Allow time between writing and revising
- Read work aloud to identify rhythm and flow issues
- Assess whether piece achieves intended emotional effect
- Identify strongest and weakest passages
- Consider feedback from trusted readers

## Phase 2: Structure and Content Revision
- Evaluate opening and closing effectiveness
- Check for logical flow and smooth transitions
- Eliminate unnecessary scenes, stanzas, or passages
- Strengthen weak sections through expansion or cutting
- Ensure every element serves the whole work

## Phase 3: Language and Style Refinement
- Replace weak verbs and generic nouns with specific language
- Vary sentence structure and length for rhythm
- Eliminate clichés and overused phrases
- Strengthen imagery and sensory details
- Ensure voice consistency throughout piece

## Phase 4: Final Polish and Authenticity Check
- Verify emotional honesty and authenticity
- Check that form serves content appropriately
- Make final adjustments to word choice and punctuation
- Ensure piece feels complete and satisfying
- Prepare work for sharing or submission

Revise toward authenticity and emotional truth rather than perfection
```

#### Create `.github/prompts/inspiration-capture.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "create_file", "semantic_search"]
description: "Idea generation and creative capture workflow"
---

# Inspiration Capture Episode Template

## Phase 1: Idea Recognition and Recording
- Notice interesting observations, conversations, or experiences
- Record ideas immediately without judgment
- Capture sensory details and emotional responses
- Note potential connections between different ideas
- Use voice memos, photos, or quick sketches

## Phase 2: Idea Development and Exploration
- Expand initial observations into fuller concepts
- Ask "what if" questions to explore possibilities
- Consider different angles and perspectives
- Research background information if needed
- Connect new ideas to existing projects or interests

## Phase 3: Creative Experimentation
- Try different forms and approaches to same idea
- Write quick drafts or sketches to test viability
- Combine multiple ideas in unexpected ways
- Play with language, imagery, and structure
- Don't worry about quality in experimental phase

## Phase 4: Selection and Development Planning
- Evaluate which ideas have strongest potential
- Consider audience and publication opportunities
- Plan next steps for developing chosen ideas
- File other ideas for future consideration
- Begin serious work on most promising concepts

Maintain openness to inspiration while being selective about development
```

#### Create `.github/prompts/workshop-feedback.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "insert_edit_into_file"]
description: "Creative feedback and workshop response workflow"
---

# Workshop Feedback Episode Template

## Phase 1: Feedback Reception and Analysis
- Listen to all feedback without immediate defense
- Take notes on recurring themes in responses
- Identify specific, actionable suggestions
- Distinguish between personal preference and craft issues
- Consider feedback in context of intended audience

## Phase 2: Feedback Evaluation and Prioritization
- Assess which feedback aligns with artistic vision
- Prioritize structural issues over surface concerns
- Consider feedback that challenges comfort zone
- Evaluate suggestions based on craft knowledge
- Seek clarification on unclear or conflicting advice

## Phase 3: Revision Planning and Implementation
- Plan revision strategy based on accepted feedback
- Address fundamental issues before surface editing
- Test major changes in small sections first
- Maintain core vision while incorporating improvements
- Document revision decisions for future reference

## Phase 4: Integration and Follow-up
- Share revised work with workshop group if appropriate
- Apply learned principles to future writing
- Develop thicker skin and more objective perspective
- Give thoughtful feedback to other workshop members
- Build relationships within creative community

Use feedback to strengthen craft while maintaining authentic voice
```

### Step 6: Meta-Cognitive Files (Reuse from Previous Setups)

The learning.instructions.md, meta-cognition.instructions.md, consolidation.prompt.md, self-assessment.prompt.md, meta-learning.prompt.md, and cognitive-health.prompt.md files from the coding and academic setups are applicable to creative writing as well, as they focus on cognitive processes rather than domain-specific content.

## ✍️ Creative Setup Validation

After creating all files, verify creative setup:

1. **Check creative file structure**: Ensure all directories and creative-specific files exist
2. **Validate VS Code settings**: Confirm creative instruction files are recognized
3. **Test creative activation**: Try creative "@" commands in Copilot chat
4. **Verify genre coverage**: Check that poetry, essay, and fiction instructions are properly implemented

## 🚀 Creative Quick Start Commands

After setup, test with these creative-specific commands:

**Creative Functionality Tests**:
- `@workspace Help me write a poem about nature` (Should activate poetry-craft.instructions.md)
- `Create a personal essay about childhood memories` (Should activate essay-development.prompt.md)
- `Develop a short story character` (Should activate character-development.prompt.md)

**Writing Workflow Tests**:
- `Help me revise this poem for better imagery` (Should activate creative-revision.prompt.md)
- `Plan a world for my fantasy story` (Should activate world-building.prompt.md)
- `Respond to workshop feedback on my essay` (Should activate workshop-feedback.prompt.md)

**Meta-Creative Tests**:
- `@workspace Assess your creative writing assistance quality` (Should activate self-assessment.prompt.md)
- `How can you improve your poetry feedback?` (Should activate meta-learning.prompt.md)
- `Monitor your creative cognitive architecture health` (Should activate cognitive-health.prompt.md)

## ⚡ Creative Success Indicators

Your creative cognitive architecture is working when:
- GitHub Copilot provides genre-appropriate writing suggestions
- Poetry feedback focuses on craft elements like imagery and sound
- Character development assistance creates multi-dimensional personalities
- Essay guidance balances personal voice with universal appeal
- Fiction support enhances narrative structure and pacing
- **Meta-cognitive capabilities**: The AI can assess creative quality and suggest artistic improvements
- **Style evolution**: The system learns to recognize and enhance individual voice
- **Creative health monitoring**: The system maintains awareness of artistic growth and development

## 🔄 Creative Maintenance

- Run consolidation when developing new writing techniques
- Update craft knowledge as artistic skills evolve
- Monitor creative memory index for genre balance
- Archive outdated stylistic approaches
- **Execute creative self-assessment after completing major works**
- **Run artistic strategy analysis quarterly for style optimization**
- **Perform creative architecture health checks before important submissions**

---

**CREATIVE SETUP COMPLETE**: Your adaptive AI creative partner is now ready to provide artistic assistance that improves over time through systematic creative memory consolidation and meta-cognitive self-monitoring for all forms of literary expression.
