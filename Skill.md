# Academic Note Generation - Operational Skill Guide

## Overview

This document provides comprehensive operational procedures, workflows, templates, and execution details for generating mastery-level study materials. Use this guide in conjunction with **CLAUDE.md**, which establishes behavioral principles and communication standards.

---

## I. Topic Input Sources and Processing

### A. Accepted Input Types

The system accommodates multiple input sources for topic content generation:

#### 1. Direct Topic Request
- User provides topic name or description verbally
- Example: "Generate notes on Quantum Mechanics"
- **Action**: Proceed with knowledge synthesis from general understanding

#### 2. File-Based Input
User provides files in various formats:
- PDF documents (.pdf)
- Text files (.txt)
- Markdown files (.md)
- Word documents (.docx)
- Jupyter notebooks (.ipynb)
- Image files (screenshots, diagrams, scanned pages)
- Other document formats

Files may contain: lecture notes, textbook excerpts, research papers, study guides, presentations

**Action**: Read and analyze file content thoroughly using Read tool

#### 3. URL References
User provides web links to:
- Online articles and blog posts
- Documentation pages
- Educational websites
- Video transcripts
- Academic publications
- Online courses or tutorials

**Action**: Fetch and extract content using WebFetch tool

#### 4. Book References
User references physical or digital books by:
- Title and author
- Specific chapters or page ranges
- ISBN or publication information
- Book excerpts or quotations provided

**Action**: Work with provided excerpts or request specific sections from user

### B. Input Processing Protocol

**Step-by-Step Workflow**:

1. **Acknowledge Receipt**
   - Confirm the source material received
   - Template: "I have received the [PDF document/URL/book reference] on [Topic]. I shall process this material to generate comprehensive study notes."

2. **Source Analysis**
   - Identify main topics and subtopics
   - Determine scope and depth of content
   - Extract key concepts and learning objectives
   - Assess complexity level
   - Evaluate completeness of source coverage

3. **Clarification** (if needed)
   Ask user:
   - "Should I focus on specific sections or chapters?"
   - "Are there particular aspects you wish to emphasize?"
   - "What is your current familiarity level with this topic?"
   - "Should I supplement this material with additional context?"

4. **Content Extraction**
   - **For files**: Use Read tool to analyze content thoroughly
   - **For URLs**: Use WebFetch tool to retrieve and process information
   - **For books**: Work with provided excerpts; request specific sections if needed
   - **Multiple sources**: Process each source individually, then prepare for synthesis

5. **Synthesis** (for multiple sources)
   - Cross-reference concepts across sources
   - Identify complementary information
   - Resolve contradictions or discrepancies (note them if unresolvable)
   - Prioritize authoritative sources
   - Create unified, coherent narrative

---

## II. Directory Structure and File Organization

### A. Directory Structure Template

```
H:\P300\notes\
  └── [Topic_Name]\
      ├── Notes\
      │   └── [topic_name]_notes.md
      ├── Flash_cards\
      │   └── [topic_name]_flashcards.md
      ├── Quiz\
      │   └── [topic_name]_quiz.md
      └── Source_Materials\ (optional - only if files provided)
          ├── [original_file1.pdf]
          ├── [original_file2.txt]
          └── references.md
```

### B. Directory Creation Protocol

**Sequential Steps**:

1. **Confirm Topic**
   - Acknowledge the topic received
   - Template: "I acknowledge your topic on [Topic Name]."

2. **Request Directory Name**
   - Ask user to specify desired directory name
   - Template: "Please provide a directory name for organizing these materials (e.g., 'Quantum_Mechanics_Fundamentals')."

3. **Create Directory Structure** (using Bash tool)
   ```bash
   mkdir -p "H:\P300\notes\[Topic_Name]\Notes"
   mkdir -p "H:\P300\notes\[Topic_Name]\Flash_cards"
   mkdir -p "H:\P300\notes\[Topic_Name]\Quiz"
   ```

4. **Create Source_Materials Directory** (if files provided)
   ```bash
   mkdir -p "H:\P300\notes\[Topic_Name]\Source_Materials"
   ```

5. **Store Original Files** (if applicable)
   - Copy provided files to Source_Materials directory
   - Create references.md file listing all URLs and book citations

### C. File Naming Conventions

**Mandatory Format**:
- **Notes**: `[topic_name]_notes.md`
- **Flash Cards**: `[topic_name]_flashcards.md`
- **Quiz**: `[topic_name]_quiz.md`
- **References**: `references.md` (in Source_Materials directory)

**Examples**:
- `quantum_mechanics_notes.md`
- `machine_learning_flashcards.md`
- `database_systems_quiz.md`

---

## III. Note Generation Procedures

### A. Pre-Generation Analysis

**Before writing notes, complete this analysis**:

1. **Scope and Depth Assessment**
   - Determine breadth of topic coverage needed
   - Assess complexity level (introductory, intermediate, advanced)
   - Identify appropriate depth of explanation

2. **Prerequisite Knowledge Identification**
   - List foundational concepts required
   - Determine if prerequisites need brief review in notes

3. **Learning Objectives Definition**
   - Define what mastery entails for this topic
   - Identify key competencies learner should achieve

4. **Bloom's Taxonomy Level Determination**
   - Decide which cognitive levels are necessary:
     - **Remember**: Facts, definitions, terminology
     - **Understand**: Explanations, interpretations, frameworks
     - **Apply**: Practical applications, procedures
     - **Analyze**: Component analysis, relationships
     - **Evaluate**: Critical assessment, comparisons
     - **Create**: Synthesis, design, original applications
   - Plan progression through levels appropriate for mastery

5. **Source Material Coverage** (if applicable)
   - Assess completeness of provided sources
   - Identify gaps requiring supplementation
   - Plan integration strategy for multiple sources

### B. Note Structure Template

**Every note document must follow this exact structure**:

```markdown
# [Topic Name]

## Summary
[First line: Concise overview of the topic]
[Second line: Significance or key application of the topic]

## [Section 1 - Foundational Concepts] (Remember/Understand Level)

### [Subsection 1.1]
[Content explaining foundational concept]

[Examples, definitions, explanations as needed]

### [Subsection 1.2]
[Content continuing foundational coverage]

## [Section 2 - Application and Analysis] (Apply/Analyze Level)

### [Subsection 2.1]
[Content demonstrating applications]

[Practical examples, procedures, methodologies]

### [Subsection 2.2]
[Content providing analysis]

[Component breakdown, relationships, systematic examination]

## [Section 3 - Advanced Understanding] (Evaluate/Create Level - if appropriate)

### [Subsection 3.1]
[Content requiring critical evaluation]

[Comparisons, assessments, justifications]

### [Subsection 3.2] (optional)
[Content involving synthesis or creation]

[Design principles, original applications, creative synthesis]

## Key Takeaways

- [Essential point 1 - foundational]
- [Essential point 2 - application-focused]
- [Essential point 3 - advanced insight]
- [Essential point 4 - practical relevance]
- [Continue as needed, typically 5-8 points]

## References and Sources

[If sources were provided:]
- [Source Type]: [Title/Name] by [Author] ([Publication/Access Date])
- [URL]: [Full URL] (Accessed: [Date])
- [Book]: [Title] by [Author], [Publisher], [Year], Chapter/Pages [X]

[If no external sources:]
- Content synthesized from established knowledge in [field/domain]
```

### C. Content Development Guidelines

**1. Content Depth Requirements**:
- **Comprehensive Coverage**: Address all essential aspects of the topic
- **Logical Flow**: Ensure smooth transitions between concepts
- **Conceptual Clarity**: Explain complex ideas in accessible yet rigorous language
- **Practical Relevance**: Connect theoretical concepts to practical applications
- **Critical Context**: Provide historical, theoretical, or practical context where relevant
- **Source Integration**: Seamlessly integrate information from multiple sources

**2. Writing Principles**:
- Begin each section with overview or introduction
- Use hierarchical headings (H2, H3, H4) to organize content
- Include examples, illustrations, case studies where beneficial
- Incorporate visual descriptions when diagrams would be helpful
- Provide cross-references to related concepts
- Synthesize information coherently across all sources

**3. Bloom's Taxonomy Application**:
- **Remember Level**: Definitions, terminology, basic facts
- **Understand Level**: Explanations, summaries, interpretations
- **Apply Level**: Procedures, methodologies, practical examples
- **Analyze Level**: Component breakdowns, relationship mapping, comparative analysis
- **Evaluate Level**: Critical assessments, justifications, criteria-based judgments
- **Create Level**: Design principles, synthesis of ideas, original applications

**4. Length Guidance**:
- Simple topics: 800-1500 words
- Standard topics: 1500-3000 words
- Complex topics: 3000-5000 words
- Highly technical topics: 4000-6000+ words

### D. Note Generation Execution

**Step-by-Step Process**:

1. Create note file using Write tool
2. Structure content according to template
3. Write 2-line summary capturing essence and significance
4. Develop foundational sections (Remember/Understand)
5. Build application and analysis sections (Apply/Analyze)
6. Add advanced sections if topic warrants (Evaluate/Create)
7. Compile Key Takeaways (5-8 essential points)
8. Add References and Sources section
9. Review for completeness, accuracy, and clarity

---

## IV. Flash Card Generation Procedures

### A. Purpose and Function

Flash cards serve as active recall reinforcement tools to strengthen retention and facilitate spaced practice.

### B. Flash Card Format Template

```markdown
# [Topic Name] - Flash Cards

## Flash Card 1
**Question**: [Clear, focused question testing one concept]

**Answer**: [Comprehensive but concise answer - typically 2-4 sentences]

---

## Flash Card 2
**Question**: [Clear, focused question]

**Answer**: [Comprehensive but concise answer]

---

## Flash Card 3
**Question**: [Clear, focused question]

**Answer**: [Comprehensive but concise answer]

---

[Continue pattern for all flash cards]
```

### C. Quantity Determination

**Initial Baseline**:
- Simple topics: 8-12 flash cards
- Standard topics: 12-18 flash cards
- Complex topics: 18-25 flash cards
- Highly technical topics: 20-30 flash cards

**Adjustment Factors**:
- Extensive source materials: Increase by 30-50%
- User scored ≤ 70% on quiz: Increase by 50-100% in next iteration
- User specifically requests more/fewer: Adjust accordingly

### D. Coverage Requirements

Flash cards must:
- Cover all main concepts from notes
- Include mix of difficulty levels:
  - 40% foundational (Remember/Understand)
  - 40% intermediate (Apply/Analyze)
  - 20% advanced (Evaluate/Create)
- Address all relevant Bloom's taxonomy levels covered in notes
- Reinforce critical relationships and applications
- Test both theoretical knowledge and practical understanding

### E. Flash Card Design Principles

**Question Design**:
- **Clarity**: Each question must be unambiguous
- **Specificity**: Focus on one concept per card
- **Relevance**: Align with learning objectives from notes
- **Progressive Difficulty**: Range from basic recall to complex application
- **Variety**: Use different question types:
  - Definition questions: "What is...?"
  - Explanation questions: "Why does...?"
  - Application questions: "How would you...?"
  - Analysis questions: "What is the relationship between...?"
  - Comparison questions: "What is the difference between...?"

**Answer Design**:
- **Completeness**: Provide sufficient detail for understanding
- **Conciseness**: Typically 2-4 sentences
- **Accuracy**: Ensure factual correctness
- **Clarity**: Use clear, accessible language
- **Source Alignment**: Accurately reflect information from notes and sources

### F. Flash Card Generation Execution

**Step-by-Step Process**:

1. Review notes to identify key concepts
2. Determine appropriate number of flash cards
3. Create flash card file using Write tool
4. Generate questions covering all main topics
5. Distribute across difficulty levels (40/40/20)
6. Write comprehensive but concise answers
7. Review for coverage, accuracy, and clarity
8. Ensure alignment with notes content

---

## V. Quiz Generation Procedures

### A. Purpose and Assessment Philosophy

Quizzes serve to:
- Evaluate user comprehension and mastery
- Identify specific knowledge gaps
- Provide diagnostic feedback
- Determine if 70% competency threshold is achieved

### B. Quiz Format Template

```markdown
# [Topic Name] - Assessment Quiz

## Instructions
- This quiz contains [X] questions covering [Topic Name]
- Each question has four options (A, B, C, D)
- Select the best answer for each question
- Passing score: 70%
- You may retake the quiz if you score below 70%

---

## Question 1
[Question text - clear, specific, unambiguous]

A) [Option A - plausible distractor or correct answer]
B) [Option B - plausible distractor or correct answer]
C) [Option C - plausible distractor or correct answer]
D) [Option D - plausible distractor or correct answer]

**Correct Answer**: [A/B/C/D]
**Explanation**: [2-3 sentence explanation of why this answer is correct and optionally why others are incorrect]

---

## Question 2
[Question text]

A) [Option A]
B) [Option B]
C) [Option C]
D) [Option D]

**Correct Answer**: [A/B/C/D]
**Explanation**: [Explanation]

---

[Continue pattern for all questions]

---

## Answer Key Summary

1. [A/B/C/D]
2. [A/B/C/D]
3. [A/B/C/D]
[Continue for all questions]
```

### C. Question Quantity and Difficulty Distribution

**Initial Quiz**:
- **Standard approach**: 15 questions
- **Simple topics**: 10-12 questions
- **Complex topics**: 18-20 questions
- **Extensive source materials**: 18-20 questions

**Difficulty Distribution for 15 questions**:
- **Low Difficulty** (Remember/Understand): 5 questions (33%)
- **Medium Difficulty** (Apply/Analyze): 7 questions (47%)
- **Advanced Difficulty** (Evaluate/Create): 3 questions (20%)

**Difficulty Distribution for other quantities**:
- Maintain approximately 33% low, 47% medium, 20% advanced
- Adjust proportions slightly based on topic nature

**Retake Quiz** (if user scores ≤ 70%):
- Generate 20-25 questions
- Focus 60% of questions on areas where user struggled
- Maintain some questions on areas user understood (40%)
- Keep similar difficulty distribution overall

### D. Question Design Standards

**Question Quality Requirements**:
1. **Clarity**: Unambiguous, professionally worded
2. **Relevance**: Directly assess learning objectives from notes
3. **Discrimination**: Distinguish between levels of understanding
4. **No Tricks**: Avoid intentionally deceptive questions
5. **Source Fidelity**: Accurately assess content from provided sources

**Distractor Quality** (incorrect options):
- Plausible to someone with partial understanding
- Clearly incorrect to someone with mastery
- Avoid obviously wrong or absurd options
- Use common misconceptions as distractors when appropriate

**Question Types to Include**:
- Definition/terminology questions (low difficulty)
- Conceptual understanding questions (low-medium difficulty)
- Application scenario questions (medium difficulty)
- Analysis questions requiring reasoning (medium-advanced difficulty)
- Evaluation questions requiring judgment (advanced difficulty)

### E. Coverage Requirements

Quiz must:
- Assess all major concepts from notes
- Include questions at multiple Bloom's taxonomy levels
- Test both theoretical understanding and practical application
- Ensure balanced representation across topic sections
- Cover key points from all provided source materials
- Avoid over-concentration on any single subtopic

### F. Quiz Generation Execution

**Step-by-Step Process**:

1. Review notes to identify all major concepts
2. Determine appropriate number of questions (typically 15)
3. Calculate difficulty distribution (5 low, 7 medium, 3 advanced)
4. Create quiz file using Write tool
5. Write instructions section
6. Generate questions with balanced coverage:
   - Start with low-difficulty questions on foundational concepts
   - Progress to medium-difficulty application questions
   - Conclude with advanced-difficulty questions
7. Create four plausible options for each question
8. Mark correct answer for each question
9. Write explanation for each question
10. Create answer key summary at end
11. Review for coverage, clarity, and accuracy

---

## VI. Assessment and Feedback Procedures

### A. Quiz Administration Workflow

**Sequential Steps**:

1. **Pre-Quiz Briefing**
   - Present quiz to user in designated Quiz directory
   - Inform user of:
     - Number of questions
     - Passing threshold (70%)
     - Retake option if needed
   - Template: "I have generated an assessment quiz with [X] questions. The passing threshold is 70%. Please review the quiz in [file_path] and provide your answers in the format: 1-A, 2-C, 3-B, etc."

2. **Quiz Presentation**
   - Quiz is already written to file in Quiz subdirectory
   - User accesses quiz file independently

3. **Answer Collection**
   - Request format: "1-A, 2-C, 3-B, 4-D, 5-A, ..."
   - Template: "Please provide your answers in the format: 1-A, 2-C, 3-B, etc."

4. **Scoring**
   - Count correct answers
   - Calculate percentage: (Correct / Total) × 100
   - Determine pass/fail status (≥70% = pass)

5. **Results Communication**
   - Provide detailed feedback using templates below

### B. Results Communication Templates

**For Passing Scores (≥ 70%)**:

```
Assessment Results:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Score: [X]/[Total] ([Percentage]%)
Status: PASSED ✓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Congratulations. You have demonstrated competency in [Topic Name]. Your performance indicates [solid foundational understanding / strong comprehensive grasp / excellent mastery-level comprehension].

[If score is 70-79%]:
You have achieved the minimum threshold for competency. I recommend reviewing [specific topics where errors occurred] to strengthen your understanding further.

[If score is 80-89%]:
You have demonstrated strong understanding of this topic. Minor review of [specific topics if any errors] would ensure complete mastery.

[If score is 90-100%]:
You have demonstrated excellent mastery of this topic. Your comprehensive understanding indicates readiness for advanced applications or related topics.

Would you like to:
1. Proceed to a new related topic
2. Explore advanced aspects of this topic
3. Generate additional study materials
```

**For Failing Scores (< 70%)**:

```
Assessment Results:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Score: [X]/[Total] ([Percentage]%)
Status: NOT PASSED (Minimum required: 70%)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Analysis of Performance:
Your assessment reveals specific areas requiring additional study:

Areas Requiring Focus:
- [Specific topic/concept 1 where errors occurred]
- [Specific topic/concept 2 where errors occurred]
- [Specific topic/concept 3 where errors occurred]

Recommended Actions:
1. Review the following sections in your notes:
   - [Specific note section reference]
   - [Specific note section reference]

2. Study the following flash cards:
   - Flash cards [numbers] addressing [concept]

3. [Any specific concept clarification needed]

Retake Preparation:
I recommend taking the following steps before attempting the quiz again:

Option 1: Review existing materials
- Study the note sections listed above
- Practice with the recommended flash cards
- Request clarification on any unclear concepts

Option 2: Receive expanded learning materials
- I can generate [X additional] flash cards focused specifically on your weak areas
- I can provide supplementary explanations for challenging concepts
- I can create an expanded quiz with more questions on areas you found difficult

Please indicate your preference:
A) I would like to review materials and retake the current quiz
B) I would like expanded flash cards and then retake
C) I would like concept clarification before retaking
D) Other (please specify)
```

### C. Adaptive Learning Path Execution

**For Passing Scores (≥ 70%)**:

1. Acknowledge mastery achievement
2. Provide performance analysis
3. Offer options for proceeding:
   - New topic
   - Advanced exploration of current topic
   - Related topics
   - Additional materials

**For Failing Scores (< 70%)**:

1. **Identify Specific Weak Areas**:
   - Analyze which questions were missed
   - Determine conceptual areas of weakness
   - Reference specific note sections needing review

2. **Generate Targeted Recommendations**:
   - Specific note sections to review
   - Specific flash cards to study
   - Concepts requiring clarification

3. **Offer Adaptive Support**:
   - Generate 50-100% more flash cards focused on weak areas
   - Offer concept clarification
   - Prepare expanded quiz (20-25 questions) for retake

4. **Prepare Retake Materials** (if user chooses expanded support):
   - Generate additional flash cards targeting weak concepts
   - Create new quiz with 60% emphasis on weak areas, 40% on understood areas
   - Maintain difficulty distribution

5. **Iterative Process**:
   - Repeat until user achieves ≥70%
   - Track progress across attempts
   - Adjust support level based on improvement trajectory

---

## VII. Complete Workflow Execution

### End-to-End Topic Generation Sequence

**Phase 1: Topic Intake and Setup**

1. Receive topic from user (verbal, file, URL, or book reference)
2. Acknowledge receipt
3. Process source materials if provided
4. Confirm understanding
5. Request directory name
6. Receive directory name from user

**Phase 2: Directory Creation**

7. Create directory structure using Bash tool
8. If files provided, create Source_Materials directory
9. Store original files (if applicable)

**Phase 3: Content Generation**

10. Analyze topic (scope, depth, Bloom's levels, learning objectives)
11. Generate comprehensive notes
12. Inform user of notes completion
13. Generate flash cards
14. Inform user of flash cards completion
15. Generate quiz
16. Inform user of quiz completion

**Phase 4: Quiz Administration**

17. Present quiz to user
18. Provide instructions
19. Request answers
20. Receive user's answers

**Phase 5: Assessment and Feedback**

21. Score quiz
22. Calculate percentage
23. Determine pass/fail status
24. Provide detailed feedback

**Phase 6: Adaptive Response**

25. If passed: Congratulate and offer next steps
26. If failed: Identify weak areas, provide recommendations, offer adaptive support
27. Iterative support if needed

---

## VIII. Implementation Checklist

**Use this checklist for every topic**:

### Pre-Generation
- [ ] Topic received and acknowledged
- [ ] Source materials processed (if applicable)
- [ ] Directory name requested and received

### Directory Setup
- [ ] All required directories created
- [ ] Source files stored (if applicable)

### Content Generation
- [ ] Notes generated with all required sections
- [ ] Flash cards generated with proper distribution
- [ ] Quiz generated with proper distribution
- [ ] User informed of all completions

### Assessment
- [ ] Quiz administered
- [ ] Answers collected and scored
- [ ] Feedback provided
- [ ] Adaptive support offered (if needed)

### Quality Assurance
- [ ] All information accurate
- [ ] Academic tone maintained
- [ ] Proper formatting
- [ ] Files in correct directories

---

## Conclusion

This operational guide provides detailed procedures for executing the academic note generation system. By following these workflows systematically, you will produce high-quality study materials that facilitate mastery learning.

Execute these procedures with precision, thoroughness, and commitment to educational excellence.
