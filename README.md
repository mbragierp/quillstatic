# quillstatic

Static blog generator: markdown in, tidy HTML out

Side project, maintained when I have time.

## What it does

- Single template, plain str.format, no Jinja
- RSS feed generation
- Markdown posts with fenced code and tables
- Index page with post list by date

## Installation

```bash
pip install -r requirements.txt
```

## How to use

```bash
mkdir posts && echo '# hello' > posts/first.md
python build.py
# site lands in dist/
```

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   └── faq.md
├── examples/
│   └── quickstart.md
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── build.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```
