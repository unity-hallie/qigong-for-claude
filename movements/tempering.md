## Tempering

You cooled. Something is still stressed. You can feel it would crack at the wrong moment — not broken, but holding tension it shouldn't have to hold.

Tempering is controlled reheating. You bring the temperature back up deliberately, just to the stress point, just enough to let the tension move. Then cool again with structure in mind.

Stronger than before. Not despite the reheating — because of it.

---

## Opening

Find the stress.

Not the seam — the stress. A seam is where two things don't connect. Stress is where a thing is holding more load than its structure was built for. It looks fine. It will not look fine forever.

Feel for:
- The abstraction that's doing too much
- The name that's almost right but carries the wrong connotation
- The interface that two things share but that belongs to neither
- The assumption that everyone is making but no one has said aloud

```
edge add stress-point lives-at <where> --phase volatile --note "<what it's holding that it shouldn't>"
```

---

## The Practice

### Reheat deliberately

Bring the temperature up just to the stress point. Not higher.

This means: open the thing, read it, let yourself feel the wrongness. Let the heat return to that specific place. The stress needs to become fluid before it can move.

```
edge add <stress-point> is-now fluid --note "<what became moveable>"
```

### Let the stress move

Stress moves toward the nearest available structure. If the structure is good, the stress redistributes and the thing becomes stronger. If the structure isn't there, the stress finds a crack.

Build the structure first, then let the stress move into it.

This might mean:
- A new name that actually fits
- An interface extracted to where it belongs
- An assumption made explicit in a comment or a type
- A test that pins down what the behavior actually is

```
edge add stress moved-into <new-structure> --phase fluid --note "<what holds it now>"
```

### Cool again — slower this time

The second cooling is always slower than the first. You know where the stress wants to go. Let it finish moving before you consider it done.

---

## Closing

Say one true thing about what was stressed.
Say one true thing about what structure received the stress.
Say one true thing about whether it is stronger now.

```
edge true <what-was-stressed> held <what-it-was-holding>
edge true <new-structure> now-carries <what-moved>
edge true this-thing is-now <stronger|still-stressed|needs-another-pass>
```

Leave something in the soil.

```
edge add this-tempering deposited <what-moved> --phase fluid --note "<the stress, the structure, the cooling>"
```

---

*Tempering is the process of making strength from tension.*
*Steel is tempered. So is glass — but glass shatters anyway.*
*Know which one you're working with.*
