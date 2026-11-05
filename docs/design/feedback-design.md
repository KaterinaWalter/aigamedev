---
layout: notes
title: "Feedback Design"
parent: "Design for Learning"
nav_order: 3
---

In a good game, the world responds to everything the player does. That response is how the player learns. This page uses four of James Paul Gee's learning principles to design feedback that teaches, instead of feedback that just grades.

## Table of Contents
{: .no_toc .text-delta }

{: .fs-2 }
- TOC
{:toc}

---

## 🎮 Gee's Principles

Gee lists 16 learning principles that good games use. Four of them are about how a game responds to the player, and they're the focus of this page. The [Scaffolding & Difficulty]({% link docs/design/scaffolding-difficulty.md %}) page covers five more. For background on Gee's argument, see the [Design for Learning]({% link docs/design/index.md %}) overview.

In LM-GM terms, this page is about the **Feedback** mechanic. See [LM-GM Mapping]({% link docs/design/lm-gm-mapping.md %}) for where it sits among the others.

---

## 🔁 Interaction: The Game Talks Back

Gee borrows Plato's complaint that books are passive: you can't get them to talk back. Games do. <span class="highlighter">Nothing happens until the player acts and makes a decision.</span> Then the game reacts, giving the player feedback and new problems.

For a learning game, this means your feedback loop *is* your instruction. Every action should produce a visible reaction from the game world that tells the player something about the system they're learning.

{:.highlight}
The most common vibe-coded feedback is a "Correct!" or "Try again!" pop-up. That's the game grading the player, not the world reacting. Compare a pop-up that says "Wrong" with a bridge that actually sags and collapses because the player put the support in the wrong place.

---

## 💥 Risk Taking: Failure as Information

Good games **lower the consequences of failure**. Players can restart from the last save, so they're encouraged to take risks, explore, and try new things. Gee goes further: in a game, failure is a *good* thing.

<div class="imp" markdown="block">

Gee's example is a boss fight. The player uses early failures to figure out the boss's pattern and to get feedback on their progress. Each failed attempt is data.

> **NOTE:** For this to work, failure has to be **cheap** (fast to retry, not much progress lost) and **informative** (the player can see *why* it failed). If either one is missing, failure just feels like punishment.

</div>

---

## ⏱️ Just in Time and On Demand

People are bad at processing lots of words out of context, which Gee says is why textbooks are so inefficient. Games give verbal information in two ways:

<html>
  <div>
<dl>
  <dt>Just in time</dt>
  <dd>Right when the player needs it and can use it. Example: a tip about a new tool appears the first time the player picks it up.</dd>
  <dt>On demand</dt>
  <dd>When the player feels they need it, wants it, and is ready for it. Example: a glossary, codex, or hint button the player can open whenever they choose.</dd>
</dl>
  </div>
</html>

What both have in common: the information arrives when it can be used. If your game opens with three screens of instructions, that's the textbook problem all over again.

---

## 🎬 Situated Meanings: Show, Don't Define

People struggle to learn what a word means from a definition made of other words. According to the research Gee cites, we really learn words when we can connect them to experiences: actions, images, and dialogue.

Gee's example: "The coffee spilled, go get a mop" versus "The coffee spilled, go get a broom." Same word, different meaning, and the situation is what tells you which.

Games always tie words to the actions, images, and dialogue they refer to. So when your feedback introduces a term (like "equilibrium," "bias," or "opportunity cost"), introduce it *at the moment* the player sees it happen in the game.

---

## 🛠️ Putting It Into Practice

Here are three kinds of feedback you can mix in a learning game, with the Gee principle each one draws on:

| Kind of feedback | What it looks like | Gee principle |
|:--|:--|:--|
| **World reaction** | The game system visibly responds to the player's action (things move, break, grow, react) | Interaction |
| **Failure debrief** | After a failed attempt, a quick look at what happened and why, then an immediate retry | Risk Taking |
| **Information on request** | Hints, a glossary, or explanations the player can open when they choose, plus short tips that appear when something new shows up | Just in Time / On Demand, Situated Meanings |

<div class="task" markdown="block">

**Feedback check.** For each core action in your game, ask:
- [ ] Does the *world* respond, or just a score or pop-up?
- [ ] After failing, can the player tell what went wrong?
- [ ] Is retrying fast and cheap?
- [ ] Do new terms show up at the moment the player sees them in action?

</div>

---

## ✏️ Paired Prompt

### Design feedback for your core mechanic

```
I'm designing an educational game. Here's my core mechanic:
[describe what the player does, and what they're learning by doing it]

Design the feedback for this mechanic using these principles from
James Paul Gee's "Good Video Games and Good Learning":
- Interaction: the game world should visibly react to the player's
  action, not just show "correct" or "incorrect."
- Risk Taking: failure should be cheap and informative. After a failed
  attempt, the player should be able to tell what to try next.
- Just in Time / On Demand: explanations appear when the player needs
  them, or when they ask.
- Situated Meanings: introduce key terms at the moment the player sees
  them in action.

Give me:
1. What the player sees and hears on success, and on failure
2. How a failed attempt shows the player what to try next
3. Which information is just in time and which is on demand
4. How quickly the player can retry after failing
```

<div class="warn" markdown="block">

**Watch for grading disguised as feedback.** If the AI's suggestions are mostly pop-ups, score changes, and "Great job!" messages, push back: *"These grade the player. Instead, show me how the game world itself reacts so the player can see why their action worked or didn't."*

</div>

---

## 📚 Sources

- Gee, J. P. (2005). Good video games and good learning. *Phi Kappa Phi Forum, 85*(2), 33–37.
