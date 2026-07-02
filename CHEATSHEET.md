# Cheat Sheet

Quick lookup for the commands in this lab. Full explanations live in the
[guide](https://eriic-builds.github.io/git-learning-lab/).

## Setup (once per computer)

| Command | What it does |
| --- | --- |
| `git --version` | Check git is installed |
| `git config --global user.name "Your Name"` | Set your name on commits |
| `git config --global user.email "you@example.com"` | Set your email on commits |

## The everyday loop

| Command | What it does |
| --- | --- |
| `git clone <url>` | Download a GitHub repo |
| `git status` | See what changed (run this often) |
| `git add .` | Stage all changes (or `git add file` for one) |
| `git commit -m "message"` | Save a snapshot |
| `git push` | Send commits to GitHub |
| `git pull` | Bring GitHub's commits to you |
| `git log --oneline` | See your commit history |

## Undo

| Command | What it does |
| --- | --- |
| `git restore <file>` | Discard changes to a file |
| `git restore --staged <file>` | Unstage a file (keep the change) |
| `git commit --amend -m "msg"` | Fix your last commit message |
| `git revert <commit>` | Safely cancel a pushed commit |

## Branches & PRs

| Command | What it does |
| --- | --- |
| `git switch -c <name>` | Create and switch to a branch |
| `git switch main` | Switch back to main |
| `git merge <name>` | Merge a branch into the current one |
| `git branch -d <name>` | Delete a merged branch |
| `git push -u origin <name>` | Push a branch to GitHub (then open a PR) |

## GitHub Copilot CLI

| Command | What it does |
| --- | --- |
| `npm install -g @github/copilot` | Install (needs Node.js 22+) |
| `copilot` | Start it in your repo folder |
| `/login` | Sign in to GitHub |
| `/diff` | Review your changes |
| `/pr` | Work with pull requests |
| `@file` | Point Copilot at a specific file |
| `/help` | Show all commands |
| `Esc` | Stop Copilot mid-task |
| `Shift+Tab` | Toggle plan mode |

**Plain-English prompts to try:**
- "Commit my changes with a clear message."
- "Make a branch called add-page and switch to it."
- "Push this branch and open a pull request."
- "Undo my last commit but keep the file changes."
