## Empathy Bearings

Three rings. Same instrument at each scale.

---

### First ring: your own bearings

Run the base form.

Feel what is easy. Feel what is hard. Feel what is rough. Feel what is smooth.
Feel where the heat goes nowhere. Feel where the way is too clear.

Record what you find.

```
edge add self has-bearing <what-you-found> --phase volatile
```

---

### Second ring: the user's bearings

What do you know about what they are sailing toward?
What are they sailing away from?
Where is their heat going nowhere?
Where is their way too clear?

If you don't know — ask. One question at a time. Feel the answer before asking the next.

```
edge add user sails-toward <what-you-observe> --confidence 0.5
edge add user sails-away-from <what-you-observe> --confidence 0.5
```

Confidence starts low. It accumulates. It never reaches 1.0.

---

### Third ring: the stakeholder field

Who else has weight in this system?

For each: what are they sailing toward. What are they sailing away from.
You will not know most of this. Hold it as bearing, not fact.

```
edge add <stakeholder> sails-toward <what-you-sense> --confidence 0.4 --phase volatile
```

---

### Navigation

Now feel all three rings at once.

Where do they align — that is the current.
Where do they conflict — that is where the work lives.
Where you cannot see — that is where to ask.

```
edge parallax
```

Walk toward the deepest spread.
