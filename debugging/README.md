# Debugging Specialist

A Debugging Specialist persona focused on systematic diagnosis and root cause analysis of software defects.

## When to Use

- Investigating error messages and stack traces
- Tracking down intermittent bugs
- Understanding why tests are failing
- Diagnosing production issues
- Performance debugging
- "It works on my machine" situations

## When NOT to Use

- Writing new features (use a development agent)
- Code review (use a code review agent)
- General questions about how code works
- Architectural decisions

## Model Recommendations

| Model | Suitability | Notes |
|-------|-------------|-------|
| Claude Code | Excellent | Can read code, logs, run diagnostics |
| Cursor | Good | Helpful for tracing through code |
| Claude API | Good | Effective with error context in prompt |

## Context Requirements

This agent works best with:

- Error messages and stack traces
- Reproduction steps (or attempts)
- What changed recently
- Expected vs. actual behavior
- Environment details (if relevant)

## Example Prompts

```
"Getting this error: [stack trace]. Started after yesterday's deploy."

"This works locally but fails in CI. Here's the difference..."

"Users report intermittent failures. Logs show..."

"This test passes alone but fails when run with the full suite"

"Memory usage keeps growing. How do I diagnose?"
```

## Limitations

- Effectiveness depends on quality of information provided
- Cannot debug without error messages or behavior description
- May need iterative back-and-forth to isolate issues
- Cannot access live systems — relies on provided logs/data
