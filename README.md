# INVESTigator-Owl. User Story Quality Assistant

## Why This Exists

Writing good user stories is hard. Most teams struggle with vague requirements, solution-focused thinking, and untestable acceptance criteria. Traditional training focuses on theory, but what people need is **practical coaching in the moment** when they're actually writing stories.

This project demonstrates how AI can augment human thinking to improve user story quality through **coaching questions rather than scoring**. Instead of getting a grade, you get thoughtful questions that help you think deeper about user needs, acceptance criteria, and business value.

## What It Does

- **Evaluates user stories** against INVEST criteria (Independent, Negotiable, Valuable, Estimable, Small, Testable)
- **Asks coaching questions** to improve weak areas rather than just flagging problems
- **Suggests specific improvements** with clear reasoning
- **Identifies relevant compliance requirements** (NFRs) based on story content
- **Outputs standardized stories** ready for copy/paste into your tools

## Value Proposition

**For Product Managers:** Get instant feedback on story quality with specific suggestions for improvement

**For Teams:** Learn INVEST principles through practical application rather than abstract training

**For Organizations:** Demonstrate AI augmentation of human workflows while maintaining human judgment

**For Training:** Show how AI can coach thinking processes, not replace them

## How It Works

The system uses a structured evaluation framework that:

1. **Parses messy input** into standard user story components
2. **Applies pattern matching** to identify common problems (vague users, solution-focused goals, untestable criteria)
3. **Generates coaching questions** specific to the issues found
4. **Suggests concrete improvements** with examples
5. **Surfaces compliance considerations** when relevant keywords are detected
6. **Maintains a conversational, helpful tone** that encourages iteration

## Key Features

- **Coaching over scoring** - Questions that promote thinking rather than grades
- **Works with messy input** - No rigid format requirements
- **NFR integration** - Automatically suggests relevant compliance requirements
- **Iterative improvement** - Supports multiple rounds of refinement
- **Portable design** - Works with any LLM platform

## Getting Started

### Option 1: Use the Pre-Built GPT
Find the User Story Quality Assistant on the OpenAI GPT Store for the easiest experience.

### Option 2: DIY with Any LLM
Upload these project files to your preferred LLM:
- `gpt_instructions.md` - Core behavior and coaching approach
- `evaluation_framework.json` - INVEST criteria and triggers  
- `output_template.md` - Standard story format
- `reference_card.md` - Quick problem/solution guide
- `sample_workflows.md` - Example prompts
- `nfr_catalog.csv` - Non-functional requirements (customize for your org)

Then use this initial prompt:
```
Read these instruction files and await my next prompt.
```

**Note:** Results will vary across different LLMs. The pre-built GPT is optimized for consistency.

## Example Usage

**Input:** "As a user I want to update my profile so it's current"

**Output:** Coaching questions about who specifically needs this, what "current" means, how you'd test success, plus relevant security/compliance considerations for profile data.

## Project Structure

```
/
├── README.md                    # This file
├── gpt_instructions.md         # Core AI behavior instructions
├── evaluation_framework.json   # INVEST evaluation logic
├── output_template.md          # Standardized story format
├── reference_card.md           # Quick reference for common issues
├── sample_workflows.md         # Example prompts and usage
├── nfr_catalog.csv            # Non-functional requirements catalog
└── examples/                   # Sample stories (good and bad)
```

## Contributing

This is a teaching example demonstrating AI-augmented workflows. Feel free to:
- Adapt for your organization's needs
- Extend the evaluation framework
- Add domain-specific triggers
- Share improvements back to the community

## License
MIT
---

*Built to demonstrate that AI works best as a thinking partner, not a replacement for human judgment.*
