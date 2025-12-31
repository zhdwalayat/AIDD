# Setup and Demo Guide - Academic Note Generation System

## Project Overview

This is an AI-powered academic note generation system that creates mastery-level study materials automatically. The system generates comprehensive notes, flash cards, and quizzes from any topic, file, URL, or book reference.

## For Instructors/Evaluators: Quick Demo Guide

### What This Project Does

This system demonstrates an AI-powered educational workflow that:
1. Takes a topic as input (text, PDF, URL, or book reference)
2. Generates comprehensive academic notes following Bloom's Taxonomy
3. Creates reinforcement flash cards (Q/A format)
4. Produces adaptive assessment quizzes (multiple-choice)
5. Provides mastery-based feedback (70% passing threshold)
6. Offers adaptive learning support for struggling students

### System Architecture

**Two Core Instruction Files:**
- `CLAUDE.md` - Defines AI behavior, academic tone, and pedagogical principles
- `Skill.md` - Contains operational workflows and execution procedures

**Output Structure:**
- Comprehensive notes with 2-line summaries
- Flash cards with difficulty distribution (40% foundational, 40% intermediate, 20% advanced)
- Assessment quizzes with mixed difficulty (33% low, 47% medium, 20% advanced)

---

## How to View the Demonstration

### Option 1: View Existing Example (Quickest)

The repository includes a complete working example in the `Spec-Kit-Plus/` directory:

1. **Navigate to the example:**
   ```
   Spec-Kit-Plus/
   ├── Notes/spec-kit-plus_notes.md
   ├── Flash_cards/spec-kit-plus_flashcards.md
   └── Quiz/spec-kit-plus_quiz.md
   ```

2. **Review the materials:**
   - **Notes**: Open `Spec-Kit-Plus/Notes/spec-kit-plus_notes.md` to see comprehensive academic content
   - **Flash Cards**: Open `Spec-Kit-Plus/Flash_cards/spec-kit-plus_flashcards.md` to see 20 Q/A cards
   - **Quiz**: Open `Spec-Kit-Plus/Quiz/spec-kit-plus_quiz.md` to see 15-question assessment

3. **Observe the features:**
   - Academic tone and formal language throughout
   - Structured progression through Bloom's Taxonomy levels
   - Comprehensive coverage from foundational to advanced concepts
   - Clear learning objectives and key takeaways
   - Source attribution and references

### Option 2: Run the System (Full Demonstration)

To see the system generate new materials, you'll need an AI assistant with access to these instruction files.

#### Prerequisites
- Claude Code CLI, or
- Any AI assistant that can read instruction files (Claude, ChatGPT, etc.)

#### Steps to Run:

1. **Clone this repository:**
   ```bash
   git clone https://github.com/zhdwalayat/AIDD.git
   cd AIDD
   ```

2. **Load the instruction files:**
   - Open `CLAUDE.md` and `Skill.md` in your AI assistant
   - These files contain all behavioral and operational instructions

3. **Provide a topic:**
   Choose any topic, such as:
   - "Machine Learning Fundamentals"
   - "Quantum Computing Basics"
   - "Database Normalization"
   - Or provide a PDF/URL as input

4. **Observe the workflow:**
   The system will:
   - Request a directory name for organization
   - Create structured directories (Notes, Flash_cards, Quiz, Source_Materials)
   - Generate comprehensive notes with academic rigor
   - Create flash cards for reinforcement
   - Generate assessment quiz with mixed difficulty
   - Administer quiz and provide adaptive feedback

5. **Expected output structure:**
   ```
   [Your_Topic]/
   ├── Notes/
   │   └── [topic]_notes.md
   ├── Flash_cards/
   │   └── [topic]_flashcards.md
   ├── Quiz/
   │   └── [topic]_quiz.md
   └── Source_Materials/
       └── references.md
   ```

---

## Evaluation Checklist for Instructors

### ✓ System Features to Verify

**1. Input Flexibility**
- [ ] Accepts direct topic descriptions
- [ ] Processes PDF files
- [ ] Fetches content from URLs
- [ ] Works with book references

**2. Content Quality**
- [ ] Academic tone maintained throughout
- [ ] Proper Bloom's Taxonomy progression
- [ ] Comprehensive coverage of topics
- [ ] Clear examples and explanations
- [ ] Proper source attribution

**3. Note Generation**
- [ ] Two-line summary present
- [ ] Structured sections (Foundational, Application, Advanced)
- [ ] Key takeaways section (5-8 points)
- [ ] References and sources section

**4. Flash Card Quality**
- [ ] Q/A format consistently applied
- [ ] Appropriate quantity (8-30 based on complexity)
- [ ] Difficulty distribution (40/40/20)
- [ ] Clear, focused questions
- [ ] Comprehensive answers

**5. Quiz Assessment**
- [ ] Multiple-choice format (4 options)
- [ ] Appropriate quantity (15 questions standard)
- [ ] Difficulty distribution (33% low, 47% medium, 20% advanced)
- [ ] Answer key with explanations
- [ ] Covers all major concepts

**6. Adaptive Learning**
- [ ] 70% passing threshold enforced
- [ ] Detailed feedback provided
- [ ] Weak areas identified
- [ ] Retake support offered
- [ ] Additional materials generated for struggling students

**7. Documentation**
- [ ] Comprehensive README.md
- [ ] Clear project structure
- [ ] Professional git commit messages
- [ ] Proper file organization

---

## Technical Implementation Details

### File Formats
- All notes, flash cards, quizzes: Markdown (.md)
- Supports reading: PDF, TXT, MD, DOCX, IPYNB, images
- Version control: Git with proper commit structure

### Pedagogical Framework
**Bloom's Taxonomy Integration:**
1. Remember: Definitions, terminology, facts
2. Understand: Explanations, interpretations
3. Apply: Procedures, methodologies, examples
4. Analyze: Component analysis, relationships
5. Evaluate: Critical assessments, comparisons
6. Create: Synthesis, design, original applications

**Mastery Learning:**
- Minimum competency: 70%
- Iterative assessment until mastery
- Personalized feedback and support

### Quality Standards
- **Accuracy**: Factually correct, technically precise
- **Completeness**: Comprehensive coverage without gaps
- **Clarity**: Accessible yet rigorous language
- **Relevance**: Aligned with learning objectives

---

## Demo Scenarios for Testing

### Scenario 1: Simple Topic
**Input**: "Pythagorean Theorem"
**Expected Output**:
- Notes: 800-1500 words
- Flash cards: 8-12 cards
- Quiz: 10-12 questions
- Focus: Remember, Understand, Apply levels

### Scenario 2: Complex Topic
**Input**: PDF on "Neural Networks and Deep Learning"
**Expected Output**:
- Notes: 3000-5000 words
- Flash cards: 18-25 cards
- Quiz: 18-20 questions
- Focus: All Bloom's levels through Create

### Scenario 3: URL Reference
**Input**: Online article URL
**Expected Output**:
- Source attribution in references
- Content synthesized from article
- Original educational value added
- Proper citations maintained

---

## Frequently Asked Questions

### Q: Is this a standalone application?
**A**: This is an AI instruction system. The CLAUDE.md and Skill.md files instruct an AI assistant (like Claude Code) on how to generate educational materials. The Spec-Kit-Plus folder shows example output.

### Q: Can I generate materials for any topic?
**A**: Yes! The system accepts:
- Topic descriptions (e.g., "Photosynthesis")
- PDF documents
- URLs to articles/documentation
- Book chapter references

### Q: How is quality ensured?
**A**: Multiple mechanisms:
- Strict behavioral guidelines in CLAUDE.md
- Detailed operational procedures in Skill.md
- Academic tone requirements
- Bloom's Taxonomy framework
- Cross-artifact consistency validation

### Q: What makes this different from AI-generated notes?
**A**: This system provides:
- Structured pedagogical framework
- Mastery-based assessment
- Adaptive learning support
- Professional documentation hierarchy
- Version-controlled educational artifacts

### Q: Can students use this for any course?
**A**: Yes! The system is domain-agnostic and works for:
- STEM subjects (Math, Physics, CS, Engineering)
- Humanities (History, Philosophy, Literature)
- Professional subjects (Business, Law, Medicine)
- Technical training and certifications

---

## Repository Structure Explanation

```
AIDD/
├── README.md                    # Project overview and documentation
├── SETUP_AND_DEMO.md           # This file - setup and demo guide
├── CLAUDE.md                    # AI behavioral instructions
├── Skill.md                     # Operational workflows
└── Spec-Kit-Plus/              # Example output (working demo)
    ├── Notes/
    │   └── spec-kit-plus_notes.md     # Comprehensive study notes
    ├── Flash_cards/
    │   └── spec-kit-plus_flashcards.md # 20 reinforcement cards
    ├── Quiz/
    │   └── spec-kit-plus_quiz.md      # 15-question assessment
    └── Source_Materials/
        └── references.md              # Source attribution
```

---

## Grading Rubric Suggestion for Instructors

### Content Quality (40 points)
- Academic rigor and tone (10 pts)
- Bloom's Taxonomy integration (10 pts)
- Comprehensive coverage (10 pts)
- Source attribution (10 pts)

### Technical Implementation (30 points)
- Proper file structure (10 pts)
- Git usage and documentation (10 pts)
- Code/instruction quality (10 pts)

### Pedagogical Design (20 points)
- Assessment design (10 pts)
- Adaptive learning features (10 pts)

### Documentation (10 points)
- README clarity (5 pts)
- Demo instructions (5 pts)

**Total: 100 points**

---

## Contact and Support

**Student**: zhdwalayat
**Repository**: https://github.com/zhdwalayat/AIDD
**Generated Using**: Claude Sonnet 4.5 via Claude Code

---

## License

This project is submitted as an academic assignment demonstrating AI-powered educational system design and implementation.

**Date**: December 31, 2025
**Version**: 1.0.0
