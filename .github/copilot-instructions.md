# Copilot Instructions for Desktop Tutorial Repository

This repository is a GitHub Desktop tutorial with Python practice files and comprehensive Copilot support for automated tasks.

## Repository Overview

This is an educational repository designed to help users learn GitHub Desktop through hands-on practice with:
- `Day.txt`: A Python script that displays the current day and date
- `test_Day.txt`: An experimental file for practicing Git operations
- Comprehensive documentation for Copilot integration

## Copilot Guidelines

### Code Standards
- Follow Python PEP 8 style guidelines for any Python code modifications
- Use clear, descriptive variable names and add comments for complex logic
- Maintain the educational nature of example scripts - keep them simple and well-commented
- Preserve existing functionality while making enhancements

### Documentation Standards  
- Use markdown formatting consistently across all documentation
- Include emoji icons for visual clarity (🧠 🎯 📝 etc.)
- Maintain the friendly, educational tone appropriate for beginners
- Always include clear examples when explaining concepts

### File Organization
- Keep practice files (`Day.txt`, `test_Day.txt`) in the root directory
- Place comprehensive documentation in the `docs/` folder
- Use the `.github/ISSUE_TEMPLATE/copilot-task.yml` for structured task delegation
- Reference the `agent-guide.md` for contributor guidance

### Testing and Validation
- Always test Python scripts to ensure they run without errors
- Verify that any changes don't break the educational workflow
- Check that documentation links and references are working
- Use `npm test` and `python Day.txt` to validate basic functionality

### Task Delegation Best Practices
- Use the copilot-task.yml issue template for structured requests
- Be specific about target files and expected outcomes
- Include acceptance criteria for any automated tasks
- Reference existing patterns in the repository when requesting similar work

## CI Workflows

This repository includes GitHub Actions workflows that:
- Download external dependencies before firewall restrictions  
- Build and test the project across platforms
- Publish artifacts and test results

### How to Extend CI
- Add new steps using comments like `# Add code quality check here`
- Use Copilot to generate YAML for caching, deployment, or matrix builds
- Ensure any new workflows maintain cross-platform compatibility
