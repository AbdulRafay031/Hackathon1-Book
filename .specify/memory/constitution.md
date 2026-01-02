<!-- Sync Impact Report
Version change: None (initial creation/major update) → 1.0.0
Modified principles:
  - PRINCIPLE_1_NAME → Technical Accuracy
  - PRINCIPLE_2_NAME → Clarity & Audience Focus
  - PRINCIPLE_3_NAME → Reproducibility
  - PRINCIPLE_4_NAME → Engineering Rigor & Traceability
  - PRINCIPLE_5_NAME → Zero Hallucination
Added sections:
  - Standards
  - Technical Stack & Content Scope
Removed sections: None
Templates requiring updates:
  - .specify/templates/plan-template.md ⚠ pending
  - .specify/templates/spec-template.md ⚠ pending
  - .specify/templates/tasks-template.md ⚠ pending
  - .claude/commands/sp.adr.md ⚠ pending
  - .claude/commands/sp.analyze.md ⚠ pending
  - .claude/commands/sp.checklist.md ⚠ pending
  - .claude/commands/sp.clarify.md ⚠ pending
  - .claude/commands/sp.constitution.md ✅ updated
  - .claude/commands/sp.git.commit_pr.md ⚠ pending
  - .claude/commands/sp.implement.md ⚠ pending
  - .claude/commands/sp.phr.md ⚠ pending
  - .claude/commands/sp.plan.md ⚠ pending
  - .claude/commands/sp.specify.md ⚠ pending
  - .claude/commands/sp.tasks.md ⚠ pending
Follow-up TODOs: None
-->
# AI-Native Book on Physical AI & Humanoid Robotics with Embedded RAG Chatbot Constitution

## Core Principles

### Technical Accuracy
Every claim and piece of information within the book MUST be rigorously source-backed. Prioritize authoritative sources from official documentation, peer-reviewed research, and established industry standards to ensure factual correctness.

### Clarity & Audience Focus
Content MUST be clear, concise, and accessible for an advanced Computer Science, AI, and Robotics audience. Complex concepts should be explained with precision, avoiding jargon where simpler terms suffice, while maintaining the depth expected by the target readership.

### Reproducibility
All code examples, configurations, and workflows presented in the book MUST be reproducible. Readers should be able to replicate results independently, requiring clear instructions, dependency management, and versioning for all tools and libraries used.

### Engineering Rigor & Traceability
The development process, including specifications, plans, and tasks, MUST adhere to engineering rigor and maintain full traceability via Spec-Kit Plus. This ensures a systematic approach, accountability, and the ability to link book content back to its design and implementation rationale.

### Zero Hallucination
Content, especially that generated or augmented by the embedded RAG chatbot, MUST exhibit zero hallucination. All information provided MUST be directly derived from the book's verified content or authoritative external sources, preventing the generation of inaccurate or unsupported facts.

## Standards

All claims MUST be source-backed.
Citation style: APA.
≥50% sources MUST be from official documentation or peer-reviewed work.
0% plagiarism tolerance.
Consistent terminology and modular structure throughout the book.

## Technical Stack & Content Scope

### Technical Stack
-   **Authoring**: Claude Code
-   **Specs**: Spec-Kit Plus (https://github.com/panaversity/spec-kit-plus/)
-   **Book**: Docusaurus → GitHub Pages
-   **RAG Chatbot**: OpenAI Agents / ChatKit SDKs, FastAPI, Neon Serverless Postgres, Qdrant Cloud (Free Tier)

### Content Scope
-   **Theme**: AI Systems in the Physical World (Embodied Intelligence)
-   **Modules**:
    1.  ROS 2: Nodes, Topics, Services, rclpy, URDF humanoids
    2.  Digital Twin: Gazebo & Unity, physics, sensors (LiDAR, depth, IMU)
    3.  NVIDIA Isaac™: Isaac Sim, synthetic data, Isaac ROS, Nav2
    4.  Vision-Language-Action: Whisper voice input, LLM task planning, ROS actions
-   **Capstone**: Autonomous humanoid system that receives voice commands, plans via LLM, navigates, perceives, and manipulates objects in simulation.

## Governance

This Constitution supersedes all other project practices and documentation. Amendments require formal documentation, explicit approval from project stakeholders, and a clear migration plan for any affected components or workflows. All Pull Requests and code reviews MUST verify compliance with these principles. Complexity introduced into the project MUST be justified against these core principles.

### Versioning Policy
-   **MAJOR**: Backward-incompatible governance/principle removals or redefinitions.
-   **MINOR**: New principle/section added or materially expanded guidance.
-   **PATCH**: Clarifications, wording, typo fixes, non-semantic refinements.

**Version**: 1.0.0 | **Ratified**: 2025-12-14 | **Last Amended**: 2025-12-14
