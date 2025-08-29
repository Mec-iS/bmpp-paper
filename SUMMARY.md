# BMPP: Blindly Meaningful Prompting Protocol

## Abstract

This paper introduces **BMPP (Blindly Meaningful Prompting Protocol)**, a protocol that enables reliable interoperability between distributed systems involving Natural Language machines such as LLMs and GPTs. BMPP extends the Blindly Simple Protocol Language (BSPL) with natural language annotations and Meaning Typed Prompting (MTP) techniques, maintaining formal verification guarantees while optimizing for LLM structured generation capabilities.

## Key Features

- 🔒 **Formal Verification**: Inherits all BSPL validation and verification features (causality checking, deadlock prevention, progress guarantees)
- 🌐 **Cross-System Interoperability**: Enables communication between heterogeneous agent systems across organizational boundaries
- 🚀 **High Performance**: Sub-100μs message processing with 100,000+ messages per second per core
- 📝 **Natural Language Annotations**: Semantic-rich protocol specifications that improve both machine and human interpretability
- 🦀 **Rust Implementation**: Production-ready toolchain with WebAssembly support for edge deployment

## Architecture Overview

BMPP operates at the **systems interoperability level**, complementing existing frameworks like LangChain and GraphChain by providing:

```
┌─────────────────────────────────────────────────────────────┐
│                    BMPP Protocol Layer                     │
│           (Cross-organizational interoperability)          │
├─────────────────────────────────────────────────────────────┤
│  LangChain  │  AutoGen  │  Custom Agents  │  MCP Servers   │
│             │           │                 │                │
├─────────────────────────────────────────────────────────────┤
│            Individual Organization Systems                  │
└─────────────────────────────────────────────────────────────┘
```

### Core Components

| Component | Description | Repository |
|-----------|-------------|------------|
| **Validation Engine** | BSPL-based formal verification | Integrated |
| **Context Management** | Semantic annotation and meaning preservation | [vibelang-rs](https://github.com/Mec-iS/vibelang-rs) |
| **Flow Management** | Protocol orchestration and agent coordination | [bmpp-agents-rs](https://github.com/Mec-iS/bmpp-agents-rs) |
| **Runtime** | Edge-deployable execution environment | [bmpp-agents-rs](https://github.com/Mec-iS/bmpp-agents-rs) |


## Quick Example

```
// Simple BMPP Protocol Definition
Purchase ("e-commerce transaction protocol") {
    roles
        Buyer ("party purchasing items"),
        Seller ("party selling items")
    
    parameters
        item_id ("unique product identifier"),
        price ("item cost in currency units")
    
    // Protocol interactions
    Buyer -> Seller: request_quote ("request price")[out item_id]
    Seller -> Buyer: provide_quote ("send price")[in item_id, out price]
    Buyer -> Seller: confirm_purchase ("complete transaction")[in price]
}
```

## Research Foundation

This work builds upon extensive research in:

- **Preliminary Studies**: [Structured Generation Features Engineering](https://github.com/Mec-iS/w3c-agents-features)
- **BSPL Theory**: Formal verification guarantees for distributed protocols
- **Meaning Typed Prompting**: Semantic annotation techniques for LLM integration

## Potential Cloud Platform Support
The workflow introduced is particularly efficient and effective using these cloud technologies:

- ⚡ **Fastly Edge Computing**: Native integration with automatic deployment
- ✨ **Cloudflare Workers**: Optimized WebAssembly builds
- ☁️ **Nuvolaris** Serverless
- 🐳 **Container Orchestration**: Docker and Kubernetes support
- 🌍 **WebAssembly**: Cross-platform edge deployment

It can provide relevant improvements in terms of financial costs monitoring and energy efficiency.

## Use Cases

- **Cross-Organizational AI Workflows**: Enable different organizations' AI systems to interact safely
- **Automated Commercial Transactions**: Handle buy-sell interactions with formal guarantees
- **Multi-Party Negotiations**: Complex protocols with multiple participants and decision points
- **Edge AI Orchestration**: Deploy intelligent agents at network edges with reliability

## Comparison with Existing Solutions

Starting from the approach of redesigning the developer experience, the BMPP toolchain compares with other tools available on the market as:

| Feature | BMPP | MCP | LangChain | AutoGen | JSON-RPC |
|---------|------|-----|-----------|---------|----------|
| Formal Verification | ✅ | ❌ | ❌ | ❌    | Limited  |
| Multi-Party Protocols | ✅ | ❌ | Limited  | Limited | ❌ |
| Cross-Organizational | ✅ | ❌ | ❌ | ❌ | ❌ |
| Natural Language Annotations | ✅ | ❌ | ❌ | ❌ | ❌ |
| Edge Deployment-friendly | ✅ | ❌ | Limited | Limited | - |

## Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

## Citation

If you use BMPP in your research, please cite:

```bibtex
@article{moriondo2025bmpp,
  title={BMPP: Blindly Meaningful Prompting Protocol for Safe and Performant Data Exchange Between Distributed Systems and LLMs},
  author={Moriondo, Lorenzo},
  journal={GitHub repository},
  url={https://github.com/Mec-iS/bmpp-paper},
  year={2025}
}
```

## Acknowledgments

- BSPL research community and contributors
- W3C Web Agents Working Group
- Meaning Typed Prompting (MTP) project contributors

For questions, issues, or collaboration inquiries, please [open an issue](https://github.com/Mec-iS/bmpp-paper/issues) or contact the author.

## Sponsor
You can sponsor my research at [Github Sponsors](https://github.com/sponsors/Mec-iS/)
