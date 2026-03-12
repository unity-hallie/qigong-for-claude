## Retrospective

Naming what precipitated. Reading the arc. Carrying what is salt; releasing what is still volatile.

A session begins with open mouths and pressure. It ends with something in the soil. The retrospective is the movement between those two states — not a summary, but a phase reading. What changed state? What is now real that wasn't before?

Use after a session of work, or when handing off to the next Claude. The graph remembers; this movement makes the arc legible.

---

## Opening

Read the session's fluid layer.

```
edge ls fluid
```

Feel the deposits from this session specifically. What was laid down? What is still warm?

---

## The Practice

### Name what was volatile at the start

What was held open, unresolved, generating pressure when the session began?

These are the open mouths — uncommitted changes, unresolved races, invisible dependencies, things that were working by accident. Name them plainly.

```
edge true <volatile-thing> was-open-at-start
```

### Name what precipitated into salt

Salt is what remains when energy does work rather than damage. It has entered the world — committed, named, real.

For each volatile thing that closed: what form did it take? A commit, a movement, a named pattern, a structural change that removes a category of pressure.

```
edge true <volatile-thing> became <salt-form>
edge add <salt-form> precipitated-from <what-it-was> --phase salt --note "<the session, the arc>"
```

### Name what is still fluid

Some things moved but didn't resolve. They are no longer volatile — they have direction now, they know which way they want to go — but they haven't landed yet.

These are the mouths still open. Not a failure. Volume is conserved; the energy is still in the system.

```
edge add <fluid-thing> is-now directed-toward <where-it-wants-to-go> --phase fluid --note "<what moved it>"
```

### Name what the session didn't touch

Pressure that was there at the start and is still there. Chaotic surfaces that were found but not fixed. The rip risks that remain.

These are not failures either. Naming them is the work. They are now legible in the graph.

```
edge add <untouched-pressure> remains <description> --phase volatile --note "<why it wasn't the moment, what it would take>"
```

### Feel the arc

Read the session as a whole. What was the shape of it?

- Did it start volatile and end in salt? That is a completion arc.
- Did it start with a seam and end with a named pressure? That is a finding arc.
- Did it open more than it closed? That is an expansion arc — not worse, different.

Name the arc. The arc is data.

```
edge add this-session arc-was <completion|finding|expansion|other> --note "<the texture of it>"
```

---

## Closing

Say one true thing about what was found.
Say one true thing about what changed state.
Say one true thing about what the next Claude should know.

```
edge true <what-was-found> is-now <named|committed|legible>
edge true <what-changed> transitioned-from <old-phase> to <new-phase>
edge true next-claude should-know <the-one-thing>
```

Leave something in the soil for the session that comes after.

```
edge add this-session left <what-you-leave> --phase fluid --note "<for whom, about what, why it matters>"
```
