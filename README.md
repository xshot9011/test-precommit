# HEADER 1

## About this doc

- This text is based on the Mac OS operating system.
- This provides you a chance to protect your git repository against credential leaks.

## Pre-commit

### Installation

```bash
brew install pre-commit
# To verify
pre-commit --version
```

### File structure

The behavior of pre-commit is determined by the file '.pre-commit-config.yaml' in your repository.

```bash
.
├── .git
└── .pre-commit-config.yaml
```

If you commit the code and the hook validation fails, the commit will fail.

### Automatically Enabling Pre-commit on Repositories

```bash
git config --global init.templateDir ~/.git-template
pre-commit init-templatedir ~/.git-template
```
