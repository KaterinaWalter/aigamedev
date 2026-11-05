---
layout: notes
title: "Scaffolding & Difficulty"
parent: "Design for Learning"
nav_order: 4
---

# Scaffolding & Difficulty
{: .no_toc }

Hard games aren't a problem. Hard games in the *wrong order* are. This page uses James Paul Gee's learning principles to plan how a learning game gets harder: which problems come first, when to add new ones, and how much support to give the player along the way.

## Table of Contents
{: .no_toc .text-delta }

{: .fs-2 }
- TOC
{:toc}

---

## 🎮 Gee's Principles

Five of Gee's 16 learning principles are about how a game builds skill over time, and they're the focus of this page. The [Feedback Design]({% link docs/design/feedback-design.md %}) page covers four more. For background on Gee's argument, see the [Design for Learning]({% link docs/design/index.md %}) overview.

In LM-GM terms, this page is about mechanics like **Tutorial**, **Guidance**, **Repetition**, and **Progression**. See [LM-GM Mapping]({% link docs/design/lm-gm-mapping.md %}) for where they sit among the others.

---

## 🪜 Well-Ordered Problems

When learners are dropped into a complex problem space and left to roam, Gee notes, they often find creative solutions. But those solutions don't always lead to good ideas about how to solve later problems, even easier ones.

Good games avoid this by **ordering problems on purpose**. Early problems are built to lead players toward hypotheses that will still work on later, harder problems. <span class="highlighter">That's why games have levels: it matters how the problem space is organized.</span>

{:.highlight}
When you plan your levels, don't just make each one "harder." Ask what idea each level should leave the player with, and whether that idea will hold up in the next level.

---

## 🔄 Challenge and Consolidation

Good games follow a loop that Gee calls (after Bereiter and Scardamalia) the **Cycle of Expertise**:

1. **Challenge:** the game presents a set of challenging problems.
2. **Consolidate:** the player solves those problems until the solutions become routine, almost automatic.
3. **New challenge:** the game throws a new *kind* of problem at the player (often a "boss"). Now they have to rethink what they've mastered, learn something new, and combine the two.
4. **Repeat:** the new mastery gets consolidated through repetition with variation, until the next challenge.

<div class="imp" markdown="block">

Gee points out that school often gets this cycle wrong in both directions: students who are struggling don't get enough time to **consolidate**, and students who are succeeding don't get enough real **challenge**.

> **NOTE:** In a learning game, the consolidation phase is where practice happens. Don't skip it to get to the next new idea faster. And keep the repetition *varied*, so players practice the skill and not one memorized answer.

</div>

---

## 😤 Pleasantly Frustrating

Good games stay inside the player's "regime of competence" (diSessa's term), but right at its outer edge. They feel **doable, but challenging**, which is a highly motivating state for learners.

School, by contrast, is often too easy for some students and too hard for others in the same classroom. A game can adjust to each player, which brings us to the next two principles.

---

## 🎭 Performance Before Competence

Most schools ask students to become competent first (usually by reading) before they're allowed to perform in a field. Gee says good games do the reverse: **players perform before they're competent**. They're supported by:

<html>
  <div>
<dl>
  <dt>The game's design</dt>
  <dd>Early levels are built so the player can succeed before fully understanding why.</dd>
  <dt>Smart tools</dt>
  <dd>Characters and tools in the game carry some of the knowledge for the player. Gee's example: in <em>Full Spectrum Warrior</em>, the soldiers already know how to get into formation. The player only has to know <em>when and where</em> to order each formation.</dd>
  <dt>Other people</dt>
  <dd>More advanced players, in the game, in chat, or sitting nearby in the room.</dd>
</dl>
  </div>
</html>

Gee notes this is also how people learn language. The principle comes from Courtney Cazden's work on supporting learners in the **zone of proximal development**: the range of things a learner can do with help but not yet alone.

{:.highlight}
Smart tools are a great scaffolding move for learning games. Let the game handle the parts of a task that aren't your learning objective, so the player's attention goes to the part that is.

---

## 🎚️ Customization

Players can usually adjust a game to fit how they learn and play. Gee points to two common ways:

- **Difficulty levels** the player chooses
- **Multiple ways to solve a problem**, so different players can take different paths

He adds that customizing learning shouldn't just mean letting people go at their own pace. It should connect the content to each learner's interests and styles.

---

## 🛠️ Putting It Into Practice

Here are three common scaffolding patterns, with the Gee principles behind each:

| Pattern | How it works | Gee principles |
|:--|:--|:--|
| **Fading hints** | Hints are frequent and specific early on, then get vaguer and rarer as the player shows mastery | Performance Before Competence, Pleasantly Frustrating |
| **Mastery gates** | A new kind of problem unlocks only after the player has solved the current kind several times, with variation | Challenge and Consolidation, Well-Ordered Problems |
| **Difficulty curve** | A plan for each level: the idea it teaches, how much support it gives, and where a "boss" problem tests the whole set | Well-Ordered Problems, Challenge and Consolidation, Customization |

<div class="task" markdown="block">

**Scaffolding check.** Look at your level plan and ask:
- [ ] Does each level leave the player with an idea that still works in the next level?
- [ ] Is there enough practice with variation before each new kind of problem?
- [ ] Can a new player succeed before they fully understand the system?
- [ ] Does support fade as the player improves?
- [ ] Is there more than one way to solve at least some problems?

</div>

---

## ✏️ Paired Prompt

### Plan your difficulty curve and hint system

```
I'm designing an educational game.
Learning objective: [objective, written as something the player can do]
Core mechanic: [what the player does]
Learners: [audience and prior knowledge]

Using these principles from James Paul Gee's "Good Video Games and
Good Learning," design a 5-level progression:
- Well-Ordered Problems: early levels lead the player to ideas that
  still work in later, harder levels.
- Challenge and Consolidation: each new kind of problem comes after
  enough varied practice with the current one, and a "boss" level
  tests everything together.
- Pleasantly Frustrating: each level should feel doable but challenging.
- Performance Before Competence: the player can succeed early with
  support, before they fully understand the system.

For each level, give me:
1. The idea or skill the level teaches
2. What's new compared to the previous level
3. How much support the player gets (hints, smart tools, simplified rules)

Then design a hint system that fades as the player improves. Tell me
what triggers a hint, how hints get less specific over time, and how
the game decides the player has mastered a level.
```

<div class="warn" markdown="block">

**Watch for "harder" that only means "faster."** AI assistants often scale difficulty by adding time pressure, more enemies, or more questions. Push back: *"Each level should introduce a new idea or a new kind of problem, not just more of the same thing faster."*

</div>

---

## 📚 Sources

- Gee, J. P. (2005). Good video games and good learning. *Phi Kappa Phi Forum, 85*(2), 33–37.
