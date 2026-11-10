# Contributing

Arkytas repositories are maintained by the founding team. We will open them to outside contributions later.

## Workflow

- Branch from `main` and open a pull request. Merge only with green CI; never force-push `main`.
- Keep pull requests small and focused; write commit messages in the imperative ("Add BOM check").
- Tag releases and write short release notes.

## Never commit

- Secrets, tokens or `.env` files.
- Datasets, checkpoints or model weights: they belong in private Hugging Face repos.
- Single files over 50 MiB.

## Data and models

- Create every Hugging Face repo as private first and push with `private=True`.
- Pin datasets and models to a tag or commit SHA, never `main`.
- Report evaluation results as k/n per condition with intervals, seen and unseen conditions separately.
