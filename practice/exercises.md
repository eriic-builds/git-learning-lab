# Exercises

Work through these in order. Every command can be copied from the
[live guide](https://eriic-builds.github.io/git-learning-lab/) too.

Run `git status` any time you're unsure what state you're in — it's your compass.

---

## Exercise 1 — Your first commit

**Goal:** save a change as a snapshot.

1. Open `hello.txt` in any editor and add a line, e.g. `Practiced by <your name> on <date>`.
2. See what git noticed:

   ```bash
   git status
   ```

3. Stage your change:

   ```bash
   git add hello.txt
   ```

4. Commit it with a clear message:

   ```bash
   git commit -m "Add my name to hello.txt"
   ```

5. Confirm it's recorded:

   ```bash
   git log --oneline
   ```

✅ **You did it** if `git log` shows your commit at the top.

---

## Exercise 2 — A branch and a merge

**Goal:** make a change in a safe sandbox, then fold it into `main`.

1. Create and switch to a branch:

   ```bash
   git switch -c practice-branch
   ```

2. Edit `hello.txt` again (add another line), then stage and commit:

   ```bash
   git add hello.txt
   git commit -m "Add a second line on a branch"
   ```

3. Switch back to `main` and look at `hello.txt` — your second line is **gone** here. That's
   the branch doing its job.

   ```bash
   git switch main
   ```

4. Merge your branch in:

   ```bash
   git merge practice-branch
   ```

5. Look at `hello.txt` again — your line is back. Clean up the branch:

   ```bash
   git branch -d practice-branch
   ```

✅ **You did it** if both your lines are in `hello.txt` on `main`.

---

## Exercise 3 — Your first pull request

**Goal:** propose a change on GitHub and merge it there.

> You'll need your own copy of this repo on GitHub. Either use a repo you created, or
> [fork](https://github.com/eriic-builds/git-learning-lab/fork) this one first.

1. Create a branch and make a small edit + commit (as in Exercise 2), then push it:

   ```bash
   git switch -c my-first-pr
   git add hello.txt
   git commit -m "Practice change for a pull request"
   git push -u origin my-first-pr
   ```

2. Go to the repo on GitHub. It shows a **Compare & pull request** button — click it.
3. Add a title and a short note, then **Create pull request**.
4. Read the diff (GitHub shows exactly what changed), then **Merge pull request**.
5. Back in your terminal, update your local `main`:

   ```bash
   git switch main
   git pull
   ```

✅ **You did it** if your change is merged into `main` on GitHub.

---

## Exercise 4 — Let Copilot CLI do it

**Goal:** repeat what you learned, but ask in plain English.

1. Install and start Copilot CLI in the repo folder (see section 06 of the guide):

   ```bash
   npm install -g @github/copilot
   copilot
   ```

2. Sign in with `/login` if prompted.
3. Try prompts like these — Copilot will ask permission before running anything:

   - "What changed in hello.txt since my last commit?"
   - "Make a new branch called copilot-practice and switch to it."
   - "Add my changes and commit them with a clear message."
   - "Push this branch and open a pull request."

4. Watch each command it proposes, approve the ones you understand, and reject anything you
   don't (press **Esc** to stop it and explain what you'd rather do).

✅ **You did it** if Copilot opened a PR for you — and you understood every step it took.

---

### Done?

Head back to the [checklist](https://eriic-builds.github.io/git-learning-lab/#gotchas) in the
guide and see if you can explain each idea in your own words. If yes — you've got the
fundamentals. 🎉
