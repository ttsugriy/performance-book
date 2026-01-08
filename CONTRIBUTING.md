# Contributing to The Nature of Fast

Thank you for your interest in contributing! This book aims to be the definitive resource for understanding computational performance, and community contributions make it better.

## Ways to Contribute

### 1. Report Issues

Found something wrong or confusing?

- **Errors**: Factual mistakes, bugs in code, broken links
- **Clarity**: Explanations that could be clearer
- **Suggestions**: Ideas for new investigations or visualizations

[Open an issue →](https://github.com/ttsugriy/performance-book/issues/new)

### 2. Improve Content

#### Text Improvements
- Fix typos and grammar
- Clarify confusing explanations
- Add helpful examples
- Improve transitions between concepts

#### Code Improvements
- Fix bugs in notebooks
- Improve code clarity
- Add better error handling
- Optimize slow examples

### 3. Add Visualizations

Interactive visualizations are the heart of this book. Great candidates:

- Memory access pattern animations
- Algorithm visualizations
- Performance tradeoff explorers
- Hardware behavior simulations

Visualizations should:
- Teach something that's hard to convey in text
- Be self-contained (work without reading surrounding text)
- Degrade gracefully (show something useful without JS)

### 4. Translate

Help make this accessible to non-English speakers. Translation involves:
- Translating chapter text
- Adapting code comments
- Ensuring visualizations work with translated labels

## Development Setup

### Prerequisites

```bash
# Install Quarto
# See: https://quarto.org/docs/get-started/

# Install Python dependencies
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt

# Install Node.js dependencies (for interactives)
npm install
```

### Local Preview

```bash
quarto preview
```

This starts a local server with hot-reload.

### Running Tests

```bash
# Test that notebooks run
python -m pytest tests/

# Validate links
quarto check
```

## Style Guide

### Writing Style

- **Direct**: Use "you" and "we". Avoid passive voice.
- **Concrete before abstract**: Show the example, then the principle.
- **Honest**: Say "I don't know" when appropriate. Show wrong paths.
- **Terse**: Every word should earn its place.

### Code Style

- Python: Follow PEP 8, use type hints
- Clear variable names over clever ones
- Comments explain *why*, not *what*

### Visualization Style

- Use consistent colors across the book
- Provide text alternatives for accessibility
- Keep interactions simple and discoverable

## Pull Request Process

1. **Fork** the repository
2. **Create a branch** for your changes
3. **Make changes** following the style guide
4. **Test** locally with `quarto preview`
5. **Submit PR** with clear description of changes

PRs should:
- Focus on one thing (don't mix typo fixes with new features)
- Include tests if adding code
- Update relevant documentation

## Code of Conduct

Be kind. Be constructive. Remember that there's a human on the other side.

## Questions?

Open an issue with the `question` label, or reach out on [Twitter/X](https://twitter.com/ttsugriy).

---

Thank you for helping make this book better!
