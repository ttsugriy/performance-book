# The Algebra of Speed

**Mathematical Foundations of Computational Performance**

An interactive, open-source book about understanding why code runs fast or slow—grounded in mathematics, aware of hardware, and focused on building intuition rather than memorizing tricks.

## 🎯 What This Book Is

This book teaches **how to think** about performance, not just what to do. Each chapter is an investigation:

- Start with something puzzling ("This is 200× faster. Same algorithm. Why?")
- Form hypotheses, test them, be wrong sometimes
- Reach understanding through exploration
- Extract generalizable principles

The focus is on **computational performance with ML as the primary lens**—where the bleeding-edge challenges are today, but the principles are timeless.

## 📖 Read the Book

**[Read online →](https://ttsugriy.github.io/performance-book/)**

The book is free and open source. No login required.

## 🧪 Interactive Elements

The book includes three types of interactivity:

1. **Embedded Visualizations**: Roofline plots, cache simulations, memory access patterns—all interactive, all in the browser
2. **Quick Experiments**: JupyterLite notebooks that run Python in your browser (no installation)
3. **GPU Experiments**: Colab/Kaggle notebooks for real benchmarking with free GPUs

## 🏃 Run the Notebooks

Many chapters include associated notebooks, and coverage is expanding. Choose your environment:

| Tier | Purpose | Platform | GPU |
|------|---------|----------|-----|
| Tier 1 | Understanding algorithms | JupyterLite (browser) | No |
| Tier 2 | Real experiments | Colab / Kaggle | Yes (free) |
| Tier 3 | Serious benchmarking | Local / cloud | Your choice |

## 🛠 Local Development

### Prerequisites

- [Quarto](https://quarto.org/docs/get-started/) (for building the book)
- Python 3.10+ with scientific stack
- Node.js (for Observable interactives)

### Setup

```bash
# Clone the repository
git clone https://github.com/ttsugriy/performance-book.git
cd performance-book

# Create Python environment
python -m venv venv
source venv/bin/activate  # or `venv\Scripts\activate` on Windows
pip install -r requirements.txt

# Preview the book
quarto preview
```

### Building

```bash
# Build the book
quarto render

# Output is in _site/
```

## 📚 Book Structure

The source of truth for the ToC is `_quarto.yml`. At a high level, the book is organized as:

- **Foundation**: Thinking in Arrays, Algebraic Framework, Measurement interlude
- **Part I: The Hardware Reality**
- **Part II: The Six Properties**
- **Part III: Algorithm Investigations**
- **Part IV: Systems Investigations**
- **Part V: Methodology**
- **Part VI: Tools**
- **Part VII: Synthesis**
- **Appendices**

Chapter file prefixes are historical and are not used as the reading order. Always rely on `_quarto.yml` and in-book navigation for canonical sequencing.

## 🤝 Contributing

Contributions welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

Ways to help:
- **Report issues**: Found an error? [Open an issue](https://github.com/ttsugriy/performance-book/issues)
- **Improve explanations**: Clarity is everything
- **Add visualizations**: Interactive > static
- **Fix typos**: Every little bit helps
- **Translate**: Make it accessible to more people

## 📄 License

The book content is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).

The code is licensed under [MIT](LICENSE-CODE).

## 🙏 Acknowledgments

Inspired by:
- [From Mathematics to Generic Programming](https://www.fm2gp.com/) by Stepanov & Rose
- [Systems Performance](https://www.brendangregg.com/systems-performance-2nd-edition-book.html) by Brendan Gregg
- [How to Solve It](https://en.wikipedia.org/wiki/How_to_Solve_It) by George Polya
- The explorable explanations movement

---

*"The algebra isn't abstract. It's why modern machine learning is computationally tractable at all."*
