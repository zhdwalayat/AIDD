# Spec Kit Plus - Flash Cards

## Flash Card 1
**Question**: What is Spec Kit Plus and what is its primary purpose?

**Answer**: Spec Kit Plus is a practical fork of GitHub's spec-kit designed for building scalable multi-agent AI systems. It combines spec-driven development with conversational AI generation ("vibe coding") to accelerate production-ready software development while maintaining structured specifications.

---

## Flash Card 2
**Question**: What is the core philosophical question that Spec Kit Plus addresses regarding modern software development?

**Answer**: "If AI writes the code, what is left for a developer to do?" The framework answers this by emphasizing that developers should focus on strategic problem-solving, system architecture, diagnostics, and technical governance rather than mechanical code writing.

---

## Flash Card 3
**Question**: What does "spec-driven development" mean in the context of Spec Kit Plus?

**Answer**: Spec-driven development prioritizes creating comprehensive specifications before implementation begins. Unlike traditional documentation that follows code creation, this approach inverts the relationship, making specifications the foundation from which AI-generated code is produced.

---

## Flash Card 4
**Question**: What are the five core workflow commands in Spec Kit Plus?

**Answer**: The five core workflow commands are: `/sp.constitution` (establish governing principles), `/sp.specify` (define requirements), `/sp.plan` (create technical roadmap), `/sp.tasks` (generate actionable tasks), and `/sp.implement` (execute implementation).

---

## Flash Card 5
**Question**: What is the purpose of the `/sp.constitution` command?

**Answer**: The `/sp.constitution` command establishes foundational governing principles for a project, including core values, constraints, quality standards, and architectural principles that guide all subsequent technical decisions and AI-generated code.

---

## Flash Card 6
**Question**: Name at least five AI coding agents that Spec Kit Plus integrates with.

**Answer**: Spec Kit Plus integrates with Claude Code, GitHub Copilot, Cursor, Gemini, Windsurf, Qwen Code, and many others—totaling 15+ supported agents. This multi-agent compatibility provides vendor independence and capability optimization.

---

## Flash Card 7
**Question**: What are the three supporting commands in Spec Kit Plus and their purposes?

**Answer**: The three supporting commands are: `/sp.clarify` (resolves underspecified requirements through targeted questions), `/sp.analyze` (validates cross-artifact consistency), and `/sp.checklist` (performs quality assurance verification).

---

## Flash Card 8
**Question**: What does it mean that Spec Kit Plus treats artifacts as "first-class citizens"?

**Answer**: It means that specifications, architecture history, prompts, tests, and evaluations receive equal importance to code. They undergo version control, peer review, automated validation, and comprehensive indexing, ensuring human understanding scales with AI-generated implementation.

---

## Flash Card 9
**Question**: What are the four main technology runtime environments supported by Spec Kit Plus?

**Answer**: The four main runtime environments are: Docker (containerization), Kubernetes (orchestration), Dapr with Actors and Workflows (distributed application runtime), and Ray (distributed computing for AI/ML workloads).

---

## Flash Card 10
**Question**: What is the difference between "0-to-1 greenfield development" and "brownfield iteration" in Spec Kit Plus?

**Answer**: Greenfield development starts with no existing codebase, allowing clean slate architecture with emphasis on constitution and planning phases. Brownfield iteration works with existing codebases, requiring extensive analysis, constraint-heavy specifications, and emphasis on consistency validation.

---

## Flash Card 11
**Question**: How do you install Spec Kit Plus, and what is the command alias used?

**Answer**: Spec Kit Plus can be installed via `pip install specifyplus` or run directly with `uvx specifyplus`. All commands use the shorthand alias `sp` (e.g., `/sp.specify` instead of `/specifyplus.specify`).

---

## Flash Card 12
**Question**: What is the Model Context Protocol (MCP) and why is it important in Spec Kit Plus?

**Answer**: MCP is a standardized protocol for managing context across model interactions, ensuring consistency in long-running conversations. It enables multiple AI agents to share consistent understanding of project state throughout the development process.

---

## Flash Card 13
**Question**: What role does Dapr's Actors pattern play in multi-agent systems within Spec Kit Plus?

**Answer**: Dapr Actors provide state management and concurrency control for agent-based systems. Each AI agent can be implemented as a Dapr actor, enabling location transparency, fault isolation, and scalable parallel execution of independent tasks.

---

## Flash Card 14
**Question**: What are the five categories of first-class artifacts in Spec Kit Plus?

**Answer**: The five first-class artifact categories are: specifications (requirements documents), architecture history (decision logs), prompts (structured AI instructions), tests (executable verification), and evaluations (quality assessment frameworks).

---

## Flash Card 15
**Question**: How does the `/sp.analyze` command perform cross-artifact consistency validation?

**Answer**: The command performs static analysis of code structure, parses specifications to extract requirements, constructs and compares dependency graphs from both specs and implementations, and uses natural language processing to analyze documentation consistency with formal specifications.

---

## Flash Card 16
**Question**: What are the three agent specialization patterns supported by Spec Kit Plus?

**Answer**: The three patterns are: Domain Experts (agents with deep knowledge in specific technical domains), Role-Based Agents (agents assuming development roles like architect or QA), and Phase-Specific Agents (agents optimized for particular workflow phases).

---

## Flash Card 17
**Question**: What is "vibe coding" in the context of Spec Kit Plus?

**Answer**: "Vibe coding" refers to conversational AI code generation where developers engage with AI agents through natural language interaction to generate implementation code rapidly while maintaining adherence to established specifications.

---

## Flash Card 18
**Question**: What are the four consistency validation dimensions performed by Spec Kit Plus?

**Answer**: The four dimensions are: requirement-to-implementation traceability, architecture-to-code alignment, test coverage mapping, and documentation accuracy. These ensure all artifacts remain synchronized as projects evolve.

---

## Flash Card 19
**Question**: Why is agent-agnostic architecture important in Spec Kit Plus?

**Answer**: Agent-agnostic architecture provides vendor independence (avoiding lock-in), capability optimization (selecting best tools for each task), redundancy and resilience (alternatives if one agent fails), and comparative evaluation (experimenting to find best-fit solutions).

---

## Flash Card 20
**Question**: What is the "creative exploration phase" workflow emphasis in Spec Kit Plus?

**Answer**: Creative exploration emphasizes rapid iteration with minimal specification overhead. The workflow follows: Specify (minimal) → Implement → Analyze → Clarify → Iterate, prioritizing discovery and learning over predetermined outcomes.

---
