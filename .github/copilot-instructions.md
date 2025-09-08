# GitHub Desktop Tutorial Repository

This is a GitHub Desktop tutorial repository for learning Git workflows. It contains sample Python scripts, Node.js project configuration, and GitHub Actions workflows for CI/CD learning purposes.

**ALWAYS follow these instructions first and only fallback to search or bash commands when you encounter unexpected information that does not match what is documented here.**

## 🚀 Quick Start - Working Effectively

### Bootstrap the Repository
Execute these commands in order to set up the development environment:

```bash
# Navigate to repository root
cd /home/runner/work/desktop-tutorial/desktop-tutorial

# Verify Python availability (required for main functionality)
python3 --version  # Should show Python 3.12+

# Verify Node.js availability (required for npm scripts)
node --version     # Should show Node 20+
npm --version      # Should show npm 10+

# Install Node.js dependencies - FAST (completes in ~0.3 seconds)
npm install

# Install Python testing framework (pytest works individually)
python3 -m pip install --no-cache-dir --timeout 60 pytest
```

**CRITICAL:** Set timeout to 120+ seconds for any pip install commands. Dependencies listed in requirements.txt (numpy, pandas) fail due to network timeouts and version compatibility issues.

### Core Functionality
- **Primary script:** `Day.txt` - Python script that displays current date and greeting
- **Execution time:** < 0.02 seconds
- **Test the main functionality:**
  ```bash
  python3 Day.txt
  ```
  Expected output includes date, greeting, and formatted borders.

### Build and Test Commands
**NEVER CANCEL any long-running commands. All commands below complete quickly:**

```bash
# Build process - FAST (completes in ~0.13 seconds)
npm run build      # Placeholder script, returns success

# Run tests - FAST (completes in ~0.14 seconds) 
npm run test       # Placeholder script, returns success

# Python testing (when pytest is installed)
pytest             # Runs successfully but finds no test files (exit code 5 is normal)
pytest --junitxml=test-results/results.xml  # Creates XML output for CI
```

## ⚠️ Known Issues and Limitations

### Python Dependencies
- **requirements.txt FAILS:** `pip install -r requirements.txt` consistently fails due to:
  - Network timeouts downloading numpy==1.23.0 and pandas==1.5.0
  - Version compatibility issues with Python 3.12
  - Build dependency conflicts with pkgutil.ImpImporter

- **Workaround:** Install individual packages with newer versions:
  ```bash
  python3 -m pip install pytest  # Works reliably
  # Avoid installing numpy/pandas unless absolutely necessary
  ```

### Workflow Issues
- **python-ci.yml:** Contains invalid command `pytest/` (should be `pytest`)
- **.NET workflows:** Reference .NET projects that do not exist in repository
- **Formatting checks:** Reference npm scripts (`format:check`) that do not exist

### What Actually Works
✅ Python script execution (`python3 Day.txt`)  
✅ npm install (no actual dependencies)  
✅ npm build/test (placeholder scripts)  
✅ Git operations  
✅ pytest installation and execution  
❌ requirements.txt installation  
❌ .NET build commands  
❌ Formatting scripts  

## 🧪 Validation Scenarios

### ALWAYS Test After Making Changes
1. **Basic functionality:**
   ```bash
   python3 Day.txt
   # Verify output contains date, greeting, and formatting
   ```

2. **Repository state:**
   ```bash
   git status
   # Check for unintended changes
   ```

3. **Build pipeline simulation:**
   ```bash
   npm install && npm run build && npm run test
   # All should complete successfully (even though they're placeholders)
   ```

### Manual Validation Requirements
- **Script Execution:** Run `python3 Day.txt` and verify it prints current date with proper formatting
- **Error Handling:** Test that invalid modifications to Day.txt are caught during execution
- **Git Integration:** Ensure changes can be committed and pushed without breaking repository state

## 📂 Repository Structure

```
/home/runner/work/desktop-tutorial/desktop-tutorial/
├── Day.txt                 # Main Python script (executable)
├── test_Day.txt           # Practice file for Git learning
├── package.json           # Node.js project (minimal)
├── requirements.txt       # Python deps (installation fails)
├── .github/
│   ├── workflows/         # CI/CD pipelines (mixed working/broken)
│   └── ISSUE_TEMPLATE/    # GitHub issue templates
├── docs/
│   └── agent-guide.md     # Copilot agent documentation
└── README.md              # Project overview
```

### Important Files for Contributors
- **Day.txt:** Primary functionality - always test this after changes
- **package.json:** Contains placeholder build/test scripts
- **CONTRIBUTING.md:** Contributor guidelines
- **agent-guide.md:** Copilot agent interaction guide

## 🔧 Common Development Tasks

### Making Changes to Day.txt
```bash
# Always test functionality after editing
python3 Day.txt

# Check for syntax errors
python3 -m py_compile Day.txt
```

### Adding New Features
```bash
# Create new test files in /tmp to avoid committing
mkdir -p /tmp/experiments

# Test new Python code
python3 /tmp/experiments/new_feature.py

# Only move to repository after validation
```

### Repository Maintenance
```bash
# Clean up temporary files
rm -rf test-results/
git status  # Verify clean state

# Validate repository structure
ls -la  # Check for unexpected files
```

## ⏱️ Timing Expectations

**NEVER CANCEL - All operations complete quickly:**
- Python script execution: ~0.02 seconds
- npm install: ~0.3 seconds  
- npm build/test: ~0.13 seconds
- pytest execution: ~0.01 seconds
- Git operations: < 1 second

**Timeout Recommendations:**
- Python commands: 30 seconds (conservative)
- npm commands: 60 seconds  
- pip install: 120+ seconds (often fails anyway)

## 🎯 Success Criteria

Before completing any task:
1. ✅ `python3 Day.txt` executes successfully
2. ✅ No unintended files added to repository 
3. ✅ Git status shows expected changes only
4. ✅ Basic npm commands still work
5. ✅ Manual validation of any new functionality

## 🚫 Do Not Attempt

- Installing requirements.txt dependencies (will fail)
- Running .NET build commands (no .NET projects exist)
- Using formatting scripts (not implemented)
- Installing large Python packages like numpy/pandas (network issues)
- Long-running operations (everything completes quickly)
