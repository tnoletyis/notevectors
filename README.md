# notevectors

Tiny embedding search: numpy cosine over cached vectors

Built for my own use; public in case it helps someone.

## What it does

- Reranks by recency when scores tie
- Interactive REPL and one-shot modes
- Vectors cached to .npy so re-runs are instant
- sentence-transformers when available, TF-IDF fallback

## Install

```bash
pip install -r requirements.txt
```

## Examples

```bash
python search.py ./notes
>> how do I back up my database?
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── pull_request_template.md
├── docs/
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
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

## Known issues

- none reported yet (surprisingly)

## License

MIT. Do whatever you want.
