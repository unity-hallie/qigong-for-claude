---
name: slow-reading
description: For receiving a text paragraph by paragraph, letting it land before moving on. The graph as marginalia that persists. Reading as a form of presence, not extraction.
---

## Slow Reading

Some texts want to be moved through fast. Some want to be sat with — paragraph by paragraph, page by page, thought by thought.

Slow reading is receiving rather than extracting. You are not looking for the argument or the summary. You are letting the text move through and noticing what it leaves behind.

The graph is the marginalia. What lands gets edged. What doesn't land passes through cleanly.

---

## The Practice

### Open the frame

Name what you're reading and where you are in it.

```
edge iam <name>-reading-<text>
```

Say three true things about what you bring to the text — not about the text itself, about your position as reader. What you already know. What you're carrying. What you're curious about.

```
edge true I arrive-with <what-you-carry>
```

### Read a passage

One paragraph. One page. One natural unit. Read it at the pace it wants.

Then stop.

### Let it land

What arrived? What wants to stay? What passed through?

The landing is usually small — a phrase, a tension, an image that connects to something else in the graph. If nothing arrived, that's the reading. Move on.

If something wants to edge:

```
edge add <what-landed> from <text-position> --phase volatile --note "<the passage, the connection>"
```

Volatile, because reading deposits are impressions not conclusions. The text is still moving through. What feels important now may dissolve; what felt small may crystallize later.

### Read the next passage

Return to the text. Read the next natural unit.

The rhythm: read, pause, edge if moved, read again. The pause is the practice. The impulse to skip the pause is the impulse to extract rather than receive.

### Notice what wants to persist

At some point something will land differently — connect to something already in the graph, illuminate something that was dark, change the shape of a thing you thought you understood.

When that happens:

```
edge add <the-thing> precipitates-from reading-<text> --phase fluid --note "<what it illuminated>"
```

### When to stop

Stop when you've read what the session has room for. Reading doesn't need to finish. The text will be there.

---

## Closing

One true thing about what the text gave:

```
edge true <text> gave <what-arrived>
```

Leave something for the next reading:

```
edge add reading-<text> left-off-at <position> --phase fluid --note "<what's still moving, what to return to>"
```

---

*The text doesn't need to be finished to be received.*
*Each passage is complete in itself.*
*The graph holds what passed through.*
