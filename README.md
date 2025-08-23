# SPlectrum in a Nutshell

**SPlectrum is an application development platform designed to make creating applications accessible through natural human-AI collaboration, built on a foundation of open architecture, well-documented APIs, and comprehensive quality frameworks.**

This overview is structured in four parts: the foundations, the platform logical components, the application focus domains, and the ecosystem organization. For detailed implementation status, see [Functional Components](./docs/implementation/functional-components.md).

## SPlectrum Foundational Components

The foundational layer provides the core infrastructure that enables the **strict boundaries, internal freedom** design philosophy throughout the platform. These components create the technical foundations for boundary enforcement (AVRO schemas, validation) and internal flexibility (JavaScript dynamic typing, JIT adaptability, streaming patterns).

*Core infrastructure layers that other components depend on*

| Area | Component | Current Status | Comments |
|------|-----------|----------------|----------|
| **JavaScript** | Node.js | ✅ Exists | Server-side JavaScript with JIT compilation and event loop concurrency |
| | Browser JS | ✅ Exists | Client-side JavaScript enabling unified development across contexts |
| | JIT Adaptability | ✅ Exists | Dynamic API generation and runtime modification capabilities |
| | Data Interoperability | ✅ Exists | Natural JS Object ↔ JSON ↔ AVRO transformation |
| **UI Components** | Terminal UI | ❌ Missing | CLI-based management interface |
| | Browser UI | ❌ Missing | React/AVRO integration for web interface |
| | Mobile/PWA | ❌ Missing | Progressive Web App capabilities |
| **AVRO Schema and RPC** | Schema Definition | 🔧 Partial | Currently implemented with command-line-args |
| | Validation | ❌ Missing | Input/output validation across platform |
| | Documentation | 🔧 Partial | Auto-generated docs from schemas, currently implemented with command-line-args |
| | RPC | ❌ Missing | AVRO RPC setup for cross-service communication |
| **Streaming Native** | Kafka Compatible Data Record | ✅ Exists | Shared internal streaming data structure |
| | Data Change Streaming | 🔧 Partial | Consume / publish immutable data change records |
| **Functional Execution** | Execution Pipeline Record | ✅ Exists | Step to step functional, procedural step internal |
| | Stateless Execution Engine | ✅ Exists | Execution requires no persistent state |
| **Peer to Peer** | Bare Runtime | ❌ Missing | Minimal runtime, ideal for P2P applications |
| | Pear Stack | ❌ Missing | Bare based P2P runtime with true P2P capabilities |

## SPlectrum Platform Logical Components

*Design approaches and methodologies that shape how the platform is built*

The platform applies a **strict boundaries, internal freedom** design philosophy enabled by the foundational architecture. **Strict boundaries** (AVRO validation, TDD contracts, schema enforcement) create **safe internal environments** with minimal constraints. Using this pattern single concern APIs are created that scale from **core APIs** at the fundamental level to **higher-level context APIs** while maintaining the same principle - each component has well-defined boundaries coupled with implementation freedom within those boundaries. This **DSL engine freedom of expression** approach is seen as an important stepping stone to meaningful AI autonomy.

| Area | Component | Current Status | Comments |
|-----------------|-----------|----------------|----------|
| **API First-Class Citizen** | Item Help | ✅ Exists | Current help system operational, needs AVRO schema integration |
| | API Discovery | ❌ Missing | Global `-h` flag with modules/apps list, API browsing capabilities |
| | Advanced API Management | 🗺️ Roadmap | API search, API registry, API versioning |
| **API Expression Contexts** | Scripting | ✅ Exists | Current implementation functional |
| | Continuation Syntax | 🗺️ Roadmap | Language design for fluent workflow composition |
| **TDC (Test Driven Creation)** | TDD Implementation | ✅ Exists | Uses functional execution audit for testing |
| | Continuous Improvement | 🗺️ Roadmap | Defect handling within expectation framework |
| | Test Driven Creation | 🗺️ Roadmap | Natural language, DSL engine, API creation |
| **Collaborative AI** | Human-AI Creative Partnership | ✅ Exists | Shared context, human-in-the-loop design principles |
| | Shared Ways of Working | ✅ Exists | Shared workflows and issue type defined workflows |
| | Strict Workflow Creation | ✅ Exists | Workflows transferable to event driven choreography |
| **Event Driven Choreography** | Strict Workflow Execution | 🗺️ Roadmap | Automated execution of defined workflow patterns **(deterministic, no AI required)** |
| | AI Issue Resolution | 🗺️ Roadmap | Autonomous issue handling and resolution **(AI within strict test/validation boundaries)** |
| **AI Autonomy** | Self-Directed Operation | 🗺️ Roadmap | Independent decision-making within validated boundaries **(creative problem definition and solution)** |
| | Autonomous Validation | 🗺️ Roadmap | Self-checking and quality assurance capabilities **(self-defined success criteria)** |
| | Creative Problem Solving | 🗺️ Roadmap | Novel solution generation within constraints **(true innovation and exploration)** |

## SPlectrum Application Focus

*Real-world application domains enabled by the platform capabilities*

| Domain | Description |
|--------|-------------|
| **Private P2P Networks** | Family and private group applications where trust is inherent and privacy is paramount. Home automation systems that operate without external servers, shared photo libraries within families, private communications, and collaborative tools for small trusted groups. These networks prioritize privacy, control, and independence from external infrastructure. |
| **Public P2P Networks** | Mass participation applications designed for open communities while maintaining decentralized infrastructure. Blockchain-integrated solutions, community platforms, content sharing networks, and collaborative applications that benefit from distributed participation without central control points. |
| **Business P2P Networks** | Enterprise applications that create ringfenced networks for specific employee groups or business functions. Department-specific tools, project collaboration networks, and business applications that maintain organizational boundaries while eliminating central server dependencies and reducing infrastructure costs. |

## Documentation, Organization Structure & Key Repositories

### 📄 **Project Documentation** ([`docs/`](./docs/))
Comprehensive technical documentation covering vision, architecture, implementation guides, and references for the entire SPlectrum ecosystem.

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