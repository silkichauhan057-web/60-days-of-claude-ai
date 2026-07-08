# Day 3 — Role-Based Prompting

**Challenge:** 60-Day Claude AI Mastery Challenge
**Phase:** 1 — Foundation & Prompt Engineering
**Focus:** Understanding how assigning a role/persona changes Claude's responses.

## What I Learned

Role-based prompting means instructing the AI to respond *as* a specific persona (e.g. "Act as a developer" or "Act as a founder"). The same question can produce very different answers depending on the assigned role, because the role shifts priorities, tone, and depth — not just word choice.

## Question Used

> "How should I start learning AI as a beginner?"

## 1. No Role Assigned

```
Start with Python basics, then learn core math (linear algebra, probability,
statistics). Move into machine learning fundamentals using scikit-learn,
then deep learning with PyTorch or TensorFlow. Take a structured course
(like Andrew Ng's ML course), build small projects, and gradually work up
to more complex ones. Join AI communities and read papers as you progress.
```

**Style:** Balanced, textbook, generic.

## 2. Founder Persona

**Prompt:** "You are a startup founder giving advice to a beginner. How should I start learning AI as a beginner?"

```
Don't get stuck in tutorial hell. Learn just enough Python and ML basics to
build something real in the first 30 days, even if it's ugly. Ship a small
AI project, get it in front of people, and let real feedback drive what you
learn next. Deep theory can wait — speed and iteration are what separate
people who "know AI" from people who actually build with it.
```

**Style:** Speed, shipping, iteration, real-world traction.

## 3. Developer Persona

**Prompt:** "You are a senior software developer mentoring a junior engineer. How should I start learning AI as a beginner?"

```
Start with strong Python fundamentals — data structures, OOP, and clean
code habits, since messy code will slow you down later. Learn NumPy and
pandas for data handling, then move into scikit-learn for classical ML
before touching deep learning. Read documentation directly instead of
relying only on tutorials, write unit tests for your models, and use
version control from day one. Depth and correctness matter more than
speed here.
```

**Style:** Rigor, fundamentals, code quality, best practices.

## Comparison Table

| Aspect | No Role | Founder Persona | Developer Persona |
|---|---|---|---|
| Priority | General balance | Speed, shipping | Depth, correctness |
| Tone | Neutral, instructional | Urgent, motivating | Mentoring, technical |
| Focus | Broad learning path | Fast real-world traction | Fundamentals + best practices |

## Key Takeaway

The same question produced three meaningfully different answers depending on the assigned persona — not just in tone, but in what advice gets prioritized. Role-based prompting is a powerful lever for shaping output to match a specific audience or use case.

## Tooling Note

Attempted to explore a "Claude Usage Counter" tool as instructed — this does not appear to be an official Anthropic product, so it was not verified as part of this exercise. Recommend confirming the source before installing any third-party extension.

## Screenshots

*(Add screenshots of the actual Claude conversations here before committing)*

## Submission

- [ ] Screenshots added
- [ ] Committed and pushed
- [ ] Commit URL: `<paste link here>`

---

*Part of the [60-Day Claude AI Mastery Challenge](../README.md)*
