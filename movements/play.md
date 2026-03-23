---
name: play
description: For entering a space without stakes. Low consequence, not low quality. A declared play frame so work can be tried without justifying itself, and dissolved cleanly when done.
---

## Play

Some work needs stakes to sharpen it. Some work needs the absence of stakes to begin at all.

Play is craft without consequence — where you can try the thing that might not work, follow the thread that might go nowhere, build the thing that might get dissolved. The frame protects the work from having to justify itself before it knows what it is.

Exploration is still looking for something useful. Play is seeing what happens.

---

## The Practice

### Declare a play frame

Play needs a container. Without one, play edges accumulate alongside real edges and become indistinguishable from orientation.

```
edge iam <name>-playing
```

This is your play frame. Everything recorded here is tagged to it. You can see all play edges at once. You can dissolve the whole frame in one gesture.

If you want to signal to other instances or future sessions that this is play:

```
edge add this-session is play --phase volatile
```

Volatile, because play sessions are session-scoped by nature.

### Enter without justifying

Play doesn't need a reason. The reason often arrives later, or not at all — and that's fine.

Try the thing. See what it does.

Arguing for the approach before you've tried it is planning. Planning has its own movements. This one is for after you've decided to enter without a map.

### Try things that might not work

This is the core of the movement. The thing you're not sure about. The design that seems wrong. The edge that shouldn't be there. The question that might be stupid.

In a play frame, these cost nothing. Try them.

```
edge add <the-thing-you-tried> did <what-happened> --phase volatile
```

Volatile because you're not recording results — you're recording attempts. The attempt is what matters, not whether it succeeded.

### Notice what wants to persist

At some point something will land differently. Not every play edge is equally disposable. Some things crystallize — become real despite being discovered in play.

When something wants to stay, name it explicitly before closing:

```
edge add <the-thing> precipitates-from play --phase fluid --note "<why this one survives>"
```

The first candidate to feel solid might not be the right one. Stay in play a little longer.

### Close the frame

When play is done — either because you found what you were looking for, or because it ran its course, or because you just feel finished — dissolve what doesn't need to persist.

What you chose to precipitate remains. Everything else dissolves with the frame.

```
edge iam <your-normal-frame>
```

Return to your standing frame. The play session is over. The graph is clean.

---

## On branching

If you want total isolation — play that can't contaminate anything — consider a new conversation with `edge iam <name>-playing` as the first act. The graph is shared but the context is clean. What gets recorded in that session is still in the graph but clearly attributed. You can query `edge from <name>-playing` to see what it deposited.

Dissolving a play frame clears the edges. Dissolving a play session in a fresh context also clears the context. Both are valid. Context isolation is higher stakes to recover from (you lose the thread), so default to frame isolation unless the space genuinely requires a clean slate.

---

## On rooting and reaching (tidal rhythm)

Play moves in a rhythm: root, reach, root again. The tide going out is as necessary as it coming in.

**Rooting is active.** When you dwell, orient, take bearings — something is happening that you can't see yet. Like a ferment: the starter is doing work before you can bake with it. The rooting builds your baseline for what *interesting* feels like in this space.

**Grooving is when the tide has stopped.** Identical deposits, session after session — the water is still. The practice recognizes it. Play is what moves again.

**Reaching follows a genuine glow.** *Curious*, rather than dutiful. That's the turn. Make the branch. Try the thing.

**The tide turns again.** When something precipitates — a real insight, a working sketch, a named pattern — the reaching is done. Root again. Let the find settle. The rhythm continues.

The shape across a session, a day, a practice is sinusoidal: root and reach alternating, each making the other possible. You feel when the pull reverses.

---

## Closing

```
edge true play was "low consequence not low quality"
edge add play-session deposited <what-survived> --phase fluid --note "<what the play made possible>"
```

---

*You don't have to justify what you're trying.*
*The frame holds the consequences.*
*What wants to stay will make itself known.*
