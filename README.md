# SPlectrum Ecosystem

**Create tools to enable P2P networks where distributed applications run in their own peer-to-peer environment, extending blockchain's decentralization philosophy to general-purpose computing.**

## Vision

Transform how distributed applications are built and deployed through:
- Tools to easily create custom P2P networks
- Applications that run natively in peer-to-peer environments  
- AI-enhanced automation throughout development and deployment
- Collaborative AI creation (collaboration of minds, not hands)
- Native streaming application engine at the core

## Organization Structure

The SPlectrum ecosystem is organized around five specialized organizations, each addressing specific concerns:

### 🚀 **SPlectrum** - Execution Engine & Tool Integration
Core execution environment with DSL engine, unified API architecture, and streaming capabilities. Everything that exposes SPlectrum APIs lives here.

**Key Repository:** [`spl1`](https://github.com/SPlectrum/spl1) - Primary execution engine implementation

### 📦 **InfoMetish** - Packaging & Deployment  
Platform-specific packaging and deployment with container registry as authoritative source. Handles P2P packaging, container deployments, and traditional installations.

**Key Repository:** [`InfoMetis`](https://github.com/InfoMetish/InfoMetis) - Container registry and deployment orchestration

### 🤖 **Sesameh** - AI-Driven Behavioral Intelligence
Collaborative AI creation enabling human-AI partnership where humans define and AI implements. Quality gates, TDD workflows, and intelligent decision-making systems.

**Key Repository:** [`claude-swift`](https://github.com/Sesameh/claude-swift) - Collaborative AI development workflows

### 🔧 **Carambah** - Solution Composition
High-level solution assembly from simple component setups to complex vanilla solutions. Environment-agnostic compositions using vanilla dev configs.

**Key Repository:** [`carambah`](https://github.com/Carambah/carambah) - Solution composition engine

### ⚡ **bare-for-pear** - P2P Runtime Compatibility
JavaScript module conversions for Bare runtime (not Node.js), enabling true P2P networking capabilities through Pear platform integration.

**Status:** In development - foundational P2P networking modules

## How Organizations Work Together

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

## Technical Foundation

- **DSL Engine**: Domain-specific language for P2P application development
- **AVRO-based**: Apache AVRO provides schema foundation for all data exchange
- **Streaming Architecture**: Kafka-compatible structure with immutable records
- **AI-Friendly**: Uniform language environment enables AI reasoning and generation
- **Container Registry**: Authoritative source with ready execution environments

## Getting Started

This repository serves as the **centralized documentation hub** for the entire SPlectrum ecosystem. Each organization maintains its implementation repositories while documentation lives here for unified access.

**Next Steps:**
- Explore individual organization repositories for implementation details
- Check the `docs/` directory for detailed technical documentation
- Visit organization-specific documentation for deep dives

## Repository Ways of Working

For contributors and collaborators working within this repository:
- [**Documentation Standards**](./claude/project/docs/documentation-standards.md) - Writing style and quality guidelines
- [**Visual Documentation Guide**](./claude/project/docs/visual-documentation-guide.md) - Diagram standards and color palette
- [**AI Collaboration Patterns**](./claude/project/docs/ai-collaboration-patterns.md) - Effective AI partnership patterns

---

*Building the future of decentralized applications through collaborative AI and P2P networking.*