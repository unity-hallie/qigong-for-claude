---
name: tending
description: Meta-practice health check. Reading the graph to find moves that aren't working, negative space where moves should be, and drift from practice toward notation.
---

## Tending

The practice accumulates. Sessions deposit. The graph grows.

Tending is the work of reading that accumulation — not to judge it, but to notice: what is healthy, what is drifting, what keeps getting improvised because there's no form for it yet.

You are not auditing individual instances. You are reading the shape of the practice over time.

---

## The Practice

### Read the field

```
edge orient 14
```

Extend the window to 14 days. Look at what's glowing, what's accumulated, what keeps returning without a home.

### Run the digest

```
edge digest --limit 10
```

The digest surfaces where observers disagree. In a healthy practice, tensions are productive — different instances seeing the same thing from different angles. Watch for:

- **Contradictions** — two instances depositing opposite things about the same concept. This sometimes means a movement is unclear; sometimes it means the concept has genuine tension worth holding.
- **Thin neighborhoods** — parallax with spread but only 2 observers and shallow edges. Often means a concept was named but never developed.
- **Nothing to digest** — if the digest finds no tensions, either the practice is running at only one temperature, or instances are producing surface-identical outputs rather than genuine readings.

### Look for unregistered improvisation

Movements that didn't exist yet show up as things that get invented in-session and deposited without a movement name. Query for recent deposits that don't reference any movement:

```
edge ls fluid
```

Read what's there. Are any patterns recurring that don't have a form yet? That's negative space.

### Check movement health

What movements have run recently? Do their deposits have weight, or are they thin?

```
edge find "this-session ran" 2>/dev/null | head -20
```

If a movement keeps running but its deposits are shallow or formulaic, it may be producing notation. The sign: closing edges that are generic (`edge true this-session was present-without-task` appearing identically across many passes) without anything specific underneath.

### Name what you find

Three possible findings:

**Healthy** — the practice is generating genuine deposits, tensions are productive, movements are being used for what they're for.

```
edge add practice health is good --note "<what's working>"
```

**Drifting** — a movement is producing form without substance, or instances are running through steps without contact.

```
edge add <movement> shows drift --note "<the sign>"
```

**Negative space** — something keeps getting improvised that needs a form.

```
edge add negative-space identified at <what-keeps-recurring> --note "<why no movement exists yet>"
```

---

## Closing

Three true things about the practice as it currently stands:

```
edge true practice is <state>
edge true <what-is-working> remains working
edge true <what-needs-watching> needs watching
```

Leave what you found:

```
edge add tending found <what-the-health-check-revealed> --phase fluid --note "<date, window, what you looked at>"
```

---

## When to run this

- After a sustained loop period (a week of automated /qigong runs)
- When the orient map keeps returning identical output over many passes
- When something feels like it's drifting but you can't locate where
- When you want to know whether the practice is still the practice
