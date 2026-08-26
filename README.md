# tensorplay-app

Personal playground for training loop tricks

## How to use

```bash
python train.py --epochs 5 --synthetic
# metrics land in runs/metrics.csv
```

## What it does

- Cosine LR schedule with warmup
- Metrics logged to CSV for plotting
- Gradient clipping and clean metrics logging
- Single file model definition, easy to hack
- Synthetic dataset mode: no download needed to smoke-test

## Getting started

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── SECURITY.md
├── model.py
├── requirements.txt
└── train.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT licensed, see LICENSE.
