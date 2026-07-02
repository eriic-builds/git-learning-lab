# Git Learning Lab

> A hands-on lab for learning **Git, GitHub, and the GitHub Copilot CLI** — built for
> people who are **not** developers. Play in a safe sandbox, then let Copilot do the typing.

**Live guide:** https://eriic-builds.github.io/git-learning-lab/

The guide is one self-contained HTML page — no build step, no dependencies. Open it in a
browser or read it online. This repo also ships a **practice sandbox** you can't break.

---

## What's in it for you

You keep hearing that git and GitHub are essential — but every tutorial assumes you already
write code. This one doesn't. Work through it and you get:

- **Version control that saves you.** Every change is recorded. You can always return to a
  version that worked — no more `final_v3_REALLY_final.docx`.
- **Confidence to experiment.** Branches let you try ideas without touching the good copy.
- **A real public presence.** Your work lives on GitHub: shareable, backed up, visible.
- **Copilot does the typing.** Once you know the moves, the CLI runs them for you from a
  plain-English prompt — and always asks before it changes anything.

> **The promise:** go from *"what is a commit?"* to *opening a pull request* — and then
> hand the busywork to GitHub Copilot CLI. No prior coding required.

**Cost if you skip it:** copying folders to "back up", losing the version that worked, and
being locked out of the tool the whole software world collaborates on.

---

## What you'll be able to do

By the end you can confidently:

- Explain a **repo**, **commit**, **remote**, **push/pull**, and **branch** in plain English.
- Run the everyday loop: **edit → add → commit → push**.
- Undo mistakes safely.
- Create a branch, merge it, and open a **pull request**.
- Ask **GitHub Copilot CLI** to do all of the above for you.

**The one mental model:** a *commit* is a labelled snapshot; *GitHub* is the shared copy of
your project; a *branch* is a safe sandbox to try things before they join `main`.

---

## The guide

Open **[`docs/index.html`](docs/index.html)** (or the [live page](https://eriic-builds.github.io/git-learning-lab/)).
It covers nine short sections:

| # | Section | You learn to |
| --- | --- | --- |
| 00 | Mental model | Speak git: repo, commit, remote, push/pull, branch |
| 01 | Setup | Install git, sign in to GitHub, stamp your name on commits |
| 02 | Everyday loop | clone, status, add, commit, push, pull |
| 03 | Undo mistakes | restore, amend, revert — safely |
| 04 | Branches & merges | Work in a sandbox, then fold it back in |
| 05 | Pull requests | Propose and review a change on GitHub |
| 06 | Copilot CLI | Drive all of it with plain-English prompts |
| 07 | Practice lab | Do it for real in the `practice/` sandbox |
| 08 | Project workflow | Run a real project with GitHub flow: issue → branch → PR → merge |
| 09 | Gotchas | Sidestep the traps that trip up newcomers |

Every command block has a **Copy** button, and there are three reading modes
(Light, Dark, and a dyslexia-friendly Reading mode). The Practice lab and Project
workflow sections include **Windows PowerShell terminal "screenshots"** so you can
see exactly what each command should look like as you follow along.

---

## Practice and prove it

Reading isn't learning — **doing** is. The **[`practice/`](practice/)** folder is a safe
sandbox with a throwaway file and a guided walkthrough. The Practice lab section of the
guide adds **try-it-yourself steps** with expandable reveals — attempt each command first,
then open the reveal to check your approach and learn *why* it works.

```bash
git clone https://github.com/eriic-builds/git-learning-lab.git
cd git-learning-lab/practice
# then follow exercises.md
```

You'll run four exercises: your first commit → a branch and merge → your first pull request
→ then the same again, this time by asking **Copilot CLI**.

**Before you're done, can you:**

- [ ] Explain *commit*, *push*, and *branch* in one sentence each?
- [ ] Run **edit → add → commit → push** from memory?
- [ ] Create a branch, merge it, and open a pull request?
- [ ] Ask Copilot CLI to do the same — knowing it asks before it acts?

---

## Who this is for

- Admins and IT pros who touch GitHub but never learned git properly.
- Writers, PMs, and anyone who wants version control without a CS degree.
- Complete beginners who want a safe place to practice.

> You don't need to be a developer. You need a terminal and a few minutes.

---

## Grounding and disclaimer

Commands are grounded in the official **Git** and **GitHub Copilot CLI** documentation, and
tested by running them.

> **Unofficial community resource. Not affiliated with GitHub or Microsoft.**

**Sources**

- Git documentation — https://git-scm.com/doc
- GitHub Docs, Using GitHub Copilot CLI — https://docs.github.com/copilot/how-tos/use-copilot-agents/use-copilot-cli
- GitHub Docs, Installing GitHub Copilot CLI — https://docs.github.com/copilot/how-tos/set-up/install-copilot-cli

---

## Why I built this

I learned git by *doing* it — installing it, making my first commit, and shipping a real
page. This lab is that experience, packaged so I can keep practicing and so anyone visiting
my GitHub can learn the same way: a little theory, then straight into the sandbox.
