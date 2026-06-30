# AthenaK documentation

User-facing documentation for [AthenaK](https://github.com/IAS-Astrophysics/athenak),
built with [Sphinx](https://www.sphinx-doc.org/) and the
[Furo](https://pradyunsg.me/furo/) theme. This site is intended to replace the
project's GitHub wiki.

## Building locally

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

sphinx-build -b html source build/html
```

Then open `build/html/index.html` in a browser. Alternatively, use `make html`.

## Contents

This first version covers:

- **Getting Started**: installation, requirements, download, and build instructions.
- **Quickstart**: running AthenaK for the first time.
