# Copilot Agent Contributor Guide

Welcome to the Copilot Coding Agent guide! This document helps contributors understand how to interact with the agent, delegate tasks, and review its output effectively.

---

## 🧠 What Is the Copilot Agent?

The Copilot agent is an AI assistant that helps automate coding tasks, generate documentation, review pull requests, and more. It responds to structured prompts and works best when given clear goals and context.

---

## 📝 How to Assign Tasks

Use the `copilot-task.yml` issue template to delegate tasks. Include:
- A clear task description
- Target files or directories
- Acceptance criteria
- Priority level (optional)

Example:
> Generate a test script for `Day.txt` that verifies the printed date format using Python’s `datetime` module.

---

## 🔍 Reviewing Copilot Output

When Copilot completes a task:
- Check for accuracy and completeness
- Verify formatting and naming conventions
- Run any generated code or scripts
- Leave feedback in the issue or PR

---

## 🧪 Best Practices

- Use comments like `# TODO:` or `# Write a function to...` to guide Copilot
- Keep prompts specific and scoped
- Reference existing files when possible
- Avoid vague instructions like “make this better”

---

## 🛠️ Troubleshooting

If Copilot’s output isn’t usable:
- Refine your prompt with more context
- Break large tasks into smaller ones
- Use examples or expected output formats

---

## 📂 Related Files

- `.github/copilot-instructions.md`: Setup and standards
- `.github/ISSUE_TEMPLATE/copilot-task.yml`: Task delegation template
- `docs/examples/`: Before/after samples (optional)
- `docs/faq.md`: Common questions (optional)

---

Happy contributing! 🚀