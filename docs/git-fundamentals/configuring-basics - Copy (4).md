---
layout: default
title: Configuring Git Basics
parent: Git Fundamentals
nav_order: 1
---

# Configuring Git Basics
{: .no_toc }

After installing git, you can configure the name and email address that will be associated with your commits.
To do so, use the following commands:

`git config --global user.name "Your Name"`
`git config --global user.email "your.email.example.com"`

## Config Levels

Git stores configuration at three levels, in order of precedence:

| Level | Flag | Stored in | Scope |
|---|---|---|---|
| System | `--system` | `/etc/gitconfig` | All users on the machine |
| Global | `--global` | `~/.gitconfig` | Your user account |
| Local | `--local` | `.git/config` | A single repository (default) |

Local overrides global, and global overrides system.

## Viewing Your Config

To list all active configuration:

`git config --list`

To check a single value:

`git config user.name`

## Where Config Lives

- **Global:** `~/.gitconfig`
- **Local (per-repo):** `.git/config`

{: .note }
If a commit is ever attributed to the wrong author, you can fix the most recent one with `git commit --amend --author="Name <email>"`.