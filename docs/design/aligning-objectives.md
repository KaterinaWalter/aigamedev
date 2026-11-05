---
layout: notes
title: "Aligning Objectives with Mechanics"
parent: "Design for Learning"
nav_order: 1
---

A good learning game doesn't wrap content in a game. The thing the player *does*, over and over, is the thing they're learning. This page covers two frameworks for designing that way: Squire's idea of games as designed experience, and MDA (Mechanics, Dynamics, Aesthetics) with LeBlanc's 8 kinds of fun.

## Table of Contents
{: .no_toc .text-delta }

{: .fs-2 }
- TOC
{:toc}

---

## 🎯 From Content to Context

Kurt Squire argues that games teach through "a grammar of doing and being." For designers, he says, this shifts the question from <span class="highlighter">"delivering content" to "designing experience."</span>

He draws a distinction (borrowed from Rieber) between two kinds of educational games:

<html>
  <div>
<dl>
  <dt>Exogenous games</dt>
  <dd>The context is a <strong>motivational wrapper</strong> around the learning. Squire's example is <em>Math Blaster</em>, where the game exists to make drilling math facts more palatable.</dd>
  <dt>Endogenous games</dt>
  <dd>The context <strong>is</strong> the content. In <em>Civilization</em>, the game's model of how geography and resources shape history is the argument the player learns by playing.</dd>
</dl>
  </div>
</html>

Here's how the two compare on a few dimensions from Squire's table:

| | Exogenous | Endogenous |
|:--|:--|:--|
| **Learning is...** | Memorizing a prescribed set of facts | Doing, experimenting, and discovering in order to act in the world |
| **Knowledge is...** | Discrete facts, true because the designer says so | A tool set for solving problems in the game world |
| **The learner is...** | An empty receptacle to be "motivated" | An active, sense-making person who brings their own identity and experience |
| **Context is...** | A wrapper to make learning more palatable | The "content" of the experience |

{:.highlight}
The exogenous approach is often called **"chocolate-covered broccoli"**: the game is the chocolate, the learning is the broccoli, and players can tell. When you vibe-code a learning game, AI assistants tend to default to this pattern (answer a question, earn points), so you have to steer them away from it on purpose.

---

## 🧩 The MDA Framework

Hunicke, LeBlanc, and Zubek's MDA framework breaks a game into three layers, each causally linked to the next:

<html>
  <div>
<dl>
  <dt>Mechanics</dt>
  <dd>The rules and components of the game, at the level of data and algorithms. The actions, behaviors, and controls available to the player.</dd>
  <dt>Dynamics</dt>
  <dd>The run-time behavior that emerges when mechanics act on player input and on each other over time.</dd>
  <dt>Aesthetics</dt>
  <dd>The emotional responses the game evokes in the player. In other words, what kind of "fun" it is.</dd>
</dl>
  </div>
</html>

### Two perspectives

The key move in MDA is that **designers and players come at the game from opposite ends**:

- **The designer** builds mechanics, which give rise to dynamics, which produce aesthetics: **M → D → A**
- **The player** experiences aesthetics first, then notices the dynamics, and eventually figures out the mechanics: **A → D → M**

<div class="imp" markdown="block">

The paper argues that games are "more like artifacts than media," meaning that <span class="highlighter">"the content of a game is its behavior."</span> This lines up with Squire: in a learning game, what you teach lives in how the system behaves, not in text or media layered on top.

> **NOTE:** The authors use Monopoly as an example of MDA in action. A mechanic (rich players collect more rent) creates a dynamic (a feedback loop where the gap between players keeps widening), which kills an aesthetic (tension, since only the leader stays invested). The fix happens at the mechanics level, such as subsidies for players who are behind.

</div>

### Why this matters for learning games

MDA encourages **experience-driven** design instead of feature-driven design. For a learning game, that means starting from two questions: what should the player *feel*, and what should they be able to *do* afterward? Then you work backward to the mechanics.

---

## 🎉 LeBlanc's 8 Kinds of Fun

"Fun" is too vague to design for. MDA replaces it with a vocabulary of aesthetics:

<html>
  <div>
<dl>
  <dt>Sensation</dt>
  <dd>Game as sense-pleasure</dd>
  <dt>Fantasy</dt>
  <dd>Game as make-believe</dd>
  <dt>Narrative</dt>
  <dd>Game as unfolding story</dd>
  <dt>Challenge</dt>
  <dd>Game as obstacle course</dd>
  <dt>Fellowship</dt>
  <dd>Game as social framework</dd>
  <dt>Discovery</dt>
  <dd>Game as uncharted territory</dd>
  <dt>Expression</dt>
  <dd>Game as soap box</dd>
  <dt>Submission</dt>
  <dd>Game as mindless pastime</dd>
</dl>
  </div>
</html>

Most games aim for several of these at once, in different amounts. The MDA paper describes *Charades* as Fellowship, Expression, and Challenge, and *The Sims* as Discovery, Fantasy, Expression, and Narrative.

<html>
  <details>
    <summary><strong>A NOTE ON THE WORDING</strong></summary>
    The MDA paper's version of the list words a few of these differently: Narrative is "game as drama," Expression is "game as self-discovery," and Submission is "game as pastime." This page uses the wording from LeBlanc's later talks.
  </details>
</html>

{:.highlight}
For learning games, **Discovery** and **Challenge** come up constantly, since both map naturally onto exploring a system and building skill. But don't overlook **Fantasy** and **Expression**. Squire points out that games let players take on identities, like thinking and acting as a scientist would.

---

## 🔗 Putting It Together

Here's a process for designing from a learning objective instead of from a game idea:

1. **Write the objective as something the player does.** "Understand electrostatics" is too vague. "Predict how a charged particle will move between other charges" is something a mechanic can require.
2. **Pick 2–3 target aesthetics.** Which kinds of fun fit your learners and your objective?
3. **Design the dynamics.** What has to happen during play so that succeeding *requires* the skill?
4. **Choose the mechanics last.** What rules and actions will produce those dynamics?

<div class="task" markdown="block">

**Alignment check:** Imagine removing the learning content from your game. Does it still play basically the same way? If so, the learning is bolted on, not built in. In a well-aligned game, removing the learning breaks the game.

</div>

{:.highlight}
This check is for games that teach a **skill or concept**. If your goal is to shift an **attitude or behavior**, some off-message content is intentional. See [Designing for Attitude & Behavior Change]({% link docs/design/attitude-behavior-change.md %}).

### Where to go next

- **Check your design in detail:** [LM-GM Mapping]({% link docs/design/lm-gm-mapping.md %}) links each player action to the learning it supports.
- **Plan how the game responds to the player:** [Feedback Design]({% link docs/design/feedback-design.md %})
- **Plan how the game gets harder:** [Scaffolding & Difficulty]({% link docs/design/scaffolding-difficulty.md %})

---

## ✏️ Paired Prompts

### Brainstorm aligned mechanics

Use this when you have a learning objective but no game idea yet. Paste your context block first.

```
I'm designing an educational game. Here's my learning objective:
[objective, written as something the player can do]

My learners are [audience, age, prior knowledge].
I want the game to feel like: [2-3 of LeBlanc's 8 kinds of fun].

Propose 5 core mechanics where performing the mechanic IS practicing
the skill, not a reward for answering questions about it.
For each one, use the MDA framework to describe:
- Mechanics: the rules and player actions
- Dynamics: what happens during play that requires the skill
- Aesthetics: which kinds of fun it supports
Then tell me which idea is most feasible as a small 2D Unity prototype, and why.
```

<div class="warn" markdown="block">

**Watch for quizzes in disguise.** If a suggestion boils down to "answer a question to unlock X," it's exogenous. Push back with: *"That's a quiz with a game wrapped around it. Make the skill itself the action."*

</div>

### Critique your design

Use this once you have a concept, before you start building.

```
Here's my game concept:
[1-2 paragraphs: learning objective, core mechanic, how a typical round plays]

Critique it as an educational game designer. Use these lenses:
1. Squire's exogenous vs. endogenous distinction: is the context a
   motivational wrapper, or is it the content?
2. MDA: trace from mechanics to dynamics to aesthetics. Does the
   chain actually produce the experience I'm going for?
3. The removal test: if I took out the learning content, would the
   game still play the same way?
Point out exactly where the learning is bolted on instead of built in,
and suggest specific changes to the mechanics to fix it.
```

---

## 📚 Sources

- Hunicke, R., LeBlanc, M., & Zubek, R. (2004). MDA: A formal approach to game design and game research. *Proceedings of the AAAI Workshop on Challenges in Game AI.*
- Squire, K. (2006). From content to context: Videogames as designed experience. *Educational Researcher, 35*(8), 19–29.
