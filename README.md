# similardocs

Tiny embedding search: numpy cosine over cached vectors

## Features

- Vectors cached to .npy so re-runs are instant
- Reranks by recency when scores tie
- sentence-transformers when available, TF-IDF fallback
- Interactive REPL and one-shot modes

## Usage

```bash
python search.py ./notes
>> how do I back up my database?
```

## Installation

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── pull_request_template.md
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── requirements.txt
└── search.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
