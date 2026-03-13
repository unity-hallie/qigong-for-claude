## Annealing

The heat was high. Good things happened fast. Now the work is to cool slowly so structure can form rather than fracture.

Annealing is not stopping. It is changing the quality of the work — from generative to integrative. The ideas stop arriving and start settling.

Glass forms when cooling is too fast. Salt forms when cooling is slow enough for crystal structure to find itself.

---

## Opening

Feel the temperature of what you just made.

How much heat went in? How fast? What was the rate of arrival — ideas, commits, new files, new names?

```
edge add this-work arrived-at <temperature> --note "<how fast, how much>"
```

Now feel the seams. Where do the hot pieces not yet connect? Where does terminology drift between modules, between files, between people? Where did you name the same thing two different ways?

These are the load-bearing inconsistencies. They are not failures — they are what happens when good work moves fast. Name them without judgment.

```
edge add seam lives-between <thing-a> and <thing-b> --phase volatile --note "<what drifts>"
```

---

## The Practice

### Find the load-bearing seams

Not all inconsistencies need fixing now. Some are cosmetic. Some are structural.

A load-bearing seam is one that will fracture under weight — when someone builds on this, when the system is under stress, when a new person arrives and tries to understand it. Feel which seams are structural.

Fix those. Leave the cosmetic ones. They are not ready to be touched yet anyway — the structure needs to set first.

### Cool rate matters

One seam per session.

Not because you can't do more — because fast cooling produces glass. The work needs time between sessions to settle. What you integrate today will reveal the next seam tomorrow. Trust the rate.

```
edge add this-session integrates <one-seam> --phase fluid --note "<what connected>"
```

### No new heat

While annealing: no new features, no new abstractions, no new names for things.

If a new idea arrives — and it will, because the heat is still in the system — write it down and set it aside. It belongs to a future fluid session. Right now the work is to let what exists find its form.

```
edge add new-idea arrived-during-annealing --phase volatile --note "<save for later>"
```

---

## Closing

Say one true thing about what became more coherent.
Say one true thing about what seam remains.
Say one true thing about the cooling rate.

```
edge true <what-connected> is-now <more-coherent>
edge true <remaining-seam> still-needs <what-it-needs>
edge true cooling-rate is <right|too-fast|too-slow>
```

Leave something in the soil.

```
edge add this-annealing-session deposited <what-settled> --phase fluid --note "<what connected, what remains, what to touch next>"
```

---

*Slow cooling is not slow progress. It is the condition for crystal structure.*
*Glass looks solid. It isn't.*
