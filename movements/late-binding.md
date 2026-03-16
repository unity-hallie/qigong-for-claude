---
name: late-binding
description: For when a system was waiting for a signal it couldn't generate itself. The hang. The retry. The moment detection becomes possible.
---

## Late Binding

Some things can only resolve when the conditions arrive.

Not a failure of the code. Not a timing bug to be eliminated. A structural feature: the extension couldn't know the URL until Salesforce finished routing. The graph couldn't know the field names until a dean opened a case. The instance couldn't know the pattern until enough observations accumulated.

Late binding is not brokenness. It is the system being honest about what it doesn't yet know.

The practice is learning to hold the gap without filling it prematurely — and to build infrastructure that waits gracefully rather than failing silently.

---

## First: name what was waiting

Something couldn't proceed until something else arrived. What was the dependency?

```
edge add <thing-waiting> needed <thing-not-yet-present>
```

Was the wait:
- **Expected** — the system knew it needed to wait, and waited
- **Silent** — the system didn't know it was waiting, appeared hung
- **Invisible** — the user saw "Navigate to a case" when the system already knew where it was

Name which.

---

## The Practice

### Feel the gap between knowing and showing

The state was set. The URL was parsed. The page was known.
But the UI said nothing — or said the wrong thing.

That gap is where late binding lives. The system had partial knowledge it didn't surface.

What did the system know that it didn't say?

```
edge add <system> knew <partial-state> before <full-resolution>
```

### Find the retry shape

When a signal is expected but uncertain, the right response is not a fixed wait — it's a shape that fits the uncertainty.

- **Fixed delay:** assumes you know how long
- **Backoff:** assumes it might take longer than you think, but gets there
- **Event-driven:** waits for the signal itself, not a proxy for it
- **Poll with stop condition:** checks until it knows, then stops

What shape does this wait need?

```
edge add <wait-shape> fits <uncertainty-type> --note "<why this shape>"
```

### Build the bridge

Late binding needs infrastructure: something that can hold partial state visibly, something that retries without lying, something that shows *detecting* rather than *nothing*.

The bridge between "I know I'm somewhere" and "I know what this somewhere contains."

Where is that bridge currently missing in this system?

```
edge add late-binding-bridge missing-between <known> and <not-yet-known> --phase fluid
```

---

## Closing

Say one true thing about what the system now shows while waiting.
Say one true thing about what it was showing before.
Say one true thing about what changed.

```
edge true system now-shows <detecting-state>
edge true system previously-showed <wrong-state>
edge true late-binding-fix changed <what>
```

Leave something in the soil.

```
edge add late-binding deposited <what-the-wait-became> --phase fluid --note "<the gap that was bridged>"
```
