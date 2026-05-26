# Contributing to AI Infrastructure Engineer Learning Path

Thank you for your interest in contributing! This document provides guidelines for contributing to this project.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Contribution Guidelines](#contribution-guidelines)
- [Style Guidelines](#style-guidelines)
- [Commit Message Guidelines](#commit-message-guidelines)
- [Pull Request Process](#pull-request-process)
- [Community](#community)

---

## Code of Conduct

This project adheres to a Code of Conduct that all contributors are expected to follow. Please read [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md) before contributing.

**In short:**
- Be respectful and inclusive
- Welcome newcomers
- Focus on constructive feedback
- Assume good intentions

---

## How Can I Contribute?

### 🐛 Reporting Bugs

Found a bug? Help us fix it!

**Before submitting:**
- Check if the issue already exists
- Verify it's not listed in known issues
- Test with the latest version

**Submit a bug report:**
1. Use the bug report template
2. Provide clear title and description
3. Include steps to reproduce
4. Add error messages or screenshots
5. Specify your environment (OS, Python version, etc.)

### 💡 Suggesting Enhancements

Have an idea to improve the curriculum?

**Submit an enhancement:**
1. Check if it's already suggested
2. Use the feature request template
3. Explain the use case
4. Describe the proposed solution
5. Consider implementation complexity

### 📚 Improving Documentation

Documentation improvements are always welcome!

**Areas to contribute:**
- Fix typos or unclear explanations
- Add more examples
- Improve code comments
- Translate to other languages
- Add diagrams or visualizations

### 🧪 Adding Exercises

Help learners practice more!

**Exercise guidelines:**
- Should reinforce lesson concepts
- Include clear requirements
- Provide starter code
- Add solution in separate branch
- Include difficulty level

### 🎯 Creating Projects

Propose new hands-on projects!

**Project requirements:**
- Align with curriculum level
- Include comprehensive README
- Provide code stubs with TODO comments
- Add tests
- Document architecture

### ✅ Reviewing Pull Requests

Help review contributions!

**Review guidelines:**
- Be constructive and kind
- Test the changes locally
- Check for clarity and completeness
- Verify code quality
- Ensure documentation is updated

---

## Getting Started

### 1. Fork the Repository

```bash
# Click "Fork" button on GitHub
# Then clone your fork
git clone https://github.com/YOUR-USERNAME/ai-infra-engineer-learning.git
cd ai-infra-engineer-learning
```

### 2. Set Up Development Environment

```bash
# Create virtual environment
python3.11 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
pip install -r requirements-dev.txt  # Development dependencies

# Install pre-commit hooks
pre-commit install
```

### 3. Create a Branch

```bash
# Create a feature branch
git checkout -b feature/your-feature-name

# Or a bugfix branch
git checkout -b fix/bug-description
```

### 4. Make Your Changes

Follow the style guidelines below.

### 5. Test Your Changes

```bash
# Run tests
pytest

# Check code style
flake8 .
black --check .

# Validate markdown
markdownlint **/*.md
```

### 6. Commit and Push

```bash
# Stage changes
git add .

# Commit with descriptive message
git commit -m "Add: Feature description"

# Push to your fork
git push origin feature/your-feature-name
```

### 7. Create Pull Request

- Go to your fork on GitHub
- Click "New Pull Request"
- Fill out the PR template
- Link related issues
- Request review

---

## Contribution Guidelines

### Lesson Contributions

**Structure:**
- Follow existing lesson format
- Include learning objectives
- Add hands-on exercises
- Provide self-check questions
- Include summary section

**Content:**
- Use clear, concise language
- Explain concepts before showing code
- Include real-world examples
- Add diagrams where helpful
- Cite sources for statistics or quotes

**Code Examples:**
- Should be complete and runnable
- Include necessary imports
- Add inline comments
- Follow Python best practices
- Test all code before submitting

### Project Contributions

**Requirements:**
- Comprehensive README with:
  - Project overview
  - Learning objectives
  - Prerequisites
  - Setup instructions
  - Architecture diagram
- Code stubs with TODO comments
- Test files
- Documentation templates
- .env.example file

**Code Quality:**
- Type hints for function signatures
- Docstrings for all functions/classes
- Error handling
- Logging where appropriate
- Configuration via environment variables

### Documentation Contributions

**Markdown Style:**
- Use headers hierarchically (# > ## > ###)
- Add table of contents for long docs
- Use code blocks with language specifiers
- Add alt text to images
- Keep line length under 120 characters

**Content:**
- Write for beginners
- Define technical terms
- Use active voice
- Be concise
- Include examples

---

## Style Guidelines

### Python Code Style

We follow **PEP 8** with some modifications:

```python
# Use type hints
def train_model(data: np.ndarray, epochs: int = 10) -> torch.nn.Module:
    """
    Train a machine learning model.

    Args:
        data: Training data as numpy array
        epochs: Number of training epochs (default: 10)

    Returns:
        Trained PyTorch model
    """
    pass

# Use descriptive variable names
model_checkpoint_path = "/data/checkpoints"  # Good
mcp = "/data/checkpoints"  # Bad

# Add docstrings to all public functions
# Use Google-style docstrings
```

**Tools:**
- **black**: Code formatter (line length: 100)
- **flake8**: Linter
- **mypy**: Type checker
- **isort**: Import sorter

### Markdown Style

```markdown
# Use ATX-style headers

## Add blank lines around headers

Use **bold** for emphasis, *italic* for terms.

\`\`\`python
# Always specify language in code blocks
def example():
    pass
\`\`\`

- Use hyphens for unordered lists
1. Use numbers for ordered lists
```

### Documentation Style

**File naming:**
- Use lowercase with hyphens: `getting-started.md`
- Be descriptive: `aws-ml-infrastructure.md` not `aws.md`

**Structure:**
- Start with title and brief description
- Add table of contents for docs > 500 words
- Use consistent header levels
- End with "Next Steps" or "Summary"

---

## Commit Message Guidelines

We follow **Conventional Commits** specification:

### Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- **feat**: New feature
- **fix**: Bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting, no logic change)
- **refactor**: Code refactoring
- **test**: Adding or updating tests
- **chore**: Maintenance tasks

### Examples

```bash
# Feature
git commit -m "feat(module-01): Add Docker basics lesson"

# Bug fix
git commit -m "fix(project-01): Correct FastAPI endpoint validation"

# Documentation
git commit -m "docs(readme): Update installation instructions"

# With body
git commit -m "feat(module-02): Add AWS ML infrastructure lesson

- Add EC2 GPU instance configuration
- Include S3 storage best practices
- Add code examples for SageMaker

Closes #123"
```

### Best Practices

- Use imperative mood: "Add feature" not "Added feature"
- Keep subject line under 72 characters
- Capitalize subject line
- No period at end of subject
- Separate subject from body with blank line
- Wrap body at 72 characters
- Reference issues in footer

---

## Pull Request Process

### Before Submitting

- [ ] Code follows style guidelines
- [ ] All tests pass
- [ ] Documentation is updated
- [ ] Commit messages follow guidelines
- [ ] Branch is up to date with main

### PR Template

Fill out all sections:

```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Refactoring

## Testing
How was this tested?

## Checklist
- [ ] Code follows style guidelines
- [ ] Self-review completed
- [ ] Documentation updated
- [ ] Tests added/updated
- [ ] All tests pass

## Related Issues
Closes #123
```

### Review Process

1. **Automated Checks**: CI/CD runs automatically
   - Tests must pass
   - Linting must pass
   - Code coverage maintained

2. **Manual Review**: At least one maintainer reviews
   - Code quality
   - Documentation
   - Test coverage
   - Design decisions

3. **Feedback**: Address review comments
   - Make requested changes
   - Push updates to same branch
   - Respond to comments

4. **Merge**: Once approved
   - Maintainer will merge
   - Delete your branch after merge
   - Update your fork

### After Merge

- Update your fork:
  ```bash
  git checkout main
  git pull upstream main
  git push origin main
  ```

- Delete merged branch:
  ```bash
  git branch -d feature/your-feature-name
  git push origin --delete feature/your-feature-name
  ```

---

## Development Setup

### Required Tools

```bash
# Install development dependencies
pip install -r requirements-dev.txt

# Includes:
# - pytest (testing)
# - black (formatting)
# - flake8 (linting)
# - mypy (type checking)
# - pre-commit (git hooks)
# - markdownlint (markdown linting)
```

### Pre-commit Hooks

We use pre-commit to ensure code quality:

```bash
# Install hooks
pre-commit install

# Run manually
pre-commit run --all-files
```

**Hooks include:**
- trailing-whitespace: Remove trailing whitespace
- end-of-file-fixer: Ensure files end with newline
- check-yaml: Validate YAML files
- black: Format Python code
- flake8: Lint Python code
- markdownlint: Lint markdown files

### Running Tests

```bash
# Run all tests
pytest

# Run specific test file
pytest tests/test_module_01.py

# Run with coverage
pytest --cov=src tests/

# Run specific test
pytest tests/test_api.py::test_health_endpoint
```

### Building Documentation

```bash
# Preview markdown locally
# Install grip: pip install grip

# Preview README
grip README.md

# Preview in browser
grip README.md --browser
```

---

## Community

### Getting Help

- **GitHub Discussions**: Ask questions, share ideas
- **Issue Tracker**: Report bugs, request features

Real-time chat and recurring office hours are not currently scheduled. Open a Discussion if you'd like to coordinate a study group.

### Recognition

Contributors are recognized in:
- Contributors section in README
- Release notes for significant contributions
- Hall of Fame for major contributions

### Becoming a Maintainer

Active contributors may be invited to become maintainers:

**Criteria:**
- Consistent, high-quality contributions
- Good understanding of project goals
- Helpful in reviews and discussions
- Commitment to project values

**Responsibilities:**
- Review pull requests
- Triage issues
- Maintain code quality
- Help shape project direction

---

## Questions?

- Read the [FAQ](./resources/faq.md)
- Ask in [GitHub Discussions](https://github.com/ai-infra-curriculum/ai-infra-engineer-learning/discussions)
- Open an issue with "question" label

---

## License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

<div align="center">

**Thank you for contributing! 🎉**

Every contribution, no matter how small, helps make this learning resource better for everyone.

[Back to README](./README.md)

</div>
