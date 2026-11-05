---
layout: notes
title: "LM-GM Mapping"
parent: "Design for Learning"
nav_order: 2
---

MDA helps you think about the *experience* of a game. The **Learning Mechanics–Game Mechanics (LM-GM)** model gets more granular: it links each thing the player does to the learning it supports. Use it to check a design (or analyze an existing game) and find the spots where gameplay and pedagogy actually connect, and the spots where they don't.

## Table of Contents
{: .no_toc .text-delta }

{: .fs-2 }
- TOC
{:toc}

---

## 🧩 What LM-GM Is

The LM-GM model comes from the Games and Learning Alliance (GALA), a European research network on serious games. It starts from a problem you'll recognize from the [Aligning Objectives]({% link docs/design/aligning-objectives.md %}) page: learning goals and game mechanics are designed separately, and they often end up not matching.

The model puts two vocabularies side by side:

<html>
  <div>
<dl>
  <dt>Learning Mechanics</dt>
  <dd>Actions drawn from learning theory: things like <em>experimentation</em>, <em>observation</em>, <em>repetition</em>, <em>reflect/discuss</em>, and <em>feedback</em>.</dd>
  <dt>Game Mechanics</dt>
  <dd>Actions drawn from game design: things like <em>resource management</em>, <em>time pressure</em>, <em>tokens</em>, <em>role play</em>, and <em>levels</em>.</dd>
  <dt>Serious Game Mechanics (SGMs)</dt>
  <dd>The links between the two. The authors define an SGM as a game element that connects a teaching practice to a concrete game mechanic tied to <strong>what the player actually does</strong>.</dd>
</dl>
  </div>
</html>

Mapping a game means filling in those links, one player action at a time.

<div class="imp" markdown="block">

The authors are careful to say that LM-GM is not a formula that produces a good serious game. It's <span class="highlighter">a method to analyze a game and suggest mechanics that could support deeper learning.</span> Think of it as a lens, not a recipe.

</div>

---

## 📊 Mechanics by Thinking Skill

The paper organizes mechanics using Bloom's taxonomy, from lower-order thinking skills (LOTS) at the bottom to higher-order thinking skills (HOTS) at the top. This is the most practical part of the model: if your objective targets a certain level of thinking, you can see which mechanics tend to support it.

| Thinking Skill | Game Mechanics | Learning Mechanics |
|:--|:--|:--|
| **Creating** ⬆️ | Design/Editing, Infinite Gameplay, Ownership, Protégé Effect, Status, Strategy/Planning, Tiles/Grids | Accountability, Ownership, Planning, Responsibility |
| **Evaluating** | Action Points, Assessment, Collaboration, Communal Discovery, Game Turns, Pareto Optimal, Resource Management, Rewards/Penalties, Urgent Optimism | Assessment, Collaboration, Hypothesis, Incentive, Motivation, Reflect/Discuss |
| **Analyzing** | Feedback, Meta-game, Realism | Analyze, Experimentation, Feedback, Identify, Observation, Shadowing |
| **Applying** | Capture/Elimination, Competition, Cooperation, Movement, Progression, Selecting/Collecting, Simulate/Response, Time Pressure | Action/Task, Competition, Cooperation, Demonstration, Imitation, Simulation |
| **Understanding** | Appointment, Cascading Information, Questions and Answers, Role-play, Tutorial | Objectify, Participation, Question and Answers, Tutorial |
| **Retention** | Behavioral Momentum, Cut Scenes/Story, Goods/Information, Pavlovian Interactions, Tokens, Virality | Discover, Explore, Generalization, Guidance, Instruction, Repetition |

{:.highlight}
Notice where **Questions and Answers** sits: down at Understanding. If your objective is about analyzing or evaluating, a quiz mechanic is aiming too low. Look further up the table for mechanics like Experimentation, Simulate/Response, or Resource Management.

A few mechanics in the table get their own pages on this site:

- **Feedback** → [Feedback Design]({% link docs/design/feedback-design.md %})
- **Tutorial, Guidance, Repetition, Progression** → [Scaffolding & Difficulty]({% link docs/design/scaffolding-difficulty.md %})

---

## 🚦 Gameplay Facilitators

Not every mechanic in a learning game has to teach. The authors suggest that mechanics linked only to the Action/Task learning mechanic add fun or challenge but aren't intertwined with the learning itself. They call these **gameplay facilitators**.

<div class="task" markdown="block">

When you map your own game, mark each row as either **learning-bearing** or a **gameplay facilitator**. Facilitators are fine, since games need fun! But if *every* row is a facilitator, your learning is bolted on. (This is the same red flag as the removal test on the [Aligning Objectives]({% link docs/design/aligning-objectives.md %}) page.)

</div>

---

## 📝 Mapping Template

Copy this table into your design doc and fill in one row per core player action. The first two columns come from the paper's mapping format; the last two help you spot weak links.

```markdown
| Game Mechanic | Implementation (what the player does) | Learning Mechanic | Thinking Skill | Learning-bearing or facilitator? |
|:--|:--|:--|:--|:--|
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
```

<html>
  <details>
    <summary><strong>HOW TO FILL IT IN</strong></summary>
    Start with the <strong>Implementation</strong> column, since it's the most concrete: describe what the player actually does, in plain language. Then name the game mechanic and learning mechanic it involves, using the table above as a vocabulary list. Finally, check the thinking skill against your learning objective. If your objective is "evaluate" but your rows mostly sit at Retention and Understanding, the mechanics aren't asking enough of the player.
  </details>
</html>

---

## ✏️ Paired Prompt

### Build an LM-GM mapping

Use this to analyze your own concept, or an existing game you're drawing inspiration from.

```
I'm designing an educational game and want to analyze it with the
Learning Mechanics–Game Mechanics (LM-GM) model (Arnab et al.).

Learning objective: [objective, written as something the player can do]
Target thinking skill (Bloom's): [e.g. Applying, Analyzing, Evaluating]
Game concept: [1-2 paragraphs describing the core loop]

Build an LM-GM mapping table with these columns:
Game Mechanic | Implementation | Learning Mechanic | Thinking Skill | Learning-bearing or facilitator?

Use one row per core player action, in the order the player encounters them.
Use the LM-GM model's names for mechanics where possible.
After the table:
1. Flag any rows that are only gameplay facilitators.
2. Tell me whether the mechanics reach my target thinking skill.
3. Suggest 2-3 mechanics from higher in the model that would make the
   learning more central to play.
```

<div class="warn" markdown="block">

**Don't let the AI be too generous.** AI assistants like to find a learning mechanic for every single row, which makes any design look well-aligned. If every row comes back "learning-bearing," push back: *"Be stricter. Which of these actions would the player do the same way if the learning content were removed?"*

</div>

---

## 📚 Sources

- Arnab, S., de Freitas, S., Bellotti, F., Lim, T., Louchart, S., Suttie, N., Berta, R., & De Gloria, A. (2012). *Pedagogy-driven design of serious games: An overall view on learning and game mechanics mapping, and cognition-based models.* Games and Learning Alliance (GALA) Network of Excellence.
