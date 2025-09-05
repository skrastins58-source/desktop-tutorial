# 🤖 Copilot Instructions for Desktop Tutorial

This file provides setup instructions, coding standards, and project structure guidance for the GitHub Copilot coding agent.

## 🏗️ Project Structure

```
desktop-tutorial/
├── README.md              # Project overview and usage guide
├── Day.txt                # Python script for GCP instance management
├── test_Day.txt           # Test file (currently empty)
├── .github/               # GitHub configuration and templates
│   ├── copilot-instructions.md
│   └── ISSUE_TEMPLATE/
│       └── copilot-task.yml
└── docs/                  # Documentation
    └── agent-guide.md
```

## 🛠️ Build and Test Commands

This is a simple Python tutorial project. Common commands:

```bash
# Run the main Python script
python3 Day.txt

# Check Python syntax
python3 -m py_compile Day.txt

# Run basic tests (if implemented)
python3 -m unittest discover -s . -p "test_*.py"
```

## 📏 Coding Standards

### Python Code Style
- Follow PEP 8 style guidelines
- Use descriptive variable names
- Add docstrings to functions
- Handle exceptions appropriately
- Use type hints where beneficial

### File Naming
- Python files: use `.py` extension (not `.txt`)
- Test files: prefix with `test_`
- Documentation: use `.md` for Markdown files

### Code Structure
- Keep functions focused and small
- Separate concerns appropriately
- Add comments for complex logic
- Use meaningful commit messages

## 🎯 Project Context

This is a GitHub Desktop tutorial repository that contains:
- A Python script demonstrating GCP Compute Engine instance management
- Basic project structure for learning GitHub workflows
- Examples of subprocess usage and error handling

## ⚠️ Important Notes

1. **File Extensions**: The main Python code is currently in `Day.txt` - this should ideally be renamed to `Day.py` for proper Python recognition
2. **Dependencies**: The script uses `gcloud` CLI tool and requires proper GCP authentication
3. **Testing**: Test infrastructure is minimal - focus on basic functionality tests
4. **Documentation**: Keep documentation simple and tutorial-focused

## 🔧 Common Tasks for Agent

- Improve Python code structure and error handling
- Add proper unit tests
- Enhance documentation
- Fix code style issues
- Add type hints and docstrings
- Improve project organization

## 🚫 Avoid

- Breaking the tutorial nature of the repository
- Adding complex frameworks or dependencies
- Over-engineering simple examples
- Removing educational comments or examples