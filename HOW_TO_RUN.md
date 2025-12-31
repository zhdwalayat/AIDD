# How to Run NOTE-X - Instructions for Teacher

## 🎯 Project Purpose

NOTE-X is an AI-powered academic note generation system. When you provide a topic (text, PDF, or URL), it automatically generates:
- Comprehensive study notes with academic rigor
- Flash cards for reinforcement (Q/A format)
- Assessment quiz (multiple-choice with 70% passing threshold)
- Adaptive feedback and support

## 📋 What You'll Need

1. **Claude Code CLI** (recommended) - OR - Any AI assistant that can read instruction files
2. This repository cloned to your computer
3. A topic you want to generate study materials for

---

## 🚀 Step-by-Step: How to Run

### Step 1: Clone the Repository

```bash
git clone https://github.com/zhdwalayat/AIDD.git
cd AIDD
```

### Step 2: Open in Claude Code (or your AI assistant)

```bash
# If using Claude Code CLI:
cd AIDD
claude-code
```

**OR** if using another AI assistant:
- Load the `CLAUDE.md` file (contains behavioral instructions)
- Load the `Skill.md` file (contains operational workflows)

### Step 3: Provide Your Topic

In your AI assistant, say one of the following:

**Option A - Simple Topic:**
```
Generate study materials for "Photosynthesis"
```

**Option B - With PDF File:**
```
I have a PDF on "Machine Learning". Generate study materials from it.
[Then provide the PDF file path]
```

**Option C - With URL:**
```
Generate notes from this URL: https://example.com/article
```

### Step 4: Specify Directory Name

When prompted, provide a directory name:
```
Example: "photosynthesis" or "machine_learning"
```

### Step 5: Watch the System Work

The system will automatically:

1. **Create directory structure:**
   ```
   [Your_Topic]/
   ├── Notes/
   ├── Flash_cards/
   ├── Quiz/
   └── Source_Materials/
   ```

2. **Generate comprehensive notes** with:
   - Two-line summary
   - Foundational concepts
   - Application examples
   - Advanced understanding
   - Key takeaways (5-8 points)
   - Source references

3. **Create flash cards** (Q/A format):
   - Variable quantity based on topic complexity
   - 40% foundational, 40% intermediate, 20% advanced
   - Clear questions with comprehensive answers

4. **Generate assessment quiz**:
   - 15 questions (multiple-choice)
   - 33% low difficulty, 47% medium, 20% advanced
   - Answer key with explanations

5. **Administer the quiz** and provide feedback

---

## 📝 Example Run-Through

Here's exactly what happens when you run it:

```
YOU: Generate study materials for "The Water Cycle"

AI: I acknowledge your topic on The Water Cycle. I shall generate
    comprehensive study materials including detailed notes,
    reinforcement flash cards, and an assessment quiz.

    Please provide a directory name for organizing these materials
    (e.g., 'Water_Cycle').

YOU: water_cycle

AI: [Creates directory structure]
    [Generates comprehensive notes - approximately 1500 words]
    [Generates 12 flash cards covering all main concepts]
    [Generates 12-question quiz with mixed difficulty]

    I have generated comprehensive study materials for The Water Cycle:

    1. Notes: H:\P300\notes\water_cycle\Notes\water_cycle_notes.md
    2. Flash Cards: H:\P300\notes\water_cycle\Flash_cards\water_cycle_flashcards.md
    3. Quiz: H:\P300\notes\water_cycle\Quiz\water_cycle_quiz.md

    The quiz contains 12 questions with a passing threshold of 70%.
    Please review the materials and complete the quiz when ready.

YOU: [Reviews materials and provides quiz answers]

AI: [Scores quiz and provides detailed feedback]
```

---

## ✅ Example Already Included: "Spec-Kit-Plus"

To see what the output looks like, check the **Spec-Kit-Plus** folder:

```
Spec-Kit-Plus/
├── Notes/spec-kit-plus_notes.md          ← 4,500+ word comprehensive notes
├── Flash_cards/spec-kit-plus_flashcards.md ← 20 Q/A flash cards
└── Quiz/spec-kit-plus_quiz.md            ← 15-question assessment
```

**This is a real example** generated using the exact same process you'll follow.

---

## 🎓 What the System Does Automatically

### Notes Generation
- **Academic Tone**: Formal, precise, evidence-based
- **Structure**: Follows Bloom's Taxonomy (Remember → Understand → Apply → Analyze → Evaluate → Create)
- **Summary**: Two-line concise overview
- **Content**: 800-6000 words depending on complexity
- **Quality**: Factually accurate, comprehensive, well-organized

### Flash Cards
- **Format**: Question on one side, answer on other
- **Quantity**: 8-30 cards (based on topic complexity)
- **Coverage**: All major concepts from notes
- **Difficulty Mix**:
  - 40% foundational (basic recall)
  - 40% intermediate (application)
  - 20% advanced (analysis/evaluation)

### Quiz
- **Format**: Multiple-choice (4 options: A, B, C, D)
- **Questions**: 10-20 (typically 15)
- **Difficulty Distribution**:
  - 33% low (Remember/Understand)
  - 47% medium (Apply/Analyze)
  - 20% advanced (Evaluate/Create)
- **Features**:
  - Answer key with explanations
  - Automatic scoring
  - Feedback with weak area identification
  - Retake support if score < 70%

---

## 🔧 System Requirements

### Minimum:
- Git installed
- Claude Code CLI or any AI assistant (Claude, ChatGPT, etc.)
- Text editor to view generated markdown files

### Recommended:
- VS Code with Markdown Preview
- Claude Code CLI for best experience
- GitHub account (to clone the repo)

---

## 📊 Testing the System

### Test Case 1: Simple Topic
**Input**: "Newton's Laws of Motion"
**Expected Output**:
- Notes: ~1200 words
- Flash cards: ~10 cards
- Quiz: ~12 questions
- Time: ~2-3 minutes

### Test Case 2: Complex Topic
**Input**: "Neural Networks and Backpropagation"
**Expected Output**:
- Notes: ~3500 words
- Flash cards: ~20 cards
- Quiz: ~18 questions
- Time: ~3-5 minutes

### Test Case 3: With Source Material
**Input**: PDF or URL about any topic
**Expected Output**:
- Same as above + source attribution
- Content synthesized from provided material
- References section with citations

---

## 🎯 How to Evaluate This Project

### 1. **Check the Example** (2 minutes)
   - Open `Spec-Kit-Plus/Notes/spec-kit-plus_notes.md`
   - Verify: academic tone, structure, comprehensiveness
   - Open `Spec-Kit-Plus/Quiz/spec-kit-plus_quiz.md`
   - Verify: quiz quality, explanations, difficulty mix

### 2. **Run Your Own Test** (5-10 minutes)
   - Choose any topic you know well
   - Follow the steps above to generate materials
   - Review the generated notes, flash cards, and quiz
   - Verify quality matches the example

### 3. **Check the System Design** (5 minutes)
   - Open `CLAUDE.md` - see behavioral guidelines
   - Open `Skill.md` - see operational workflows
   - Verify: pedagogical framework, quality standards

---

## 🔍 Key Features to Verify

When you run this with your own topic, verify:

✅ **Automatic Directory Creation**: Proper structure (Notes, Flash_cards, Quiz folders)

✅ **Academic Quality**:
- Formal tone throughout
- No contractions ("do not" not "don't")
- Evidence-based explanations
- Proper terminology

✅ **Bloom's Taxonomy**:
- Notes progress from simple to complex
- Questions test different cognitive levels
- Clear learning progression

✅ **Comprehensive Coverage**:
- All major concepts addressed
- Logical flow and organization
- Examples and applications included

✅ **Assessment Quality**:
- Clear, unambiguous questions
- Plausible distractors
- Explanations for answers
- Mixed difficulty levels

✅ **Adaptive Learning**:
- 70% passing threshold
- Feedback identifies weak areas
- Recommendations for improvement
- Retake support offered

---

## 💡 Troubleshooting

**Q: The AI doesn't seem to follow the instructions**
- Make sure `CLAUDE.md` and `Skill.md` are loaded in the AI's context
- Restart the AI assistant and reload the files

**Q: Output quality is poor**
- Ensure you're using a capable AI model (Claude Sonnet 4.5 or similar)
- Check that the instruction files are being read properly

**Q: Files aren't being created**
- Verify the AI assistant has file write permissions
- Check the working directory path

---

## 📞 Project Information

**Student**: zhdwalayat
**Repository**: https://github.com/zhdwalayat/AIDD
**Date**: December 31, 2025
**AI Model Used**: Claude Sonnet 4.5

---

## 🎓 Expected Outcome

After running this system with your own topic, you should have:

1. **Well-organized directory** with all materials
2. **Comprehensive notes** (1000-5000 words depending on complexity)
3. **Effective flash cards** (8-25 cards)
4. **Quality assessment quiz** (10-20 questions)
5. **Professional documentation** with proper formatting

**The output quality should match the Spec-Kit-Plus example included in the repository.**

---

## ✨ What Makes NOTE-X Special

1. **Pedagogically Sound**: Based on Bloom's Taxonomy and mastery learning principles
2. **Adaptive**: Adjusts to user performance with personalized feedback
3. **Scalable**: Works for any topic in any domain
4. **Professional**: Academic rigor with proper documentation
5. **Automated**: Generates complete study packages in minutes
6. **Quality-Controlled**: Multiple validation mechanisms ensure excellence

---

**Ready to test? Follow the steps above with any topic of your choice!**
