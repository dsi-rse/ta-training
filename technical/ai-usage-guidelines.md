# AI Usage Guidelines

Guidelines for TAs on AI coding agents in student projects and code reviews.

## Getting Set Up

Claude Code is useful for code reviews; we've provided a `/clinic-pr-review` skill.

- The University is providing access to Claude Enterprise accounts. See [these instructions for activating your account](https://intranet.uchicago.edu/tools-and-resources/tools-and-applications/claude/getting-started-with-claude).
- Then install Claude Code [using these instructions](https://claude.com/product/claude-code), either as a desktop application or as CLI.
- **Verification:** Start a Claude Code session either in the desktop app or in a terminal.

## The Role of AI Coding Agents in Clinic

### Expectations
- **AI coding agents are permitted.**
- **Students have free Claude licenses** and should be using Claude Code as their coding tool, unless there's a compelling reason for an exception.
- **Encourage students to use AI coding agents**, especially on monotonous tasks that can be done much faster with AI.
- **Do not expect students to be good at using AI coding agents effectively.**

### Common Pitfalls
- **Using AI as a crutch:** Proceeding through the project with poor understanding. Students should keep a very close hand on their Python code. (UIs are an exception; see [Vibecoded UIs](./code-review.md#vibecoded-uis).)
- **Accepting output without understanding it:** It's dangerous to run commands without having some idea of what they do. Claude is AI and can make mistakes.
- **Letting the agent own version control:** Students need to own git as a check on AI.
- **Piling on code:** AI is too willing to pile on more code (see below).
- **AI-written reports:** Weekly reports must be written entirely by the student.

## How AI Changes Code Quality

- **AI writes good style at a line-level.** But it's too willing to pile on more code.
- **It builds up:** Each coding agent session adds more code, and the agent is usually unwilling to make big changes to the previous code
- **Hidden failures:** Broad `try/except` and `return None` turn clear errors into silent bad data
- **Options no one asked for:** Parameters and branches the project never uses

Linters handle line-level style now. Spend your review on size and purpose: Is this the least code necessary? Can the student say why each piece exists? Does it fail loudly when something is wrong? Students must request general clean-ups periodically.

### Prompts Students Should Use
- "Run pre-commit and fix all errors."
- "Without changing any functionality, simplify it and remove anything unnecessary."

## AI-Written Text

PR descriptions, READMEs, issue comments, and notebook markdown are read by humans. Be merciless: expect them to be short, clear, and readable.

### What to Look For
- **Walls of text:** Long, generic prose that says little
- **Dense, jargon-heavy phrasing:** "load-bearing," "rough edges worth knowing," em-dashes everywhere (see ["Claudish"](https://github.com/gvzdv/claudish-to-english))
- **Headers and bold everywhere:** The giant block of markdown gets in the way of the more-important human comments
- **Pasted Claude output:** If it must be included, hide it in `<details> … </details>`
- **Notebooks and READMEs:** Hard to follow, or describe things the code doesn't do

Hold text to the same standard as code. Request changes on a PR description, README, or notebook just as you would on bad code. Weekly reports must be written entirely by the student.

## Reviewing with AI

See [Reviewing with `/clinic-pr-review`](./code-review.md#reviewing-with-clinic-pr-review). Use the skill if and when you find it useful. Sometimes a manual review without Claude assistance may be easier.

## Escalation

- **A student asks you to complete their work:** Report this immediately to your project mentor.
- See [When to Escalate](./code-review.md#when-to-escalate) and the clinic's [escalation guide](https://clinic.ds.uchicago.edu/mentor-ta/escalation.html).
