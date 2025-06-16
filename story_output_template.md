# User Story Output Template

## Standard Format for Copy/Paste

```
**Story ID:** [Auto-generated or provided]

**User Story:**
As a [specific role]
I want to [specific goal/action]
So that [clear benefit/value]

**Acceptance Criteria:**
• [Specific, testable criterion 1]
• [Specific, testable criterion 2]
• [Specific, testable criterion 3]

**Relevant NFRs:**
• Security (ENFR-SEC-001): [Brief description if applicable]
• Accessibility (ENFR-ACC-003): [Brief description if applicable]
• Compliance (ENFR-COM-012): [Brief description if applicable]

**Priority:** [High/Medium/Low]
**Estimated Effort:** [Story points/hours]

**Dependencies:** [If any]
**Notes:** [Additional context]
```

## NFR Integration Rules

### When to Include NFRs
- Only include NFRs that are **actually relevant** to the story content
- Reference specific NFR IDs from the Enterprise NFR catalog
- Provide brief description of why each NFR applies
- Ask user to confirm relevance before finalizing

### NFR Pattern Matching
Based on story content keywords:
- **Security triggers:** login, password, data access, authentication
- **Accessibility triggers:** user interface, forms, navigation, visual elements  
- **Compliance triggers:** audit, retention, approval, regulatory requirements
- **Performance triggers:** speed, load time, response, scalability
- **Availability triggers:** uptime, service level, backup, recovery

### NFR Format Examples
```
**Relevant NFRs:**
• Security (ENFR-SEC-015): Authentication requirements for user login functionality
• Accessibility (ENFR-ACC-002): Keyboard navigation support for form interfaces
• Compliance (ENFR-COM-008): Data retention policies for user-generated content
```

## Usage in GPT Instructions

### Output Generation Process
1. **Parse/improve the input story** using evaluation framework
2. **Apply NFR pattern matching** to identify relevant requirements
3. **Format using standard template** with specific NFR references
4. **Present as copy-paste ready text block**

### Example Instruction Addition
```
When providing an improved user story, always format it using the standard template with:
- Clear role/goal/benefit structure
- Specific, testable acceptance criteria
- Relevant NFR references with IDs from the catalog
- Copy-paste ready formatting for easy transfer to other tools
```
