---
layout: default
title: Configuring Git Advanced
parent: Git Fundamentals
nav_order: 2
---

# Configuring Git Advanced
{: .no_toc }

Beyond your name and email, Git has a number of preferences worth setting early.

## Default Branch Name

`git config --global init.defaultBranch main`

## Default Editor

`git config --global core.editor "code --wait"`

Replace `code --wait` with your editor of choice (e.g. `nano`, `vim`).

## Line Endings

- **Windows:** `git config --global core.autocrlf true`
- **Mac / Linux:** `git config --global core.autocrlf input`

## Credential Caching

`git config --global credential.helper cache`

Use `store` to save credentials to disk, or `manager` on Windows.

## Aliases

Aliases are shortcuts for longer commands:
