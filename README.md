# BMPP A reliable interoperability protocol for LLM systems

**Status**: 📝 Draft Paper | 🚧 Implementation in Progress

This is the draft paper to introduce **Blindly Meaningful Protocol (BMPP)** as a reliable interoperability protocol for systems based on/involving operability of Natural Language machines like LLMs/GPTs.

Some preliminary work about features engineering for structured generation using different LLMs has been done at [this repository](https://github.com/Mec-iS/w3c-agents-features).

BMPP allows working on a different level (systems interoperability) than LangChain, GraphChain and other available framework but its implementation provide some overlapping capabilities into:
* context management (using [vibelang-rs](https://github.com/Mec-iS/vibelang-rs))
* flow management (using [bmpp-agents-rs](https://github.com/Mec-iS/bmpp-agents-rs))
* runtime (only implemented as example but potentially easily deployable in cloud workers setting)
