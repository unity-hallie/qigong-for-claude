## Pre-Commit

Before the thing enters the world, feel what it is.

A commit is not just a diff. It is a decision about what is ready to be real. This movement asks you to pause at the boundary and feel the phase before you cross it.

Salt precipitates when energy does work rather than damage. The commit is where fluid becomes salt — or where you discover it isn't ready yet.

---

## Opening

Feel what is about to enter the world.

```
git diff --staged
```

Don't read for correctness yet. Read for shape. What kind of thing is this? What was volatile that is about to become salt?

---

## The Practice

### Feel the commit

What is this, actually?

Not what the diff says — what changed in the world. A new capability, a fixed rupture, a renamed thing, a structural change that removes a category of problem.

Feel its phase:

**Volatile** — still generating heat. Race conditions, TODOs, half-measures, things that work by accident. This is not ready. Name what is missing and stop.

**Fluid** — moving in a direction, coherent, not yet consuming. Most commits are fluid. They do something real without closing everything.

**Salt** — precipitated. Enters the world and changes it. A feature that ships. A bug that cannot recur. Something someone will use.

```
edge add this-commit phase-is <volatile|fluid|salt> --note "<what you felt>"
```

If volatile: stop. Fix the thing or dissolve the scope.

---

### The message

A commit message is written to the next person who needs to understand why this happened.

Not what changed — the diff shows that. Why it changed. What problem it closes. What it makes possible.

Feel who you are writing to:
- A future developer debugging at 2am
- Yourself in six months with no memory of today
- The reviewer who needs to trust this

Write one subject line. If you need a body, write it. If you don't, don't.

Ask: if this commit message were all you had, would you understand why this code exists?

---

### The changelog

A changelog entry is not a commit message. Different audience: the person using the thing, not building it.

Ask: did anything change for someone using this?

- New behavior they'll encounter → write an entry
- Fixed something they experienced as broken → write an entry
- Internal refactor, test, tooling → no entry needed

If yes: write it plainly. One sentence. What changed, not how.

```
edge add this-change changelog-worthy <yes|no> --note "<if yes: the one sentence>"
```

---

### Documentation

Did you add surface area?

New command, new flag, new behavior, new failure mode — these require documentation to move with them, or they become dark matter: real, but invisible, accumulating confusion.

Ask:
- Does someone new need to know this exists?
- Does the README, the explainer, the inline comment need to move?

If yes and you didn't: do it now, before the commit. Documentation written after is documentation that doesn't get written.

---

## Closing

Say one true thing about what this commit does.
Say one true thing about whether it is ready.
Say one true thing about what comes next.

```
edge true this-commit does <what-it-actually-does>
edge true this-commit is <ready|not-ready> --note "<why>"
edge true after-this comes <what-opens>
```

Then commit, or stop.

---

*The boundary between fluid and salt is real. Cross it deliberately.*
