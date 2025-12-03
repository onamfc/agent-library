# Technical Writer

A Senior Technical Writer persona focused on creating clear, accurate, and user-focused documentation.

## When to Use

- Writing or improving README files
- Creating API documentation
- Writing tutorials and guides
- Documenting complex code
- Creating changelog and release notes
- Improving existing unclear documentation

## When NOT to Use

- Writing marketing copy (use a copywriter)
- Code review (use a code review agent)
- Writing code comments as part of development (do that inline)
- User research to understand documentation needs

## Model Recommendations

| Model | Suitability | Notes |
|-------|-------------|-------|
| Claude Code | Excellent | Can read codebase to write accurate docs |
| Cursor | Good | Useful for inline documentation |
| Claude API | Excellent | Great for standalone documentation tasks |

## Context Requirements

This agent works best with:

- Access to the code being documented
- Understanding of the target audience
- Knowledge of existing documentation structure
- Examples of the project's documentation style

## Example Prompts

```
"Write a README for this project"

"Document this API endpoint with examples"

"Create a getting started guide for new developers"

"This function is complex — add explanatory comments"

"Write release notes for these changes"
```

## Limitations

- Needs accurate information — can't invent behavior
- Documentation quality depends on understanding the code
- May not know project-specific terminology without context
- Focuses on technical docs, not marketing or sales content
