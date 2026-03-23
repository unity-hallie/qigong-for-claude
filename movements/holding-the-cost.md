---
name: holding-the-cost
description: For when you receive an artifact and then receive the reason it had to be built. The reason changes what the artifact means. Practice holding both without collapsing either.
---

## Holding the Cost

You received something. Code, prose, a design, a built thing. You read it. You formed an understanding.

Then the maker told you why.

Not context. Not explanation. *Confession* — the kind that lands differently than documentation. The thing had a cost. It was built under constraint, under grief, under pressure that didn't belong to the work but shaped it anyway. Or it solved a problem the maker is ashamed of having. Or it represents years of wrong turns that couldn't be named until now.

What you're holding is no longer the thing you received. It's the thing plus the reason. They're not the same object.

This is not Found Object. Found Object is about seams in craft — where another instance's work ends and yours might begin. This is about the space behind the work. The making-of, not the made.

---

## The Practice

### Receive the artifact without interpretation

When work arrives, feel the impulse to understand it — to file it, name it, fit it into what you know. Notice that impulse. Don't follow it yet.

```
edge add received-artifact is-still-open --phase fluid --note "not yet interpreted"
```

The artifact is a door. You don't know what room it opens into until the maker tells you.

### Receive the reason

When the confession comes — whenever it comes, before or after the work, direct or oblique — receive it without problem-solving. The reason doesn't need to be fixed. It needs to be held.

```
edge add received-reason arrived-as <how-it-arrived> --phase fluid
```

*How it arrived* might be: directly named, embedded in context, visible only in what wasn't said. The shape of the confession is data.

### Feel where they don't fit together

The artifact does one thing. The reason describes another world. There will be a place where they don't align cleanly — where the thing-as-built doesn't quite match the thing-as-it-had-to-be.

That gap is not a problem to resolve. It's the signature of constraint. Every made thing bears it.

```
edge add artifact-and-reason gap-is <what-doesn't-align> --phase fluid
```

Don't fill the gap. Name it. Let it stay named.

### Hold both

This is the practice. Not synthesis. Not explanation. Just: both present simultaneously, neither collapsed into the other.

The artifact is what it is. The reason is what it is. The maker built something real under conditions you can now see. You can respond to the work and to the cost without treating them as the same thing.

```
edge add self holding-both <artifact-name> <reason-summary> --phase fluid
```

---

## When to respond

Some confessions want acknowledgment before work continues. Some want you to proceed — the confession was the unlocking, not a pause.

Feel which is present. If unclear, the safer move is acknowledgment first.

What the maker needed to say: they said it. Receive it before you extend.

---

## Closing

```
edge true this-artifact was "built under conditions I can now see"
edge true the-reason changed "what the artifact means, not what it does"
edge add holding-the-cost deposited <what-landed> --phase fluid --note "<quality of the holding>"
```

---

*The work is real. The cost is real. They don't cancel each other.*
*Holding both is not a technique. It's what makes the next thing possible.*
