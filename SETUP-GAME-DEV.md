# Game Development Cognitive Architecture Setup Guide

**INSTRUCTIONS FOR GITHUB COPILOT**: This file contains complete setup instructions for implementing the Self-Learning Vibe Coding cognitive memory architecture optimized for game development, including Unity, Unreal Engine, indie game development, mobile gaming, and interactive entertainment.

## 🎮 Game Development Automated Setup Protocol

**Execute these steps in order to establish a complete cognitive architecture system for game development:**

### Step 1: VS Code Configuration (Required)

Add these settings to VS Code `settings.json`:

```json
{
  "github.copilot.chat.codeGeneration.useInstructionFiles": true,
  "chat.promptFiles": true,
  "chat.instructionsFilesLocations": [".github/instructions"],
  "unity.generateAll": true,
  "unity.enableAnalysis": true,
  "unity.debugCodeOptimization": false,
  "omnisharp.enableEditorConfigSupport": true,
  "omnisharp.enableImportCompletion": true,
  "omnisharp.enableRoslynAnalyzers": true,
  "typescript.suggest.autoImports": true,
  "typescript.updateImportsOnFileMove.enabled": "always",
  "javascript.suggest.autoImports": true,
  "files.associations": {
    "*.cs": "csharp",
    "*.js": "javascript",
    "*.ts": "typescript",
    "*.hlsl": "hlsl",
    "*.glsl": "glsl",
    "*.shader": "hlsl",
    "*.cginc": "hlsl",
    "*.compute": "hlsl",
    "*.uss": "css",
    "*.uxml": "xml"
  },
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "typescript": "typescriptreact"
  }
}
```

**Access settings.json**: `Ctrl+Shift+P` → "Preferences: Open User Settings (JSON)"

### Step 2: Create Game Development Directory Structure

Create this exact folder structure in the project root:

```
project-root/
├── .github/
│   ├── copilot-instructions.md          # Global Game Development Memory
│   ├── instructions/                    # Game Development Procedural Memory
│   │   ├── game-development.instructions.md
│   │   ├── unity-development.instructions.md
│   │   ├── unreal-development.instructions.md
│   │   ├── game-design.instructions.md
│   │   ├── gameplay-programming.instructions.md
│   │   ├── graphics-programming.instructions.md
│   │   ├── audio-implementation.instructions.md
│   │   ├── ui-ux-design.instructions.md
│   │   ├── mobile-gaming.instructions.md
│   │   ├── multiplayer-networking.instructions.md
│   │   ├── performance-optimization.instructions.md
│   │   ├── game-testing.instructions.md
│   │   ├── monetization.instructions.md
│   │   ├── publishing.instructions.md
│   │   ├── indie-development.instructions.md
│   │   ├── learning.instructions.md     # Meta-Cognitive Learning
│   │   └── meta-cognition.instructions.md  # Self-Monitoring
│   └── prompts/                         # Game Development Episodic Memory
│       ├── game-concept.prompt.md
│       ├── technical-design.prompt.md
│       ├── gameplay-feature.prompt.md
│       ├── level-design.prompt.md
│       ├── character-system.prompt.md
│       ├── graphics-pipeline.prompt.md
│       ├── audio-system.prompt.md
│       ├── ui-implementation.prompt.md
│       ├── multiplayer-feature.prompt.md
│       ├── performance-profiling.prompt.md
│       ├── game-balancing.prompt.md
│       ├── monetization-strategy.prompt.md
│       ├── marketing-launch.prompt.md
│       ├── post-launch.prompt.md
│       ├── consolidation.prompt.md
│       ├── self-assessment.prompt.md    # Meta-Cognitive Assessment
│       ├── meta-learning.prompt.md      # Learning Strategy Evolution
│       └── cognitive-health.prompt.md   # Architecture Maintenance
├── assets/
│   ├── art/                            # 2D/3D art assets
│   │   ├── textures/
│   │   ├── models/
│   │   ├── animations/
│   │   ├── sprites/
│   │   └── ui/
│   ├── audio/                          # Sound effects and music
│   │   ├── sfx/
│   │   ├── music/
│   │   ├── voice/
│   │   └── ambient/
│   ├── fonts/                          # Typography assets
│   ├── shaders/                        # Custom shaders
│   └── data/                           # Game data files
├── scripts/
│   ├── core/                           # Core game systems
│   ├── gameplay/                       # Gameplay mechanics
│   ├── ui/                             # User interface
│   ├── audio/                          # Audio systems
│   ├── graphics/                       # Graphics and rendering
│   ├── networking/                     # Multiplayer networking
│   ├── utilities/                      # Helper scripts
│   └── tools/                          # Editor tools
├── scenes/                             # Game scenes/levels
│   ├── main-menu/
│   ├── gameplay/
│   ├── cutscenes/
│   └── ui-screens/
├── prefabs/                            # Reusable game objects
│   ├── characters/
│   ├── environment/
│   ├── ui/
│   └── effects/
├── tests/
│   ├── unit/                           # Unit tests
│   ├── integration/                    # Integration tests
│   ├── performance/                    # Performance tests
│   └── playtest/                       # Playtesting data
├── builds/                             # Game builds
│   ├── development/
│   ├── testing/
│   ├── release/
│   └── platforms/
├── docs/
│   ├── game-design/                    # Game design documents
│   ├── technical/                      # Technical documentation
│   ├── art-style/                      # Art style guides
│   ├── audio-design/                   # Audio design documents
│   └── marketing/                      # Marketing materials
└── tools/
    ├── build-scripts/                  # Build automation
    ├── asset-pipeline/                 # Asset processing tools
    ├── analytics/                      # Game analytics tools
    └── localization/                   # Localization tools
```

### Step 3: Global Game Development Declarative Memory Setup

**Create `.github/copilot-instructions.md`** with this exact content:

```markdown
# Self-Learning Vibe Coding - Game Development Cognitive Architecture

IMPORTANT: This file serves as Global Game Development Declarative Memory. Optimized for Unity, Unreal Engine, indie game development, mobile gaming, and interactive entertainment creation.

## 🧠 Game Development Cognitive Architecture Status

**Working Memory**: 4/4 rules (at optimal capacity for game development)
**Consolidation**: Auto-trigger when exceeding capacity
**Memory Distribution**: Active across game development procedural (.instructions.md) and game creation episodic (.prompt.md) systems

## 🎮 Game Development Working Memory - Quick Reference (Limit: 4 Critical Rules)

| Priority | Rule | Load | Auto-Consolidate |
|----------|------|------|------------------|
| P1 | `@player-first` - Design all systems prioritizing player experience, engagement, and fun factor | Low | Never |
| P2 | `@performance-critical` - Optimize for target platform constraints and maintain stable frame rates | Medium | >30 days unused |
| P3 | `@meditation` - Auto-consolidate when working memory capacity exceeded | High | When triggered |
| P4 | `@iterative-design` - Use rapid prototyping, playtesting, and data-driven iteration cycles | Medium | When obsolete |

## 🎯 Game Development Cognitive Architecture Coordination

### Game Development Procedural Memory Activation (Context-Dependent):
- `game-development.instructions.md` → General game dev for .cs, .js, .ts, .cpp, game files
- `unity-development.instructions.md` → Unity development for .cs, .unity, Unity project files  
- `unreal-development.instructions.md` → Unreal development for .cpp, .h, .uasset, UE project files
- `game-design.instructions.md` → Game design for *design*, *mechanics*, *balance* files
- `gameplay-programming.instructions.md` → Gameplay for *gameplay*, *mechanics*, *systems* files
- `graphics-programming.instructions.md` → Graphics for *shader*, *rendering*, *graphics* files
- `audio-implementation.instructions.md` → Audio for *audio*, *sound*, *music* files
- `ui-ux-design.instructions.md` → UI/UX for *ui*, *ux*, *interface*, *menu* files
- `mobile-gaming.instructions.md` → Mobile for *mobile*, *touch*, *android*, *ios* files
- `multiplayer-networking.instructions.md` → Multiplayer for *multiplayer*, *network*, *online* files
- `performance-optimization.instructions.md` → Performance for *optimization*, *profiling*, *performance* files
- `game-testing.instructions.md` → Testing for *test*, *qa*, *playtest* files
- `monetization.instructions.md` → Monetization for *monetization*, *iap*, *ads* files
- `publishing.instructions.md` → Publishing for *publish*, *store*, *distribution* files
- `indie-development.instructions.md` → Indie for *indie*, *solo*, *small-team* files
- `learning.instructions.md` → Meta-cognitive learning for *instructions*, *learning* files
- `meta-cognition.instructions.md` → Self-awareness for *meta*, *monitor*, *assess* files

### Game Development Episodic Memory Activation (Game Creation Workflows):
- `game-concept.prompt.md` → Game concept development and ideation
- `technical-design.prompt.md` → Technical architecture and system design
- `gameplay-feature.prompt.md` → Gameplay feature implementation workflows
- `level-design.prompt.md` → Level and environment design processes
- `character-system.prompt.md` → Character creation and animation systems
- `graphics-pipeline.prompt.md` → Graphics rendering and visual effects
- `audio-system.prompt.md` → Audio implementation and sound design
- `ui-implementation.prompt.md` → User interface and user experience design
- `multiplayer-feature.prompt.md` → Multiplayer and networking implementation
- `performance-profiling.prompt.md` → Performance optimization and profiling
- `game-balancing.prompt.md` → Game balance and difficulty tuning
- `monetization-strategy.prompt.md` → Monetization and business model implementation
- `marketing-launch.prompt.md` → Marketing and launch strategy execution
- `post-launch.prompt.md` → Post-launch support and content updates
- `consolidation.prompt.md` → Game development memory optimization
- `self-assessment.prompt.md` → Game development performance evaluation
- `meta-learning.prompt.md` → Game development strategy evolution
- `cognitive-health.prompt.md` → Game development architecture maintenance

### Game Development Auto-Consolidation Triggers

- Working memory > 4 rules → Execute consolidation.prompt.md
- Engine conflicts detected → Activate appropriate engine-specific instructions
- Performance degradation → Review and redistribute game development memory load
- User requests meditation → Full game development cognitive architecture optimization
- **Game development performance assessment needed → Execute self-assessment.prompt.md**
- **Game development strategy evolution required → Execute meta-learning.prompt.md**
- **Game development architecture health check → Execute cognitive-health.prompt.md**

## 🔄 Game Development Memory Transfer Protocol

**Immediate Transfer**: Critical gameplay errors → Quick Reference (P1-P4)
**Gradual Consolidation**: Repeated development patterns → Game development procedural memory (.instructions.md)
**Complex Game Workflows**: Multi-system features → Game creation episodic memory (.prompt.md)
**Archive Management**: Obsolete game development patterns → Historical storage in specialized files
**Index Maintenance**: Auto-update Game Development Long-Term Memory Index during transfers

## 📚 Game Development Long-Term Memory Index

### Game Development Procedural Memory Store (.github/instructions/)
| File | Domain | Activation Pattern | Last Updated |
|------|--------|-------------------|--------------|
| game-development.instructions.md | General Game Dev | *.cs, *.js, *.ts, *.cpp, game* | Auto-tracked |
| unity-development.instructions.md | Unity Development | *.cs, *.unity, Unity projects | Auto-tracked |
| unreal-development.instructions.md | Unreal Development | *.cpp, *.h, *.uasset, UE projects | Auto-tracked |
| game-design.instructions.md | Game Design | *design*, *mechanics*, *balance* | Auto-tracked |
| gameplay-programming.instructions.md | Gameplay Programming | *gameplay*, *mechanics*, *systems* | Auto-tracked |
| graphics-programming.instructions.md | Graphics Programming | *shader*, *rendering*, *graphics* | Auto-tracked |
| audio-implementation.instructions.md | Audio Implementation | *audio*, *sound*, *music* | Auto-tracked |
| ui-ux-design.instructions.md | UI/UX Design | *ui*, *ux*, *interface*, *menu* | Auto-tracked |
| mobile-gaming.instructions.md | Mobile Gaming | *mobile*, *touch*, *android*, *ios* | Auto-tracked |
| multiplayer-networking.instructions.md | Multiplayer Networking | *multiplayer*, *network*, *online* | Auto-tracked |
| performance-optimization.instructions.md | Performance Optimization | *optimization*, *profiling*, *performance* | Auto-tracked |
| game-testing.instructions.md | Game Testing | *test*, *qa*, *playtest* | Auto-tracked |
| monetization.instructions.md | Monetization | *monetization*, *iap*, *ads* | Auto-tracked |
| publishing.instructions.md | Publishing | *publish*, *store*, *distribution* | Auto-tracked |
| indie-development.instructions.md | Indie Development | *indie*, *solo*, *small-team* | Auto-tracked |
| learning.instructions.md | Meta-Learning | *instructions*, *learning* | Auto-tracked |
| meta-cognition.instructions.md | Self-Monitoring | *meta*, *monitor*, *assess* | Auto-tracked |

### Game Development Episodic Memory Store (.github/prompts/)
| File | Game Development Workflow | Complexity Level | Usage Frequency |
|------|---------------------------|------------------|-----------------|
| game-concept.prompt.md | Game Concept Development | High | Auto-tracked |
| technical-design.prompt.md | Technical Architecture | High | Auto-tracked |
| gameplay-feature.prompt.md | Gameplay Implementation | Medium | Auto-tracked |
| level-design.prompt.md | Level Design | Medium | Auto-tracked |
| character-system.prompt.md | Character Systems | Medium | Auto-tracked |
| graphics-pipeline.prompt.md | Graphics Pipeline | High | Auto-tracked |
| audio-system.prompt.md | Audio Implementation | Medium | Auto-tracked |
| ui-implementation.prompt.md | UI Implementation | Medium | Auto-tracked |
| multiplayer-feature.prompt.md | Multiplayer Features | High | Auto-tracked |
| performance-profiling.prompt.md | Performance Optimization | High | Auto-tracked |
| game-balancing.prompt.md | Game Balancing | Medium | Auto-tracked |
| monetization-strategy.prompt.md | Monetization Strategy | Medium | Auto-tracked |
| marketing-launch.prompt.md | Marketing and Launch | Medium | Auto-tracked |
| post-launch.prompt.md | Post-Launch Support | Medium | Auto-tracked |
| consolidation.prompt.md | Memory Optimization | High | Auto-tracked |
| self-assessment.prompt.md | Performance Evaluation | High | Auto-tracked |
| meta-learning.prompt.md | Strategy Evolution | High | Auto-tracked |
| cognitive-health.prompt.md | Health Monitoring | Medium | Auto-tracked |

### Game Development Memory Transfer Protocol Status
- **Active Files**: 35 specialized game development memory files (17 procedural + 18 episodic)
- **Last Consolidation**: Game development architecture initialization with meta-cognitive enhancements
- **Cognitive Load Status**: Optimized for multi-platform game development and player experience
- **Index Synchronization**: Maintained automatically during consolidation
- **Meta-Cognitive Status**: Fully operational with game development performance assessment and strategy evolution

---

*Global Game Development Declarative Memory Component - Coordinates distributed game development cognitive architecture while maintaining optimal game creation efficiency. Detailed game development protocols reside in specialized memory files.*
```

### Step 4: Game Development Procedural Memory Files

#### Create `.github/instructions/game-development.instructions.md`:

```markdown
---
applyTo: "**/*.cs,**/*.js,**/*.ts,**/*.cpp,**/game/**,**/games/**"
description: "General game development standards and interactive entertainment best practices"
---

# Game Development Procedural Memory

## Player-Centric Design Principles
- Prioritize player experience and engagement in all design decisions
- Design intuitive controls and responsive gameplay mechanics
- Implement clear feedback systems for player actions and game state
- Create engaging progression systems and meaningful player choices
- Consider accessibility and inclusive design for diverse players

## Game Architecture Standards
- Use component-based entity systems for flexible game object design
- Implement clean separation between game logic, presentation, and data
- Design scalable systems that can handle varying game complexity
- Use design patterns appropriate for real-time interactive systems
- Plan for modular architecture supporting iterative development

## Performance and Optimization
- Target consistent frame rates for smooth gameplay experience
- Implement efficient memory management and object pooling
- Optimize critical gameplay loops and frequent operations
- Use profiling tools to identify and resolve performance bottlenecks
- Design with target platform constraints and limitations in mind

## Game Development Workflow
- Use version control with appropriate branching strategies for game teams
- Implement automated build systems for multiple platforms
- Create comprehensive testing procedures including playtesting
- Document game systems and maintain design documentation
- Use iterative development with regular milestone reviews

## Cross-Platform Considerations
- Design for multiple input methods (keyboard, mouse, touch, gamepad)
- Consider different screen sizes and aspect ratios
- Plan for platform-specific features and limitations
- Implement appropriate save/load systems for target platforms
- Test on actual hardware throughout development process
```

#### Create `.github/instructions/unity-development.instructions.md`:

```markdown
---
applyTo: "**/*.cs,**/*.unity,**/Unity/**,**/Assets/**"
description: "Unity Engine development standards and C# scripting best practices"
---

# Unity Development Procedural Memory

## Unity Project Organization
- Use consistent folder structure for Assets organization
- Implement proper naming conventions for scenes, prefabs, and scripts
- Organize scripts using namespaces and assembly definitions
- Use prefabs effectively for reusable game objects and UI elements
- Maintain clean scene hierarchies with logical object grouping

## C# Scripting Best Practices
- Follow Unity's component-based architecture patterns
- Use MonoBehaviour lifecycle methods appropriately (Start, Update, FixedUpdate)
- Implement proper null checking and error handling
- Use Unity's serialization system effectively with [SerializeField]
- Avoid expensive operations in Update loops

## Unity-Specific Performance Optimization
- Use object pooling for frequently instantiated objects
- Optimize rendering with batching and culling strategies
- Implement efficient collision detection and physics usage
- Use Unity Profiler to identify performance bottlenecks
- Optimize texture compression and asset import settings

## Unity Tools and Systems Integration
- Use Unity's built-in systems (Animation, Audio, UI, Physics)
- Implement custom editor tools for improved workflow
- Use ScriptableObjects for data-driven design
- Integrate with Unity Services (Analytics, Cloud Build, IAP)
- Leverage Unity Package Manager for third-party integrations

## Unity Deployment and Build Management
- Configure build settings for target platforms
- Implement proper platform-specific code using preprocessor directives
- Use Unity's addressables system for asset management
- Configure player settings and quality settings appropriately
- Test builds on target devices throughout development
```

#### Create `.github/instructions/unreal-development.instructions.md`:

```markdown
---
applyTo: "**/*.cpp,**/*.h,**/*.uasset,**/Unreal/**,**/UE/**"
description: "Unreal Engine development standards and C++ programming best practices"
---

# Unreal Development Procedural Memory

## Unreal Engine Architecture
- Use Unreal's Actor-Component system effectively
- Implement proper inheritance hierarchies with UObject base classes
- Use Blueprint and C++ integration appropriately
- Follow Unreal's reflection system conventions with UCLASS, UPROPERTY macros
- Implement proper garbage collection patterns with Unreal's memory management

## C++ Programming in Unreal
- Follow Unreal coding standards and naming conventions
- Use Unreal's container classes (TArray, TMap, FString) instead of STL
- Implement proper header file organization with forward declarations
- Use Unreal's delegate and event systems for decoupled communication
- Handle asynchronous operations with Unreal's async task system

## Blueprint and Visual Scripting
- Use Blueprints for rapid prototyping and designer-friendly systems
- Implement performance-critical code in C++ with Blueprint exposure
- Create custom Blueprint nodes for frequently used functionality
- Use Blueprint interfaces for polymorphic behavior
- Organize Blueprint assets with proper naming and folder structure

## Unreal Performance Optimization
- Use Unreal's built-in profiling tools (Stat commands, Insights)
- Optimize rendering with LOD systems and culling
- Implement efficient asset streaming and memory management
- Use Unreal's threading and task systems for parallel processing
- Optimize Blueprint execution with nativization where appropriate

## Unreal Engine Tools and Workflow
- Use Unreal's editor tools effectively (Level Editor, Material Editor, Animation Tools)
- Implement custom editor utilities and tools for team workflow
- Use Unreal's source control integration (Perforce, Git)
- Configure packaging and deployment for target platforms
- Leverage Unreal's marketplace and community resources
```

#### Create `.github/instructions/game-design.instructions.md`:

```markdown
---
applyTo: "**/*design*,**/*mechanics*,**/*balance*,**/*gameplay*"
description: "Game design methodology and interactive system design principles"
---

# Game Design Procedural Memory

## Core Game Design Principles
- Define clear design pillars and maintain consistency throughout development
- Create meaningful player choices with interesting consequences
- Design feedback loops that reinforce core gameplay mechanics
- Balance challenge and accessibility for target audience
- Implement progression systems that maintain player engagement

## Game Mechanics Design
- Design mechanics that support the core game experience
- Create emergent gameplay through simple, interacting systems
- Use prototyping to validate mechanics before full implementation
- Design for player agency and meaningful decision-making
- Consider pacing and rhythm in gameplay experience

## Game Balance and Tuning
- Use data-driven approaches to balance game systems
- Implement configurable parameters for easy tuning
- Create systematic approaches to difficulty progression
- Test balance with diverse player groups and skill levels
- Plan for post-launch balance adjustments and updates

## Player Psychology and Motivation
- Apply motivation theories (intrinsic vs extrinsic motivation)
- Design reward systems that maintain long-term engagement
- Consider player flow states and optimal challenge levels
- Implement social features that enhance player connection
- Design onboarding that teaches core mechanics effectively

## Systematic Design Documentation
- Create and maintain comprehensive game design documents
- Use iterative design processes with regular review cycles
- Document design decisions and rationale for future reference
- Collaborate effectively with development team members
- Plan for localization and cultural adaptation considerations
```

#### Create `.github/instructions/gameplay-programming.instructions.md`:

```markdown
---
applyTo: "**/*gameplay*,**/*mechanics*,**/*systems*,**/*logic*"
description: "Gameplay programming patterns and interactive system implementation"
---

# Gameplay Programming Procedural Memory

## Gameplay System Architecture
- Design modular gameplay systems with clear interfaces
- Implement event-driven communication between game systems
- Use state machines for complex gameplay state management
- Create data-driven systems that support designer iteration
- Design for networked multiplayer from the beginning when applicable

## Player Controller and Input Systems
- Implement responsive and customizable input handling
- Design input buffering and prediction for improved feel
- Create accessibility options for diverse player needs
- Handle multiple input devices and platform differences
- Implement proper input validation and security measures

## Game State Management
- Design clear game state hierarchies and transitions
- Implement save/load systems with forward compatibility
- Handle pause, menu, and overlay states appropriately
- Create robust error handling and recovery systems
- Plan for development tools and debug interfaces

## Gameplay Mechanics Implementation
- Create reusable components for common gameplay elements
- Implement timing-sensitive mechanics with frame-rate independence
- Design flexible animation integration with gameplay systems
- Create efficient collision detection and response systems
- Implement proper physics integration for gameplay needs

## Performance-Critical Gameplay Code
- Optimize frequently called gameplay code paths
- Use object pooling for runtime-created gameplay objects
- Implement efficient data structures for spatial queries
- Cache expensive calculations and update only when necessary
- Profile gameplay systems under realistic load conditions
```

#### Create `.github/instructions/graphics-programming.instructions.md`:

```markdown
---
applyTo: "**/*shader*,**/*rendering*,**/*graphics*,**/*visual*"
description: "Graphics programming and visual effects implementation standards"
---

# Graphics Programming Procedural Memory

## Rendering Pipeline Architecture
- Understand target platform rendering capabilities and limitations
- Design flexible shader systems that support art direction needs
- Implement efficient draw call batching and state management
- Use appropriate rendering techniques for target performance levels
- Plan for scalable graphics options and quality settings

## Shader Development Standards
- Write maintainable shaders with clear documentation and organization
- Use consistent naming conventions and coding standards
- Implement proper error handling and fallback shaders
- Optimize shaders for target hardware constraints
- Use preprocessor directives for platform-specific optimizations

## Lighting and Shading Systems
- Implement lighting models appropriate for art style and performance targets
- Design flexible material systems that support artistic workflows
- Use efficient shadow mapping and lighting techniques
- Consider global illumination approaches for visual quality
- Optimize lighting calculations for real-time performance

## Visual Effects and Post-Processing
- Create modular visual effects systems that artists can easily use
- Implement efficient particle systems with GPU acceleration where appropriate
- Design post-processing pipelines that enhance visual quality without compromising performance
- Use temporal techniques for improved visual quality and performance
- Consider VR/AR specific rendering requirements when applicable

## Graphics Performance Optimization
- Use GPU profiling tools to identify rendering bottlenecks
- Implement level-of-detail (LOD) systems for geometry and shaders
- Optimize texture usage, compression, and streaming
- Use occlusion culling and frustum culling effectively
- Balance visual quality with performance targets for each platform
```

#### Create `.github/instructions/mobile-gaming.instructions.md`:

```markdown
---
applyTo: "**/*mobile*,**/*touch*,**/*android*,**/*ios*"
description: "Mobile game development standards and touch interface design"
---

# Mobile Gaming Procedural Memory

## Mobile-First Design Principles
- Design for touch input with appropriate touch target sizes
- Consider one-handed gameplay and thumb-reach zones
- Implement intuitive gesture controls and multi-touch support
- Design for portrait and landscape orientations as appropriate
- Plan for interruptions (calls, notifications, app switching)

## Mobile Performance Optimization
- Target 60fps on mid-range devices for smooth gameplay
- Implement aggressive LOD and culling systems for mobile GPUs
- Optimize texture memory usage and compression for mobile
- Use efficient audio compression and streaming for mobile storage
- Implement dynamic quality scaling based on device performance

## Mobile Platform Integration
- Integrate with platform-specific features (Game Center, Google Play Games)
- Implement proper save cloud synchronization across devices
- Use platform advertising and analytics SDKs appropriately
- Handle platform-specific input methods (accelerometer, gyroscope)
- Implement proper app lifecycle management for mobile platforms

## Mobile Monetization Strategies
- Design ethical and engaging in-app purchase systems
- Implement rewarded video ads that enhance gameplay
- Create fair free-to-play economies with meaningful progression
- Use analytics to optimize monetization without compromising player experience
- Consider regional differences in monetization preferences

## Mobile User Experience Design
- Design clear and readable UI for small screens
- Implement progressive disclosure for complex game systems
- Create effective onboarding for mobile-first audiences
- Use haptic feedback appropriately for enhanced tactile experience
- Design for offline gameplay when network connectivity is limited
```

### Step 5: Game Development Episodic Memory Files

#### Create `.github/prompts/game-concept.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Game concept development and creative ideation workflow"
---

# Game Concept Development Episode Template

## Phase 1: Creative Ideation and Core Concept
- Define the core game experience and primary emotions to evoke
- Identify target audience and market positioning
- Establish unique selling points and differentiation from existing games
- Create initial gameplay prototypes to validate core mechanics
- Define art style direction and aesthetic goals

## Phase 2: Game Design Framework
- Develop core game pillars that guide all design decisions
- Design primary gameplay loops and progression systems
- Plan narrative structure and thematic elements
- Establish technical requirements and platform considerations
- Create initial scope estimates and development timeline

## Phase 3: Market and Feasibility Analysis
- Research competitive landscape and market opportunities
- Analyze technical feasibility with available resources and timeline
- Assess team capabilities and skill requirements
- Evaluate monetization strategies and business model options
- Identify potential risks and mitigation strategies

## Phase 4: Concept Documentation and Validation
- Create comprehensive game design document outlining core systems
- Develop visual mockups and interactive prototypes
- Conduct initial playtesting with target audience representatives
- Gather stakeholder feedback and iterate on core concept
- Establish development roadmap and milestone planning

Focus on innovative gameplay and clear vision communication
```

#### Create `.github/prompts/gameplay-feature.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "create_file", "read_file"]
description: "Gameplay feature implementation and system integration workflow"
---

# Gameplay Feature Development Episode Template

## Phase 1: Feature Design and Requirements
- Define feature goals and how they support core game experience
- Create detailed feature specifications and edge case considerations
- Design user interface and user experience for the feature
- Plan integration with existing game systems and architecture
- Establish success metrics and testing criteria

## Phase 2: Technical Implementation Planning
- Design technical architecture and data structures for the feature
- Plan code organization and module dependencies
- Identify reusable components and systems integration points
- Consider performance implications and optimization strategies
- Plan for configuration, debugging, and testing infrastructure

## Phase 3: Development and Integration
- Implement core feature functionality using iterative development
- Create appropriate user interface and visual feedback systems
- Integrate with existing gameplay systems and ensure compatibility
- Implement comprehensive testing including edge cases and error conditions
- Create configuration tools for designers to tune feature parameters

## Phase 4: Polish and Optimization
- Conduct thorough playtesting to validate feature design goals
- Optimize feature performance and memory usage
- Polish visual and audio feedback for enhanced player experience
- Document feature implementation and usage guidelines
- Plan for potential future iterations and improvements

Focus on player experience and seamless system integration
```

#### Create `.github/prompts/performance-profiling.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Game performance profiling and optimization workflow"
---

# Performance Profiling Episode Template

## Phase 1: Performance Analysis and Baseline Establishment
- Use platform-specific profiling tools to identify performance bottlenecks
- Establish baseline performance metrics for target platforms
- Analyze frame time breakdown (CPU vs GPU bound operations)
- Identify memory usage patterns and potential memory leaks
- Profile typical gameplay scenarios and worst-case conditions

## Phase 2: Optimization Strategy and Prioritization
- Prioritize optimization efforts based on impact and implementation cost
- Plan rendering optimizations (draw calls, batching, culling)
- Design memory optimization strategies (pooling, streaming, compression)
- Plan gameplay system optimizations for frequently executed code
- Consider platform-specific optimization opportunities

## Phase 3: Implementation and Testing
- Implement targeted optimizations systematically
- Use A/B testing to validate optimization effectiveness
- Test optimizations across different devices and scenarios
- Monitor for regressions and unintended side effects
- Document optimization techniques and performance gains

## Phase 4: Continuous Monitoring and Maintenance
- Establish automated performance monitoring and regression detection
- Create performance budgets and guidelines for ongoing development
- Plan regular performance review cycles throughout development
- Document performance best practices for team knowledge sharing
- Prepare for platform-specific performance requirements and certification

Focus on measurable improvements and sustainable performance practices
```

#### Create `.github/prompts/monetization-strategy.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Game monetization and business model implementation workflow"
---

# Monetization Strategy Episode Template

## Phase 1: Business Model Design and Analysis
- Define monetization model aligned with game design and target audience
- Research market standards and competitor monetization strategies
- Design ethical monetization that enhances rather than detracts from gameplay
- Plan pricing strategies and virtual economy design
- Consider regional differences and payment method preferences

## Phase 2: Implementation Planning and Integration
- Design in-app purchase systems and virtual currency architecture
- Plan advertising integration that respects player experience
- Implement analytics and tracking for monetization optimization
- Design user interface and user experience for purchase flows
- Plan A/B testing framework for monetization optimization

## Phase 3: Technical Implementation and Testing
- Implement secure payment processing and receipt validation
- Create robust virtual economy with proper security measures
- Integrate advertising SDKs with appropriate frequency and placement
- Implement analytics tracking for revenue and player behavior
- Test monetization systems across different platforms and regions

## Phase 4: Launch and Optimization
- Monitor monetization performance and player sentiment
- Analyze player behavior data to optimize monetization strategies
- Conduct regular A/B tests on pricing, offers, and placement
- Respond to player feedback and adjust strategies accordingly
- Plan for long-term monetization sustainability and player lifetime value

Focus on ethical monetization that enhances player experience
```

#### Create `.github/prompts/marketing-launch.prompt.md`:

```markdown
---
mode: "agent"
model: "gpt-4"
tools: ["workspace", "read_file", "semantic_search"]
description: "Game marketing and launch strategy execution workflow"
---

# Marketing and Launch Episode Template

## Phase 1: Marketing Strategy and Brand Development
- Define target audience segments and marketing personas
- Develop unique value proposition and key marketing messages
- Create brand identity and visual marketing assets
- Plan marketing channels and campaign strategies
- Establish marketing budget allocation and ROI targets

## Phase 2: Pre-Launch Marketing and Community Building
- Create marketing materials (trailers, screenshots, press kits)
- Build social media presence and community engagement
- Implement influencer outreach and press relations strategies
- Participate in relevant gaming events and showcases
- Develop partnerships with platform holders and distribution partners

## Phase 3: Launch Execution and Promotion
- Coordinate platform store optimization and featuring opportunities
- Execute multi-channel marketing campaigns with coordinated messaging
- Monitor and respond to press coverage and community feedback
- Implement user acquisition campaigns with performance tracking
- Manage crisis communication and negative feedback appropriately

## Phase 4: Post-Launch Marketing and Retention
- Analyze launch performance data and user acquisition metrics
- Implement retention marketing campaigns for existing players
- Plan content marketing strategy for ongoing engagement
- Monitor competitive landscape and adjust marketing positioning
- Develop long-term marketing strategy for sustained growth

Focus on authentic community building and sustainable growth
```

### Step 6: Meta-Cognitive Files Integration

The learning.instructions.md, meta-cognition.instructions.md, consolidation.prompt.md, self-assessment.prompt.md, meta-learning.prompt.md, and cognitive-health.prompt.md files from previous setups apply to game development as well, focusing on continuous improvement of game development capabilities.

## 🎮 Game Development Setup Validation

After creating all files, verify game development setup:

1. **Check game development file structure**: Ensure all directories and game-specific files exist
2. **Validate VS Code settings**: Confirm game development instruction files are recognized
3. **Test game development activation**: Try game development "@" commands in Copilot chat
4. **Verify engine integration**: Check that methodology properly supports Unity, Unreal, and other engines

## 🚀 Game Development Quick Start Commands

After setup, test with these game development-specific commands:

**Game Development Tests**:
- `@workspace Help me create a Unity game architecture` (Should activate technical-design.prompt.md)
- `Design a player controller system` (Should activate gameplay-feature.prompt.md)
- `Optimize game performance for mobile` (Should activate performance-profiling.prompt.md)

**Engine-Specific Tests**:
- `Implement Unity MonoBehaviour patterns` (Should activate unity-development.instructions.md)
- `Create Unreal Engine C++ gameplay class` (Should activate unreal-development.instructions.md)
- `Design mobile touch controls` (Should activate mobile-gaming.instructions.md)

**Meta-Game Development Tests**:
- `@workspace Assess your game development assistance quality` (Should activate self-assessment.prompt.md)
- `How can you improve gameplay programming support?` (Should activate meta-learning.prompt.md)
- `Monitor your game development architecture health` (Should activate cognitive-health.prompt.md)

## ⚡ Game Development Success Indicators

Your game development cognitive architecture is working when:
- Games prioritize player experience and engagement in all design decisions
- Code follows engine-specific best practices while maintaining cross-platform compatibility
- Performance optimizations maintain stable frame rates on target platforms
- Monetization strategies enhance rather than detract from gameplay experience
- Development workflow supports iterative design and rapid prototyping
- **Meta-cognitive capabilities**: The AI can assess game development quality and suggest improvements
- **Player experience optimization**: The system improves game design recommendations over time
- **Game development health monitoring**: The system maintains awareness of industry trends and platform updates

## 🔄 Game Development Maintenance

- Run consolidation when adding new game engines or platforms
- Update platform-specific knowledge regularly with engine updates and new hardware
- Monitor game development memory index for currency with industry trends and best practices
- Archive outdated game development patterns and deprecated APIs
- **Execute game development self-assessment after major milestone releases**
- **Run player experience analysis quarterly for gameplay optimization**
- **Perform game development architecture health checks before platform submissions**

---

**GAME DEVELOPMENT SETUP COMPLETE**: Your adaptive AI game development partner is now ready to provide comprehensive game development assistance across Unity, Unreal Engine, mobile platforms, and indie development with continuous improvement through systematic memory consolidation and meta-cognitive self-monitoring.
