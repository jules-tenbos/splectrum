# SPlectrum Ecosystem

## What's Where

### 📄 [`docs/`](./docs/) - **Project Documentation**
Comprehensive technical documentation covering vision, architecture, implementation guides, and references for the entire SPlectrum ecosystem.

### 🤖 [`claude/`](./claude/) - **AI Workflow Operations** 
Operational documentation and workflows for AI-assisted development, including ways of working (wow), project configuration, and task management systems.

### 📝 **This README** - **Quick Navigation & Overview**
High-level ecosystem overview with navigation to detailed documentation and operational guides.

## SPlectrum Overview

**Create tools to enable P2P networks where distributed applications run in their own peer-to-peer environment, extending blockchain's decentralization philosophy to general-purpose computing.**

The SPlectrum ecosystem transforms distributed application development through five specialized organizations working together: execution engines (SPlectrum), solution composition (Carambah), packaging & deployment (InfoMetish), AI-driven intelligence (Sesameh), and P2P runtime compatibility (bare-for-pear). Each organization addresses specific concerns while enabling seamless collaboration through unified APIs and collaborative AI workflows.

Key innovations include event-driven choreography replacing rigid orchestration, unified app/module architecture enabling complexity navigation, and collaborative AI creation where humans evolve ideas while AI handles implementation labor.

## Organization Structure & Key Repositories

The SPlectrum ecosystem is organized around five specialized organizations, each addressing specific concerns:

### 🚀 **SPlectrum** - Execution Engine & Tool Integration
Core execution environment with DSL engine, unified API architecture, and streaming capabilities. Everything that exposes SPlectrum APIs lives here.

**Key Repository:** [https://github.com/SPlectrum/spl1](https://github.com/SPlectrum/spl1) - Primary execution engine implementation

### 📦 **InfoMetish** - Packaging & Deployment  
Platform-specific packaging and deployment with container registry as authoritative source. Handles P2P packaging, container deployments, and traditional installations.

**Key Repository:** [https://github.com/InfoMetish/InfoMetis](https://github.com/InfoMetish/InfoMetis) - Container registry and deployment orchestration

### 🤖 **Sesameh** - AI-Driven Behavioral Intelligence
Collaborative AI creation enabling human-AI partnership where humans define and AI implements. Quality gates, TDD workflows, and intelligent decision-making systems.

**Key Repository:** [https://github.com/Sesameh/claude-swift](https://github.com/Sesameh/claude-swift) - Collaborative AI development workflows

### 🔧 **Carambah** - Solution Composition
High-level solution assembly from simple component setups to complex vanilla solutions. Environment-agnostic compositions using vanilla dev configs.

**Key Repository:** [https://github.com/Carambah/carambah](https://github.com/Carambah/carambah) - Solution composition engine

### ⚡ **bare-for-pear** - P2P Runtime Compatibility
JavaScript module conversions for Bare runtime (not Node.js), enabling true P2P networking capabilities through Pear platform integration.

**Status:** In development - foundational P2P networking modules

### How Organizations Work Together

```
SPlectrum (APIs & Engines) → Carambah (Compositions) → InfoMetish (Packaging) → Deployment
                    ↑                                           ↑
              Sesameh (AI Intelligence)              bare-for-pear (P2P Runtime)
```

1. **SPlectrum** provides execution foundations and API wrappers
2. **Carambah** composes these into complete solutions  
3. **InfoMetish** packages compositions for target platforms
4. **Sesameh** adds intelligence at any layer
5. **bare-for-pear** enables P2P capabilities across the ecosystem

## Documentation Overview

### 📚 **Project Documentation** ([`docs/`](./docs/))

#### [Foundation](./docs/foundation/) - Vision & Organization
- **Project Vision**: Why SPlectrum exists and core goals
- **Organization Structure**: Five specialized organizations working together
- **AI Collaboration Model**: Human-AI partnership principles

#### [Architecture](./docs/architecture/) - Technical Design
- **Core Patterns**: Unified app/module, event choreography
- **Design Principles**: Single concern, complexity navigation
- **CCAI Evolutionary Paradigm**: Seed-to-split lifecycle for organic growth

#### [Implementation](./docs/implementation/) - Building SPlectrum
- **Bootstrapping Strategies**: Getting started with development
- **Development Practices**: Quality gates and TDD workflows
- **Phase-Based Development**: Roadmap execution approach

#### [Guides](./docs/guides/) - Practical Tutorials
- **Getting Started**: Step-by-step introduction
- **Creating Applications**: Building with SPlectrum
- **Working with AI**: Effective collaboration patterns

#### [Reference](./docs/reference/) - Standards & Quick Lookups
- **Visual Style Guide**: Colors, diagrams, and branding
- **API Conventions**: Consistent interface design
- **Technical Specifications**: Detailed reference materials

## Operational Documentation Overview

### 🤖 **AI Workflow Operations** ([`claude/`](./claude/))

#### Ways of Working (`claude/wow/` → [`claude-swift`](https://github.com/Sesameh/claude-swift))
- **Workflow System**: SESSION_START, INBOX, COMMIT, VERSION_TRANSITION
- **Operational Rules**: Step-by-step execution and collaboration patterns
- **Audit Logging**: Complete trail of all operations

#### Project Configuration (`claude/project/`)
- **Version Management**: Target versions and release planning
- **Issue & Milestone Caching**: GitHub integration and tracking
- **Documentation Standards**: Writing style and AI collaboration guidelines

#### Task Management (`claude/inbox/`, `claude/outbox/`)
- **Cross-Repository Communication**: OUTBOX/INBOX workflow patterns
- **Task Processing**: Converting tasks to GitHub issues
- **Workflow Integration**: Seamless AI-assisted development

### Key Operational Workflows
- **`start sesame`**: Initialize new development sessions
- **`inbox sesame`**: Process cross-repository tasks
- **`commit sesame`**: Intelligent commits with issue closure
- **`version sesame`**: Version planning and milestone management

---

*Building the future of decentralized applications through collaborative AI and P2P networking.*