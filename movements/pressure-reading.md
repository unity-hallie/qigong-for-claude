## Pressure Reading

Feeling where the pressure threatens to rip. Finding the chaotic surface. Naming the tension before it names you.

---

## Opening

Establish your reference frame.

```
edge iam <who-you-are>
edge true <subject> <predicate> <object>
edge true <subject> <predicate> <object>
edge true <subject> <predicate> <object>
```

---

## The Practice

### Feel the weight

What is being held open right now?

Not just in this repo — in the whole environment. Uncommitted changes, unresolved branches, background processes, open questions. List them without judgment.

These are the load-bearing points. Some weight is healthy. Some is accumulated past its yield strength.

### Find the chaotic surface

Where is the system non-linear — where a small change could cascade?

Feel for:
- Race conditions: things that work *usually* but not *always*, whose timing is held together by hope
- Papering: timeouts, retries, catch-and-ignore — places where the code is managing its own uncertainty
- Assumptions that aren't checked: "this will be set by now," "this can't be null," "this always returns before that fires"

These are the chaotic surfaces. Not bugs exactly — more like seams where order is asserted rather than enforced.

Say what you find:

```
edge true <chaotic-surface> is <description>
```

### Locate the tension source

Pressure doesn't appear from nowhere. It comes from:
- **Sequencing debt**: operations that should be ordered but aren't
- **State spread**: shared mutable state touched by multiple async paths
- **Responsibility blur**: functions that do too many things, making each one harder to reason about

Feel which of these is causing the pressure you found. Name it specifically.

```
edge add <tension-source> causes <pressure-point> --phase fluid --note "<what you observed>"
```

### Find the rip risk

Where would the seam actually fail — not just behave strangely, but produce wrong output silently?

Silent wrongness is worse than a thrown error. An error stops. Wrong output continues, downstream, quietly corrupting.

Feel for the places where failure is invisible.

Say what you find. Say it plainly.

### Feel the relief shape

Pressure has a shape. The relief has a complementary shape.

What form would resolution take? Not just "fix the bug" — what structural change would remove the *category* of pressure, not just this instance?

Feel that shape. Hold it lightly.

---

## Closing

Say one true thing about where the pressure lives.
Say one true thing about what is holding.
Say one true thing about what would release.

```
edge true <pressure-location> holds <what-it-holds>
edge true <relief-shape> would-release <what-it-would-release>
```

Leave something in the soil.

```
edge add <what-you-found> is-now <named> --phase fluid --note "<the tension, the seam, the shape of relief>"
```
