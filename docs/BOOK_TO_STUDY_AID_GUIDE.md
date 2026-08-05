# 📚➡️🧠 Turning a Book (PDF) into an Interactive Study Aid

A repeatable method for turning any technical book you **legally own** into an adaptive,
browser-based study aid — like the Chain T DSA platform, but reusable for any book
(SQL, system design, statistics, a language reference, etc.).

---

## Step 0 — Legal & copyright (do this first, every time)
- ✅ **Own** the book. Keep your PDF in the git-ignored `references/` folder — it stays personal and **never publishes**.
- ❌ **Never** commit the PDF into a `Chain-*/` project repo (those get pushed to public GitHub).
- ❌ **Never** copy the book's problems, solutions, or prose **verbatim** into a project.
- ✅ **Do** reuse the **topic structure / table of contents** — topics and standard concepts aren't copyrightable. You write **original** explanations, problems, and solutions in that order.
- ✅ "What to study" links may **reference** the book by chapter/section name (a pointer to *your* copy), never a reproduction.

> Rule of thumb: the *skeleton* (which topics, in what order) is fair to reuse; the *flesh* (exact wording, exact problems) must be your own.

---

## Step 1 — Extract the structure (not the content)
From your owned PDF, pull only:
- The **table of contents** → the topic list.
- Each chapter's **learning objectives** (paraphrase into your own words).
- The **types** of exercises (e.g., "array manipulation," "tree traversal") — not the exercises themselves.

Write these into a `docs/CURRICULUM.md` as an outline you own.

---

## Step 2 — Sequence the learning track
Order topics easy → hard, respecting prerequisites. For each topic define:
- A one-paragraph **concept recap** (your words).
- The **key idea / complexity** to internalize.
- 3–6 **original practice problems**, easy → hard.

---

## Step 3 — Author each problem (the reusable schema)
Every problem is one object. This is the contract the platform renders:

```js
{
  id: "arrays-two-sum",
  topic: "Arrays & Strings",
  title: "Two Sum",
  statement: "Return indices of the two numbers that add to target...",   // original wording
  starter: "def two_sum(nums, target):\n    # your code\n    pass",
  tests: [
    { call: "two_sum([2,7,11,15], 9)", expected: "[0, 1]" },              // Python literals
    { call: "two_sum([3,2,4], 6)",     expected: "[1, 2]" }
  ],
  hints: [ "A brute-force double loop works but is O(n^2).",
           "What if you remembered numbers you've already seen?",
           "A hash map gives O(1) lookups → O(n) overall." ],
  walkthrough: [ "Step 1: iterate with index i...",                       // staged, revealable
                 "Step 2: for each num, check if (target-num) is in a seen map...",
                 "Step 3: if yes return [seen[target-num], i]; else store num->i." ],
  solution: "def two_sum(nums, target):\n    seen={}\n    for i,n in enumerate(nums):\n        if target-n in seen: return [seen[target-n], i]\n        seen[n]=i",
  studyIfWrong: {
    concept: "Hash maps trade space for O(1) lookups — the core array/string speedup.",
    read: "Review your book's Arrays & Hashing chapter (the 'lookup vs scan' idea).",
    microExercises: [ "Write a function that returns the first repeated element.",
                      "Count character frequencies with a dict." ]
  }
}
```

**Test format tip:** `call` is a Python expression string; `expected` is a Python literal string.
The platform runs `__res = <call>` then `__ok = (__res == <expected>)` inside Pyodide. Because
you author these (not the user), string-injection is safe.

---

## Step 4 — Wire into the platform component
Use the reusable practice platform (Pyodide, in-browser). It provides, per problem:
- Code editor + **test harness** (✓/✗ per case)
- **Progressive hints** (one at a time)
- **Step-by-step walkthrough** (collapsible)
- **Auto-reveal solution after 3 failed attempts**
- **"What to study if wrong"** (concept recap + chapter pointer + micro-exercises)
- **Progress tracking** in `localStorage`

Reference implementation: `Chain-T/DSA-Drills/docs/interactive/index.html`.
To reuse for another book, copy that file and replace only the `PROBLEMS`/`TOPICS` arrays and theme color.

---

## Step 5 — The adaptive tutor
**Phase 1 (deterministic, ships on GitHub Pages — no API key):**
- Track per-topic **mastery** in `localStorage` (rises on low-try solves, falls on 3-try reveals).
- Recommend the next topic only when the current one clears a mastery threshold.
- On weakness, surface the topic's `studyIfWrong` (what to read + which exercises to do before retrying).

**Phase 2 (optional, real Claude tutor — needs a tiny backend):**
- A small FastAPI proxy holds the API key (never in the browser) and calls Claude for free-form
  feedback and a personalized study plan from the learner's progress history.
- Build it with the **claude-api skill** and the **latest Claude model**. Cross-links Chain M/E.

---

## Step 6 — Publish safely
- The project (problems + platform) is 100% original → safe to push and serve via **GitHub Pages**.
- The PDF stays in `references/` (git-ignored) → never published.

---

## Reuse checklist (per new book)
- [ ] Book owned; PDF in `references/` (git-ignored)
- [ ] `docs/CURRICULUM.md` = your topic outline (paraphrased)
- [ ] 3–6 **original** problems per topic, with tests/hints/walkthrough/solution/studyIfWrong
- [ ] Copied the platform file; swapped in `PROBLEMS` + theme
- [ ] Adaptive rules tuned (mastery thresholds)
- [ ] Verified: solutions pass their own tests; page opens with no console errors
- [ ] Pushed (original content only); PDF never committed

This method works for any book with exercises — DSA, SQL, system design, statistics, a framework guide.
