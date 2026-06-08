# Before Class — L05 — Unsupervised Learning

**Estimated time: ~30 minutes.** Complete this before class.

This is the simplest version of "show up prepared": watch a short intro, run one notebook, answer a few questions. You'll come to class having seen the idea in action.

| Step | Time | What you do |
|---|---|---|
| **0. Watch the intro** | ~5 min  | Short video framing the lesson |
| **1. Try it** | ~20 min | Open and run `notebooks/01_monday_morning.ipynb` |
| **2. Reflect** | ~5 min  | Three short questions below |

---

## Step 0 — Watch the intro (~5 min)

Watch the short intro video: **[L05 — Unsupervised Learning intro →](https://youtu.be/_nm7QrtOoUQ)**

It sets up Sarah's pivot: from "predict churn with labels" to "find structure *without* labels" — and previews PCA, K-Means, and Isolation Forest at a high level.

---

## Step 1 — Try it (~20 min)

Open **`notebooks/01_monday_morning.ipynb`** in VS Code with the `dsai-m3` kernel. Run every cell top to bottom. Read the markdown between cells. Don't skip any cell.

Marcus pivots: *"Find me natural customer segments — without labels."* Sarah meets the unsupervised toolkit: PCA to visualise high-dim customers in 2D, K-Means to group them, Isolation Forest to flag anomalies. The notebook's honest reveal: PCA captures 22% variance in 2D, and that's *correct*, not a failure.

If this is your first time running a notebook in this repo, see [setup.md](./setup.md) once — you only need to do this for the first lesson.

---

## Step 2 — Quick reflection (~5 min)

Write a sentence or two for each. You can scribble in a notebook, in a journal, or just hold the answer in your head — what matters is that you *tried*.

**Q1. PCA shows 22% variance in 2D. Is that good or bad?**

What does it tell you about the original feature set?

**Q2. How do you choose K for K-Means without ground truth?**

Sarah uses elbow + silhouette + business judgement. Why all three rather than just one?

**Q3. Anomaly detection has no labels.**

If your Isolation Forest flags 500 customers as anomalous, how do you decide if it's *actually finding* anomalies?

---

## Bring to class

- Your answer to Q1.
- One business problem from your own work that's naturally unsupervised (no labels available).

---

**Want to go deeper before class?** See **[reference.md](./reference.md) → *Further reading & watching*** at the bottom — videos and recommended readings that used to live in this guide.

**Ran out of time?** Doing just Step 1 (running the notebook) is enough. The class builds on having felt what the lesson teaches; the reflection questions get re-asked live.
