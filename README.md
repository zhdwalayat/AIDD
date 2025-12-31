# NOTE-X: Academic Note Generation System

## Project Overview

NOTE-X is an AI-powered academic note generation system designed to create mastery-level study materials. The system combines structured specification-driven workflows with AI-assisted content generation to produce comprehensive notes, reinforcement flash cards, and adaptive assessments.

## System Architecture

### Core Components

#### 1. CLAUDE.md
Defines behavioral guidelines and communication principles for the AI agent:
- Academic tone and communication standards
- Pedagogical philosophy and mastery learning principles
- Quality assurance standards
- Academic integrity and source attribution guidelines
- Ethical considerations and user interaction principles

#### 2. Skill.md
Provides operational procedures and execution workflows:
- Topic input source processing (files, URLs, books)
- Directory structure templates and organization protocols
- Note generation procedures with Bloom's Taxonomy integration
- Flash card generation guidelines (Q/A format)
- Quiz generation procedures (multiple-choice format)
- Assessment and feedback protocols
- Complete workflow execution sequences

## Directory Structure

```
notes/
├── README.md                    # Project documentation (this file)
├── CLAUDE.md                    # Behavioral guidelines and principles
├── Skill.md                     # Operational procedures and workflows
└── [Topic_Name]/                # Individual topic directories
    ├── Notes/
    │   └── [topic]_notes.md     # Comprehensive study notes
    ├── Flash_cards/
    │   └── [topic]_flashcards.md # Q/A format flash cards
    ├── Quiz/
    │   └── [topic]_quiz.md      # Multiple-choice assessment quiz
    └── Source_Materials/         # (Optional) Original reference materials
        ├── [source_files]       # PDFs, documents, etc.
        └── references.md        # Source citations and URLs
```

## Study Materials Format

### Notes
Each note document includes:
- **Two-line Summary**: Concise overview and significance
- **Foundational Concepts**: Remember/Understand level (Bloom's Taxonomy)
- **Application & Analysis**: Apply/Analyze level
- **Advanced Understanding**: Evaluate/Create level (when appropriate)
- **Key Takeaways**: 5-8 essential points
- **References & Sources**: Complete attribution

### Flash Cards
- **Format**: Question/Answer pairs
- **Quantity**: Variable (8-30 cards based on topic complexity)
- **Distribution**: 40% foundational, 40% intermediate, 20% advanced
- **Coverage**: All main concepts from notes

### Quizzes
- **Format**: Multiple-choice (4 options: A, B, C, D)
- **Quantity**: 15 questions (standard), adjustable based on complexity
- **Distribution**: 33% low difficulty, 47% medium, 20% advanced
- **Passing Threshold**: 70%
- **Features**: Answer key, explanations, adaptive retake support

## Current Topics

### Spec Kit Plus
**Location**: `Spec-Kit-Plus/`

A comprehensive study of Spec Kit Plus, a practical toolkit for building scalable multi-agent AI systems through spec-driven development.

**Contents**:
- Comprehensive notes (4,500+ words)
- 20 flash cards covering foundational to advanced concepts
- 15-question assessment quiz with mixed difficulty levels
- Source attribution (GitHub repository)

**Key Concepts Covered**:
- Spec-driven development methodology
- Multi-agent AI system architecture
- Core workflow commands (`/sp.constitution`, `/sp.specify`, `/sp.plan`, `/sp.tasks`, `/sp.implement`)
- Integration with 15+ AI coding agents
- Technology stack (Docker, Kubernetes, Dapr, Ray, OpenAI SDK, MCP)
- First-class artifact management
- Cross-artifact consistency validation

## Pedagogical Framework

### Bloom's Taxonomy Integration
The system structures learning progression through six cognitive levels:

1. **Remember**: Foundational facts, definitions, terminology
2. **Understand**: Explanations, interpretations, conceptual frameworks
3. **Apply**: Practical applications, procedures, methodologies
4. **Analyze**: Component analysis, relationships, systematic examination
5. **Evaluate**: Critical assessment, comparisons, justifications
6. **Create**: Synthesis, design, original applications

### Mastery Learning Approach
- **Competency Threshold**: 70% minimum on assessments
- **Adaptive Support**: Additional materials for struggling learners
- **Iterative Assessment**: Retake opportunities with expanded question sets
- **Personalized Feedback**: Specific recommendations based on performance

## Usage Workflow

### Creating New Study Materials

1. **Provide Topic**: Submit topic via direct description, file, URL, or book reference
2. **Directory Setup**: Specify directory name for organization
3. **Material Generation**: System generates notes, flash cards, and quiz
4. **Study & Practice**: Review notes and practice with flash cards
5. **Assessment**: Complete quiz to evaluate mastery
6. **Adaptive Learning**: Receive feedback and additional support if needed (score < 70%)
7. **Mastery Achievement**: Pass assessment (score ≥ 70%) to demonstrate competency

### Input Source Types

The system accepts multiple input formats:
- **Direct Topic Request**: Verbal topic description
- **Files**: PDF, TXT, MD, DOCX, IPYNB, images
- **URLs**: Articles, documentation, educational websites
- **Books**: Title/author references, chapter specifications

## Quality Standards

### Content Quality
- Factual accuracy and currency
- Technical precision
- Comprehensive coverage
- Logical flow and clarity

### Pedagogical Quality
- Systematic progression from simple to complex
- Balanced difficulty distribution
- Effective assessment aligned with learning objectives
- Constructive, actionable feedback

### Academic Integrity
- Proper source attribution
- Accurate representation of source materials
- Original synthesis and educational value
- Transparency about AI-generated content

## Technical Implementation

### AI Agent Integration
- Supports 15+ AI coding agents
- Agent-agnostic architecture
- Vendor independence
- Capability optimization

### File Formats
- All notes, flash cards, and quizzes: Markdown (.md)
- Supports reading: PDF, TXT, MD, DOCX, IPYNB, images
- Version control friendly

## License

This educational system and generated materials are intended for academic and personal learning purposes.

## Version History

### v1.0.0 (2025-12-31)
- Initial system implementation
- CLAUDE.md behavioral guidelines
- Skill.md operational procedures
- First topic: Spec Kit Plus with comprehensive materials
- Complete directory structure and workflow

## Contributing

To add new topics to this repository:

1. Create topic directory following naming convention
2. Generate materials using system workflows
3. Ensure all quality standards are met
4. Update this README with topic information
5. Commit with descriptive message

## Author

Generated using Claude Sonnet 4.5 with academic note generation system specifications.

---

**Note**: This system emphasizes mastery learning, academic rigor, and pedagogical effectiveness. All materials maintain formal academic tone and evidence-based reasoning throughout.
