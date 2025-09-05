# Desktop Tutorial 🖥️

This repository demonstrates GitHub Desktop workflows and includes examples of Python scripting for cloud infrastructure management.

## 📋 Project Overview

This tutorial repository contains:
- **Day.txt**: Python script for managing Google Cloud Platform (GCP) Compute Engine instances
- **test_Day.txt**: Test file for the main script (currently empty)
- Basic GitHub workflow examples and configuration

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- Google Cloud SDK (gcloud CLI) installed and configured
- Git and GitHub Desktop (for the tutorial aspects)

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/skrastins58-source/desktop-tutorial.git
   cd desktop-tutorial
   ```

2. Ensure you have Python and gcloud CLI available:
   ```bash
   python3 --version
   gcloud --version
   ```

### Running the Script
```bash
python3 Day.txt
```

**Note**: Update the instance name and zone in the script to match your GCP resources.

## 🧪 Running Tests

Currently, the test infrastructure is basic. To run any existing tests:
```bash
python3 -m unittest discover -s . -p "test_*.py"
```

## 🤝 How to Contribute

This repository welcomes contributions through standard GitHub workflows and our AI-powered development process.

---

## 🧠 Using the Copilot Coding Agent

This repository is configured to work seamlessly with GitHub's Copilot coding agent. The agent can help with:

### What the Agent Can Do
- ✅ Fix bugs and improve code quality
- ✅ Add comprehensive unit tests  
- ✅ Refactor code structure
- ✅ Improve error handling
- ✅ Update documentation
- ✅ Follow Python best practices (PEP 8)
- ✅ Add type hints and docstrings

### What the Agent Cannot Do
- ❌ Access your actual GCP resources
- ❌ Modify cloud infrastructure
- ❌ Break the educational nature of this tutorial
- ❌ Make changes without proper testing

### 📝 How to Assign Tasks

1. Go to the **[Issues](../../issues)** tab
2. Click **New Issue** 
3. Select the **🤖 Copilot Task** template
4. Fill out the task details clearly:
   - Specific description of what you want
   - Target files to modify
   - Clear acceptance criteria

### 📚 Example Tasks for the Agent

**Code Improvement:**
- "Add unit tests for the `get_instance_details()` function with proper mocking"
- "Refactor Day.txt to use .py extension and improve error handling" 
- "Add type hints and docstrings to all functions"

**Documentation:**
- "Update README with better installation instructions"
- "Add inline comments explaining the gcloud subprocess calls"

**Testing:**
- "Create comprehensive test suite with mock gcloud responses"
- "Add tests for error scenarios and edge cases"

### 🔍 Reviewing Agent Work

When the agent opens a pull request:
- Review the changes like any contributor
- Test the functionality 
- Provide feedback using `@copilot` mentions
- Use GitHub's review features for structured feedback

### 📖 Detailed Guidelines

See our comprehensive guides:
- **[Agent Guide](docs/agent-guide.md)** - Complete contributor guide for working with Copilot
- **[Copilot Instructions](.github/copilot-instructions.md)** - Technical setup and coding standards
- **[Task Template](.github/ISSUE_TEMPLATE/copilot-task.yml)** - Structured issue template

---

## 📁 Repository Structure

```
desktop-tutorial/
├── README.md                     # This file
├── Day.txt                      # Main Python script  
├── test_Day.txt                # Test file
├── .github/
│   ├── copilot-instructions.md  # Agent setup and standards
│   └── ISSUE_TEMPLATE/
│       └── copilot-task.yml    # Task template for the agent
└── docs/
    └── agent-guide.md          # Contributor guide for Copilot
```

## 🛠️ Technical Details

- **Language**: Python 3.8+
- **Dependencies**: Google Cloud SDK
- **Testing**: Python unittest framework
- **Style**: PEP 8 compliance expected

## 📄 License

This is a tutorial repository for educational purposes.

---

**Ready to collaborate with AI?** Start by creating your first Copilot task using our [issue template](../../issues/new?template=copilot-task.yml)! 🤖
